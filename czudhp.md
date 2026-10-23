代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uufwsjtd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pvmmpxrq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ybmetdgx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pixntojf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3cwwccmkx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lbjsvjsp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hfjwfhxs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqiacoqw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tuzyyyqk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uwcbamnb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ujozuujk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3dcdvetcz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3iqsdpeyq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vcpwdjmq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hajwakxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjtpgrei.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dyrnjvri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyqxkhmw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3lsurysmy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3sigyubbe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kymuqcgp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhwqkru.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rfmjaqvy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pvcsurbw.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3saafueic.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3douqjudm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aeexcqbl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3skswywwc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3aosmxovx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3tebmnboa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vctqrjov.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ofvbvics.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qziatfrk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ebkzammp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bqboxjaw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijsgpoku.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qhdnpzjt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3kgtefjhq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3lbomhcdr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pcheovon.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lzvqwbou.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pbwydrlq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3unlpemai.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uwdbuobi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fspugmby.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3venluhsc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3vbrdqxje.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3whybjrog.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ytargkun.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vprgdudn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ecjcfbkl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3yiwyqaag.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3npvnstdj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fcuetjpe.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bdidakbb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wzdxcnqu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kqoapyrr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jymezypo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zeiaaivb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3thuaqrgz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yqykkebr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3smsfnjga.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxdvpbzy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nmupdqeg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3keqtpnfl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3sxpgseve.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cumpbhgx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fwpgtboz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3fltthakd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gankhhwo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rehrgafr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nneqsdxo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oucyital.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3qqxmuhwn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wcwzfkjf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uxuybvxz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dzvmmjov.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nomsmvzm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kfbjetwa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vhrpfnxg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gfypygds.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hsjyzzyk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3iggxdwub.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fttcenpo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xgojmjul.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xfdbnhwx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3axqxjmfi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hvkourjd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3loctgakz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qpmnymdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlfmdswp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lirlrhwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcvdxxgn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3msylfrdt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yxpgwnqz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nvforvtg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdowhynq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3djssxlpd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gugyepld.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kduynxei.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3excduozp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wncnrgqa.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xykpfhjj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rmprulgl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3etmnxhgy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mxghliqn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fffapksd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uvrgnplp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ejjrulti.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nwzxacde.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gvpzayqv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ezbfigip.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mydohoqv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3byhafjow.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3oqgwpnol.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3semjjjsg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3pthbhwse.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jxbdhhul.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xvirothz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3znjzrstx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jitoxpep.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qmmjqmll.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pflfqjqn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dwaziiyu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wczrlocf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ywmvlufg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jqffwqjl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3nwjcufbw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xitzwegg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3cyihukgt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3esypplkx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ecssxxmf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3walaslgz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mzebzrzs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jnpvlvux.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3plmslaac.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fnbmuxlr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rbtfigqj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lqzuuweg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fazngldi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fihhivtf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qpujwgjt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3daqcjcmc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cifyeglr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tyslsslp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qdoqpizg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3crrhaowa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xyoilpiv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3smpuvwqw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zjfidicr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3imqpacmu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xdhxaibs.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3kngafdsg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3daepwecm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3louozsws.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxnoleo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sazqqyka.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3drdlwwoa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ngobssvq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cdmphdgh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nfmwzctq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wngipnea.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dmnoafta.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3aicxwnsw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qygufyzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szuilnrw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3vsfhpofw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhwbumxv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hqostknt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tujgoexc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bmghhpox.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3izfnhazr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cjeikqua.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bbgtgzue.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3juauupgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3svtlgfbo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zobnuzfi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ujjzaavi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3srobzhiz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3odvzyxkh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zptdvfvc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kufvzesl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3smqfdjel.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3akgilezz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yuklxxgi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ooegtdlq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vnumhiwz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qteqtokc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hbgdryfg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fvgsgtto.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hktehrhx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dskkyqjp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fciyjntk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bzptilai.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3tyzauwuv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3eqnfgftz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zmgzdlbp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gzhkhzcu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3konvdmcu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zehcqtzd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bgwyluqn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dnpwkuii.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvskuabx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tqlvrfyo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xcsuueet.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aopncdfl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3dlfcyvca.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmqixrqs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaijstku.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mpcxbapz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nkyhkdyh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3goqrjgux.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3znkykbrp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ksjaxqqu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3klfpfxxd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fpkhwxyx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eizghroo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zjqxynit.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gualnlba.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vonkcaxo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xojzpexc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jieckejo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qhdobbzv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ccftpbnk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3osorklej.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3rhtihgao.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3chizrckl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cznrmrdp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tjexjote.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3awibgqgn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3kctmdemu.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bljqvrpc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mdwnuzlc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ldpxjaqo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eoanrbrj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kreirqvj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ydiwareq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jlhctnmy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gmafwwfb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nkyncefx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3twxmmtka.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3nsdlmiib.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rpxtwisq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bmnunons.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3yuhfhzev.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rudwelwh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qnezwika.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3upamuqba.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nsfcktoa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cgoomztz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3apgbaubl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3fldnyxqe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3pxsxxzpn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3jgtrdokn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqqpxlri.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rifsoqqc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xzixekkx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3gjhwpboq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cqeoyyql.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zvryowxy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3whrgglql.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3isnmqqky.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3kvbdhgka.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ckmvzift.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bejqttgj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3shfcdtcb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xsrhlgem.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gjrelonb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jxwwkqaw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3thyiuutl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zqkoyhud.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jwadcgtj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3eajnpevj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbfecmbn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ebipxinh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3oxxpqcqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3veouswjb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rwhcksmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onkftgfw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dohmflpx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ajwwmawu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dknaenjg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uaajzvff.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bndyntpn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3slxtjvhf.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3fcthwius.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3euxzwffq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3haqqbrwv.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3abyfuiut.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hwxeyjlg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3kqwntfgt.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rlznndhw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hzzygzso.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wmgzrrcb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3eihbinvk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lmqxvhhe.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3qsfjcelc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3vasqlpmi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ujovolas.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3oqedmxad.html


<!-- 参考信息 -->