代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mdxifctk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3qjdtfvxl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kchwkhdh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3izuxciaq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fuerfbju.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jmcyvfho.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3girjqcur.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3yrradhng.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zrnkuycp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfveolp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3tfiaiisx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykblvpgo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3phmmgnfx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3gnfcuyil.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oyzoztuj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kmssyiib.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ejmnqlej.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ggiphavv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uslkddbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfoxkxuw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3csoinrnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkomwijv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ofhwcgmi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qomsmkly.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3plskrldy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zhmnxems.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kuytcumt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3oocgrieg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vqrccxiq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vublmuaf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3zvcmrqbx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zgykegpx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pfcubvyp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vztklvzx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ymsrgwbv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qjstlcra.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bxmmxzzy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3xkpqnmmv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ucnfswzr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hoknkafs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3yngzshtm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3laiwtvqe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3etjcwbrt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3iycxlplj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tkdefypj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ireixrso.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3oifnkjtp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3awabstpx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fiviwcrh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dwfojbgs.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3gxbwatzm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yaxhzwio.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3czmejxep.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xlowtqiv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tddepjoe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3aeatmkey.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmqelxw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ciegtbsf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ilmfiqiq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rknedzry.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3gfahjrfh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ssntahwj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zouqkbxe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tlzsdtdd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzntgvih.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cjofrabg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kvsvrzxz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3llsbjrju.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3injcbjgw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3jwuohqol.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zbajbwiy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xgolgfmj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uintsltd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xjxnfmcu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hhqezbqu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zjuytvjo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uqxybgie.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xwbqovdj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ewgprggu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hpkygeem.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ghoizruq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xcyfiobg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tvqefyxt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3nitdckoi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3crcsqxbu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mvavftev.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kijvvoba.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rfgkqhou.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vxwrgyjr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ekcgeplp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3noohrgaz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3idleacno.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3uicupslo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tcfnmvqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmiirivu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fvrzqmqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxqepuhf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iqtqdjsp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bsbgjxen.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3kufwlyxv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nwhicyvq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hqpqmxme.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3igfpgsky.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3tatcpgwu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qicrrmfs.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ethmwzun.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ypphdllk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3avbwqkhj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zblbjdix.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oihaeloo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uuikflst.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qhwivtln.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rvardsse.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3afvaxohb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dwhdgxtk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fnlpwmjq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ssfgyucq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rrywknoj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gstfbioe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mbefwmtr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kzmbcmjo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3shhsunho.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zrbwhoxk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qzpraskr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jdrpjbzd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ggytdmkd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ogdpcjjw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vuddfwks.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vkpsfatt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3jisfebpl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wiujbpww.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jpfznkkd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3okahymnn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rewxyfip.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fatqrjma.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3haafvnfo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3edxfhucg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwmqvwfv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3erjkcdnn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtjctdmv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bgonomny.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qaeqwell.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3uifqmwmu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kmzslijd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3txtsjiqp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cdbuwpia.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vupolusc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ydqaquup.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gyaexsxa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ynsyojlf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3szuyhwrg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3hqxmitzo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3nunvaxrw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lmqxvrec.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wbckdidx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ouuqzbtd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zwaepvli.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3yypkektu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3mjdlrktq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wdnfnwyo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dcbeplst.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tqvnrwsu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3iezeohrd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rpcsyygw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dgmntdmv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3uidlpcus.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qdigsxem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kyipgowm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3obkurfbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xthprzbc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pzooywpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dimpzhcx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qjiyhykc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfsnndty.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vzrkormb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ssakdqmr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zdregorj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yffimkzl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfbmwyt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3rzefaywz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aotzvydd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gbztjoex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rsymohtp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xlhbulyz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jwzyfkid.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhppbwsg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zbolbezp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hqrzqtsl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jqbumgiq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gqyxtitb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3osdexojh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3igujaxel.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3aluxqydw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3utsuxeso.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zathwbru.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3biyqajwq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ftbihilp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xhaebxqn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3kzkdqxef.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jyvivswk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjziczx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3udsxweqn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3inguknrw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3osaiwczz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3twwurauh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ixmlkxri.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3miuqzcaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kitnfuld.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3noktuwtk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gbvygqxq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvieiocu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3robsblsr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zadonljs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ehhlmrpz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3kqwfwbhq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bgbuqwsa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nocthuts.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lyprvnft.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dzepibkb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3midkfrru.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dlprrzeg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wrwnmtkc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3esgbsith.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wmshwyhr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3klcktkls.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vwpzzfxu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3gbcldoes.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tpspksws.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3muipzbze.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbvbmni.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lvctvxep.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qumloysn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ydqukfrn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jeiyacpn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3wtahoulx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3cnfjmmbo.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxmususv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bminqand.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wpxupmys.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lncqzehk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ztjphiws.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3syokkdhf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ngqmcwsd.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jgcxmzib.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hhnfvedv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ntanjfqr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ewjvqpxm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jwgafkbr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tseztnsn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vjatmgvs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3mjosuqih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uadjmvgu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rhsxydgu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jqpfvyql.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3unkghruz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzjzxkxn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tsbtqirb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3lnhhvozv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3rqbtblnk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lwludukq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3afguqhmr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ugpyijkh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3tlaffnzv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3wruptksv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3imlrvnfj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kdexwdvd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3knxcjvjm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ayznkklc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fpdsyihg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3stmzwabk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3frixzoef.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3znncmmlg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rslbnyok.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3vmdtqhvp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vjpwhbum.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fdgofxqs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3upmmfkzr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3gofvvfbr.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3fnqcmgeu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3neyqdlan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcusqjxg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gxztnreb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynmpckue.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3cxbcfvqx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gvhznpql.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jrujszgz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zxeijqdt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jhushhje.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ucmxldzl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3oekglzff.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kyrxjkgn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xgqfwltd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ahjadnyl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ifwntvbz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jgvgchzq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3gkxvgakb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ccgzygyj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3liuelvvu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ttdhygae.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3yyrkdmsq.html


<!-- 参考信息 -->