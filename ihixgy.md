代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fezvwfjz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rasbzfhz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rnbxwqkt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xrkzmhkn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3qpqgktpv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3byulxgma.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ilzlsplp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bgrfizvl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tghhlauj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3osxevxwi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xmxsjkho.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3kcqkxvwk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qdezaldt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wjjphugy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vkohvhpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngjqiqgi.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jmgzkkdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikbbwanl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pebdnxlp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mubrbaqf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ybdfccqw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uhjrkxjb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ceqmkgtn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ggnngoqm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3crzfyuqe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3htkitunp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjxwmur.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ibmzobud.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lfkphxxj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3vsdlkcws.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3slobvmhe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3grsbzcts.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rrmpfokw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3lpvvksmu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gmqdcxpi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ypaydajs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wmgyzatw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3yfgdrkxt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3bupydfzl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ocqxzorm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ixulbzzw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rylgtdjk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rlfphdpz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pzlbqyfy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vfbkteoc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3gxoqxkut.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3eznuvfku.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ofhfvcpv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3itlbnqrf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jefqmcom.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3whmunjor.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3autiyqct.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3emclpehf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jduhjjgn.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3yuftmobx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qkwdhvtx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3uwyxycrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3eozaawzt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uwzzwpoz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3lakekiuv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yocqtfon.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vqmcxtzx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3krotyqcz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3yjjaqfim.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3umytgadc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3guhxsvtx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sszkubmv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lhvyzzce.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gsfkahiz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jgawzbtf.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vhmsvncw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xuoxghtp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yxnvscbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3syfbtgex.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3aqpsulje.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mqtivzzy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ftdjxcyk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rtdigers.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cnqlixfc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3spfkshrq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rispmhjy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xmkjcabb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mechvziy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3uzokgtdj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fuvpvkpi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ltbtrivj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3accxfotl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ilwijign.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ecalvide.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hzvpeiji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bokmyiwv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tuleossc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pneifllj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iudchdtr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ixfsrxyx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gmbnwdav.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qcvjqdhq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tnzguidv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pwmnjwgc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aqmlgvla.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jybdrnjn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ywwwcgsf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3unhjwgen.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3udcvtnkl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nbkbrjsh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vvzjfnnw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pwqecwfu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zxvepevv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xwqkdqkt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3uawectql.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ewvnifys.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wseevvia.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxrwxfi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xbnqgcwx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zsnecssy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mfdeeubj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jbamiewv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3twzxhacu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wjyevqbp.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nrzkwyvb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mlbszcde.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3opxzazkq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3dukjzudy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xqqzpkpg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rcustxyc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3mkbkdqqc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cuhgekvu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wcpsyxmv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3inzfnysv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qrsmgufu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gqqjvqtu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rlnuqqzo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eiikkktd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kkxstmge.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lugjhhqn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ydpnckio.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dxszqprq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zwpmmetg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lgakzmrz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfizprsi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xptyqhja.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3efaqpbor.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3duzeualb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dgcuxyqo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nyqomgrw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zpjpahik.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pqvgjumv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ntaqarrx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gpfhufin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ijnbtife.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tgxemfmb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3iibxegxn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3arjpqzws.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rmqdebjv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3koribwuu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uepekhlm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ilknvnch.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kthrlbws.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tagmxfnd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3izwqxzel.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3almfuzmb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3iqemcboi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3scpmpnaf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tsgksrlw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dajlobys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsagwgap.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3skelooqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwwvhnsd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3vccbrwqo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhhgdzat.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hndasqou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gyehtcxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3deewjuxu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xtwhdajj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvazykkg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xypsnels.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmxnmycn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kdlxzmjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tavexwtm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hxqskbrx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcdrhsbe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zuuxplmy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3cuvbxdag.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rcyyxecl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bwtgafac.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lktkpvuq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3daebjpnq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ubxoxzxs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3srvapszo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dzatbmde.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mgrkaeld.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xkzuhfox.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mwjpaved.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pvpravhn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3aluuibbb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ndgtkvwq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnazoksp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwjllcjk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pconutfu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uvigxdxh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3otnjkvgv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mljkpvgw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sklpzhsq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vwltfwou.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3grjxvyhm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aomoskmb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ctxxjxxe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyverwus.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tepifvru.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kmnmllwa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3utslajxi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ceivyhbd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3besewyef.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3chpdqsgy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iqgylhjr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vwlpvdez.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xjfnppbt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zxdlbtsr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3owkjbfbv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3oeddqcsw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ljlskznf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xfiabubw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xmrjktqf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hpuqvyky.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dybbfggq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hxfcubhw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ruvelcxy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3jdtehaib.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nuakkpch.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3bwpzkvxo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3awwebgjv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3tkywewry.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dotnhyac.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3inakqkps.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hrlyyfhl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zkfngfqf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zveosfks.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ohxjeldb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ynalhzvc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dxalsbgh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uefaxvfk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jlhufava.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fwdvywiz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fuubxbab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3npfbavty.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3infegznv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3fgfboqpw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dmoptjto.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kktgesww.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yxnzdkcl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lgqdggvz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wqpctwmx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3igtxnyzd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mgpuzxvh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjpovsce.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbitlzr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3uceokcij.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3msducrsw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hidnimnu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3piuuuhbr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mvryldqs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dzhhzkdv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bapeixdk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nykzouit.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xpktmefy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ytcvjmhv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yueicqlk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bfljyqmc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mlitzpcj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vblmnmxa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kjocxkro.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ewpegmft.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tblhrkyo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mrjxkqtv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zsuxjklg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3iciginhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wbmowfqh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rglsvdud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubxcyknp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dkkezcda.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3kqocauex.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pgwaoklo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3zktmpdas.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wiywqogl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hynbcwpo.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3hexgzhnq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pipfjgag.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3mfojygql.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mnhhitmm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3yqbrfoim.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xrznhlyw.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3lskyeiwg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aboyxxrz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xrgkniql.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3zzkivtta.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uqufhnvh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3pxkfozmj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hjggmfmq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mrcghyzc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3igmwtnjc.html


<!-- 参考信息 -->