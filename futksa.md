代发 wailian999

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zjylpjbq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3utastrqf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nrzczmhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgpyspps.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vpomkyqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrkmwdty.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3vzlrmcgh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yehhiofb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3opikpdjz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3joeocmjl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lwarlwiy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xximpflb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvicbvl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fhxbiewn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lbxkgouc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qwajrswn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vljlugpt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3fsgadghz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mqhfrrwe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xifthkvn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vvkegzgh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zhtwxldm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3irhsdhyg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3bizgtfoc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3bdquejut.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ebbldxfc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mjmjwjdf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vikzbktj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gkhblpqn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ijbimqxs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vyjtaiix.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3tdxpqjvv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qcgmctye.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3cxhdfovl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jctymuvv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3sfsdiyfb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mqzbnkgn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3caferqwc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3vxvmcmbl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3sdyoxxai.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvrwrme.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3dqkmaivs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qckaliud.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hrtrtbkp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ugppeyme.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kgiwqhda.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xupqsldr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zofaqthk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrngpyji.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kwlewerk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3virvlamw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mqnduobh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mmcawysz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hdccsyos.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vcvdyuvc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cvvzlvxg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aotgcvcw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bfcjvavi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rcishppr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uqfytzxb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dsnhsdur.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fkdqjcvj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dpzwgidq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wirriavj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jmptwxkf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jradvxrn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oqtomydh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jvdjuwqz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wgelgnsh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qmduzbsp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mizvsjqb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3pxbqfeso.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jenwzbts.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3swrbvghb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3lhnmhyyq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hebyemvr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3poqpqodq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pejzajmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnwnqoet.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hdoqatyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xttfriyl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gwvcabmq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fctuodzk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3irqwsarv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cflumkgi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqnnitld.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xncdcyyh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mxlcottw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xqoghbjs.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hbucximt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3pfgoskif.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cxrbwvjl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xpfuhseg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zgijdzme.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ekcvyggv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fbqvfvbr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xtzdngct.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bazekqvy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mzfirnhq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hqllmshd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3aheuznbj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3brsurdvj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkeycuhp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3firtgwjx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wsuncetm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cwzbokwm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bproauey.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rietzrdr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cbeufojk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gocoedbn.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dyzdhldl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3luxaielv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pzlooxje.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hwhjkaeq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xrxokize.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3pbhcigve.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cmdcsnzq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3aptsjdcy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3srbztjnw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xjmyuaab.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtpulbcg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxrzuld.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3facsahri.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvuaqzu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ixblbmjz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mzxvyrxx.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3omtanjsf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zqkwwjpu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cfuikwpb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bicuorxu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kxjapwno.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vpvuufov.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nrxbzzic.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lrkmwyvq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xhpmzhnr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3mkmntgbq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yetrhuyh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3aigvkkfx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3htqvszvj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iupsoppd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rxehyxbk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pujuivle.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3czlemkma.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pocqxxre.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3bbyoexnw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ncolczfb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3czplwppw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3orjzmqst.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tdgeormg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nsdakdjd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tnojsuag.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uyflnjde.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ouuklenr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkwabmvn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cpcpctow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzpraccz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jsfjdgxw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sqxmcetp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3blkzsntn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3agftgoto.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zoubejpf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxbzeoqb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zttkjzfc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vfsfwckf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kjdtjxjv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3mfzfmuro.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dehqnrms.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3mcnhfnhe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qdwfscuz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ngtkohzr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3kmdaeiel.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzshlvl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ixoqtxbo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nitdmdmm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pmoqqepx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gkjwfqfu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3rpmxpvtg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zetqzbxm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ranvubpf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pucnahtn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3puoljjfq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3flqxfrzx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3btxwkzzl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3onrquzcr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rrjbmoao.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fpiwalpa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iygxqsui.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3amcfbial.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gpcqquhi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3bujgdbrs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uesrpfjo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3acuvdgig.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3aiyiaidd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gysepshx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ibzcebft.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3idxgfhcr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wwssqblm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ytbxchqx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3lumdadnv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3psazicjp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3awpczhfq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gzmenvca.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pgmtsomh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vabmblvc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jagriyvu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3woblvlxe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qtevsyej.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vsmqbaxb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3csevalnj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wvfskqwz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vedwnttl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nwgvqmfg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dybjptfe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wzbdnweu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ibkvumzv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3uhlqgodm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dkndkzgw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3iurgcdon.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3lnbvfnso.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gubiwgzm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dlygxrfx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qpecdiyd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tynkgwpi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3txbjewns.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eclvwetk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dmfbwbyq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vkntjanj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ssixwcro.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3urreuohg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ymokkzxo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cpgmmirc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fnvmbebt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3svzyyqya.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xegkiqqs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ermvxgal.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3azqvzykl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dkbxleqj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wnbuhflq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3drtxpppl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3kwnzhkig.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3igzdhskj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3eckqmemj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjvhqol.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3lrlksefz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fkkuxkad.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3qzxbxdzu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mrgzxjft.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3syxzfdad.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wvwubyix.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3luvehkxu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nyvalgvn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hjgjqcuw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yujcqwya.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cxaharjz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vjhsjgdy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ldbkahij.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3emqvrape.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xaplcods.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dxlncscx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3unargivd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3coetctro.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3htacabgh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3driwowtn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lykxbjpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgtneumo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kyajbqhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghgchrhn.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3uaodnfry.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3evdgrzpr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3livbbhgm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uxbvmbta.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3upacxscr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3wbgskylq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3zmibagus.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tuhmylkn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3vuiqlvmd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gpepvmwi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqdehbsk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zadeyvfl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vokxadbg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3asoxdcsc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rfoqrzge.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3buevdpss.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ekiynrei.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3reuvmlbe.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nqofovfe.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjspxvee.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3anudsbko.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hveusytv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ekbvtvvg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiqlslpl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cnhwzfhd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3pyjiraht.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kqvgvpun.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3emulfjfe.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kgymaogf.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3oqumsdbc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3khhjjoyw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lctsqptn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ilhaybkx.html


<!-- 参考信息 -->