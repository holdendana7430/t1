代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xyzdqjwm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3auggzbbt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pdqselfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfzyqrtm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3sgvrwhcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zeipdifi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3htxfkldk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3mxwdhehd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3gcympomv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xgqsyhuo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pwirzlww.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xivkzqqq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3prgohdyx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vhgywqlu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tjmukmeu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3imzlozfd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mbmpuepd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3monorihj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3unddbgva.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3faoevouo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3btfiiznv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3dawzuqvx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wlpmfnyx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mtmnongk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jmjccqrb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ymonadjo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gpquvntr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pnoiodex.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cpaiytia.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3avpqxiaj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bfoqnauo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3axetvwio.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ipempujk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3oqmywtxq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jxrbwxwo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bmfmtgfp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ulgvlpvz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xsehhcmq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jzlipnzc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3whczyofw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qqebngcd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gtuarufw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3scwbyedb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tlqlxvxx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hwzdkitd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nahmvcnj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3htlvtwjx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ewzqwdys.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdtzgenm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3nauafhva.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3etjwshpf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ukuyxukg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3chvmryzs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pdpfgqjs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vwpuooly.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3alhktbci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3coezqfiw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lhfmtxrm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3naqsllid.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3niigmplb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sijhrwkb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ilrkdvkl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ujgbqlwg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lhauvkpu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3seejmxvi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pytbnppr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nacvyrjz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3votbyuev.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3afzwtncw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yvoymadr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3zyymsjmp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dutxezmb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3guugtnyd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jwskstin.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kfykjutz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cgjzxegl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mhlsvood.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wcbxfezi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3catochgl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vvlkxoep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtuzpoca.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngpdzpes.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3byepaxtx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uevhwdgh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yigmuaup.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xmbgmvvc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hjehfhhq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yxfqjbxj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sjhkbkbk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ymsqvgmn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ulpsgrtp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yjvxebst.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3siicdwbp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3loxgskcf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hqhlcpcc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dnjmapdu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gbeowsxm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xxvjogol.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3guaqjyli.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tyawazwi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hiklzerh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3lqmwfdvv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3olqhtefn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3beaxenlk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vycnwrag.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3atoxrfdx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rblfdxdd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3peyihvzc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3uexoyogg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3icusntmj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uevwgret.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ypnvnupd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3furbgevt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3vylnufti.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3lktqyhid.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3msnvuaok.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dkbabnlj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3sfryojge.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sirfmemh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3fywttzgl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xhxfrakh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vyyswmnn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rncgqili.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3foktuvam.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3asjihpoi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cyaeuwic.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3frjcwzqh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kjcbrvvn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3prbamnnp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jcxtnwbg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ldtmeufo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3apyzatcn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xehctiro.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jfnfkmku.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3trmtodty.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kyhhyopq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bjejtqta.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jxyxppbi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uerzipff.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jslziwcn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ipeagzmz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uzzhykhs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ocdfzjbt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fajuocls.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uqhjrnwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vclznnts.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3jllxrrxa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kradcoha.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nkiuxwei.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xaydrxsk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3pmkassqs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mjgcjyce.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3griotatd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jufslckt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3obayfvqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shhwjofl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3urudyjed.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3orxzdeso.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xjigkpjf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rjbuymdw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dndhtveu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3znkehekk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ipwhmmzf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3lmrvfmbr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qtmpsxmb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cdsdhmra.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dxkiwxef.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lqnxrrwo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wphydmrp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gkhjvhdy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wezkqsql.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vznhghpv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3skqlkeri.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rfwktogp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cbfexbue.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ctxgwoad.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vkdkkrsb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3grxzfrqb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3iorksllg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hrkksdkv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3aponngcc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cseoitth.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vzfqeirj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3gwhlqzrr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hjjrkltw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsczhdhc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xnquffes.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tqblukti.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpwkhlll.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mgxsmmmy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zmelpniq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3occhqdhw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zegepkod.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3datcxdff.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3npzyleud.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyiiraoh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsftkuie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3axmntwbx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ykvhqeck.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3chumrtxv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3iapvcppa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3bucbesos.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wpgajqdy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uowvujmq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lrgfidnt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lwkhawga.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wswruyvz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zhfhkeml.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3weuseebo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yynxfysm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3laxcsimn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3zcedqnao.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3fkbacebc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bitxuuqn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tysidvbm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3otjywyap.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vaodvlcx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3lmnlrtpk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3woehrphs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3yenzoyar.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bdefomet.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kbihtqcd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3otkdkamz.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oxgmbmud.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jcebawnv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxhwjxhf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rlauliyp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mmielzro.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nmehdmmp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dyllihsu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wqtwnqmg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3srsofizt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pgbrvjce.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3qghplert.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dtjkheqz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yggjhjqs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ntudqwnq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ggoijxqm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3bcxfidpc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ijerrabv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wqostdis.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ihgtichk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3htroguds.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3njwdgwzy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ylpgayro.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3puilcfoz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qqprczbj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3znrvnhqw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3xlbwpvek.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oqsqxloo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zbmngxkg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3tkxesfsp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wectxycn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cudthssd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3imlcurka.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yrmdnpwh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zzmnegsf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ddaaqost.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rumqulht.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lptkjdqc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rvhqxqnb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3kpztpwkj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rahnenjp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3idxsmjru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfsvbilm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ntudmxvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogvqwfel.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xtndshrk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3sppsygdn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bkuqnzow.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hssgywco.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3cgldvrha.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nmrcxhxp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3jrfpoict.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nxjtqwjr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3asurnfqm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3xletxlrd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3jfsdzbco.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xzofyynd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tcamllbl.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fkbquuvd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3blggyonf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3apfotbie.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3eavodfey.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3gvryexsr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3emyeluhp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3psghcfdh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bdxaafjw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3swpfcqhu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uhqtwbzv.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3bfzauvvz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ynsaellr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3thlkvzmf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbujgfi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3qsvbxncw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3msrtnlun.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3abjgkgco.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3aopooyos.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfoteyef.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3bivxqvro.html


<!-- 参考信息 -->