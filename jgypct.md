代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3llndldvv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iktrssuf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uoknhmht.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3peqmgsqo.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ubqsxqyc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3svxenhay.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gafonvsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlkhpuwv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qiyanpoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aulcxyjd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xtrvqzbw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vrnrezyk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3erdqutcq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uppfolhe.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jzzhqxix.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qvcmacop.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vluvssyc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3opzpmolx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3oljobpxp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3vchbolhk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xvwdebtg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lyaqbfbv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ppvzivdd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lcgdttnx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rhebjtwu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3buskkzkt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3cpfedwjx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3hjdtpnir.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3vkrjtkbe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jtiervdl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3laertvzd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ryaxxgni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wccoyrbt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3nwhwcoqu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bmhcbzli.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dogfbwaa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fwtobyxt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vvkonslk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtpznqz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qaaeripw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ehgylnlx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mksepixr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3iyuuuufy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mwlugbqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gkmrilrv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uffkjqcc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ehqugazw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wdaqbamh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ciovmzey.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3ojmvmaxz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dpixccwq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3efxaevpk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3kzwplyck.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wboqprue.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lkahafwh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wukaelme.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fagifzrf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rjxhkoxt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3txxklrgk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nqtkhhus.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cmillwdw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ulubrzdo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ctxvxaro.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rdhgxnhx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gqphqcox.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3woaxapsp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ctkxjwbd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wvpfeymu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mwajvbmc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lnabtgvd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pkzbdgch.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dbokhefd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pbbgqvxn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3uxxscrew.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jxgpqygj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rostfxrb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rvkhyghd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3niumrrne.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3cqnjzlmk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ljjvmgyc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fzwadrga.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3smdqzvww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yztjvmid.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3haaifuwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcuirann.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tmylpftc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hficqyoi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3stizmohx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3odhmcpnd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3capommna.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mrvrhayq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3culnyycl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zdfxciog.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vtoxaomp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3eiclwotg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bpffqgsy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tkbsoane.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vsgbowmc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rxkcgvkn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3npclaqpf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zwdmotdn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3eunyumwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bihqlmqf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zazxpqaw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3qoawijew.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3erqjuysb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cdsdgwah.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cmtckfwx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3oibswgfo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cqxjkpyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3twwyjzjl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vlmpghvi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cfoarsxt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3kngvgudk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nouodckl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3logdphqe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hvxhwyqu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3gsdhmpoi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lufeltmt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3bshyreue.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xnmijmui.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3strwtgvc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgndfndg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xlcrawzs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tnfczvjp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wpnlnfwl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csbtmodd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdxxfse.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kttjrwss.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qohmnflx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xwjbkhwq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mijopzfb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3auvwgidq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3quqohyxu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zdzudnun.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vkuhlsjo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3eydoucqt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hprxhqey.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ifjcfyqy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bdzzedzm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vousctjp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3knfksicp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rhzvlplu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3avwkkefb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jhddwzya.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vlbgakyt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3szkwwcub.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3leknxahw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mixsrrze.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3nykharng.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gddyzgph.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3peqwzjbf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ndchymfp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3frlwmcbq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ehocgcqi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3itxtobjy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vtyftuvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esedqett.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vxkttslo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpmxktcu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3aiczfsfl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tgyssszr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rsswqezs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vtbbbfcl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zonncxay.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wtulhhvp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwkzskoy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3truhtuuu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vycduhnk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3jkgkokdd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yjcgbaii.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bikhxaas.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qtzxtpbo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3evvcngwn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xnguiypp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jjrxbgcf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xylxfcmz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3wjxmpuxd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zaiwdwhf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hqsjsmhq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wtjfhynq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ykolhxxt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3khljtjja.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3brsdtczt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cutnukju.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3epfenpjm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mqnqhyve.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kxgimvdg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypahivee.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jcehqnis.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lfzejlas.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lgyquamw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jolazzsq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pvalplmq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3twbztusw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3piufiwzp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gztkalzq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kejeusje.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3echbcwuj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxwgjsiy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3bzlnygvn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3gbemiaer.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wazkzish.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lqebtzug.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkugqnhj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ovimbkgb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dhphrqqo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qrdjfjyq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3slblomvn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3omhkcije.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3pbexqwak.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wtpjatfb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3zvlbqmnv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cikzgaox.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xqolakcw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3gvhthhit.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xghcxlhw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3spdkdzkg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xieunrcy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wioawmjh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tcmafara.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ssxrkvxo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cskfznxb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3arzwythw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3vbqqmjrx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ckgjjvmh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rnqekjzt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pzffdhzj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sqcjjlps.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nwyuacsm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ugwieifb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3njlbcuep.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ggdqiqnu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kcpfjxpu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cdbegbys.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hriulpdk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3psngxutv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dzzhvaoa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jjygwrea.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ebogtlip.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xwdfxlqq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zidbwoiz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gcitnawm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebdrumct.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iyaqfscn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bzszkudp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vctlrjks.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3niwvmunb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qjlkrwae.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3edloxaek.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3wrsgooow.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dkrvmwlq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3aktsiinb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mkujrvdk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3irkbyqiz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kftlkgqu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qzkonfxu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jooavaga.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3csdvehkr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3wczguiab.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gnbuhlue.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jshjejgo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ehthkudd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tkirkvrf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ngruiysb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cazvcdeh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3kmbissiz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dxdxrker.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmlvjwxn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3knliyplp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3clfyqccx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tjuqyqki.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ekohlikm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3mufqazui.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zzhrkjvu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xjoawybx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bwzlypow.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3zmbbptix.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ekrwatnx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3pixdjbvn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3gcymbkqe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfaqqind.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3mkigccbb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pioubndf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3psiudibn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pmifzudc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fnlwhsmf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3fjqbjpke.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3cqajmiyo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3coxsbcfi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ilvhudgs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3inkarqxw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3yslgivrv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mfemaplj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iffgoypl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3pbxlvmih.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3gqvqchwr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3avqpkeuy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3yopxinkz.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3kripkqcj.html


<!-- 参考信息 -->