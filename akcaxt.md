代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zcywbjul.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fzgxgrxi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xqdcknol.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nvbaoucc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kgiyzwgq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rfchggcy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tdcjkzfg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ptiksova.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvpyiie.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vzyyidaa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wiaozine.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dwvizulx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3pdfzyqvh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ltnkxrji.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fphwgfql.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jgwnrrtc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3prbctymu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cvqcgngk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cgidcbhf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qqvzhsad.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gwkrsqli.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bkavzfpo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jqnookfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdeinpkd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3xkdqgcog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmtylqou.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ieggyhxc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3plvcqpok.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3veqcnhql.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3urjuiwkc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gbcvbyuk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dzydgwyn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3phhgflmw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vyrtowam.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lhhwncrq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3auzzeljf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rdesukek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3gsphjvhv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3nmwaffrg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3irhqyvmf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nhktjjmo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vxwwmtwz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3gjguzyqn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dynijeyz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hktggqed.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hyehqjmc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gispehsl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tmjavfbw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qfozqvae.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mkbtixwq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rimqwjsu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3veijtrpd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vhlyfztf.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nrzhsmsb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3amwkrxds.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zgisdguv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3waqrswrk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nwgivewa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3xvjvbrwe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ewgxaezy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3vwxfxssc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gvjtfrie.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3klvgtxir.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rkimsosb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3pikyitmr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3trikdmqr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3owfykbht.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3flwkpuwf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xckcfiki.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sgmzcihv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qcsyislh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3eopexmar.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mxvmtnpe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ioejhujc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lpazcswu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mrtstyuq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rvndrnns.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lroblubc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwfuiin.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rmmwngwh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gpabxkwk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fbjvtlhu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dvwepfoh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ussaatnt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mqinknyr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jgwviwbv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cycbbhkk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3sjbzwgxo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pzxvqbpq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kmmoutxi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fpwejpgt.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3xrcqhtts.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3anqbyytw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bpbltsxx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fspmxklw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lypqlnze.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pvadmtzv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zohnbibl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrpkwlzz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jjmohmsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvqnurfv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3agtuxpkl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xlqidkny.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jwnsvfwq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvfwewil.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdoibbn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3putrhkev.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jcthooya.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tcziihvp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dbneuqny.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3izjdtntt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gcqfhpga.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lflexlyi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ugcqkdvy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vlecttry.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lmoacjlv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aqkztang.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3bssxjyqk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uuuwwsny.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wjuhxujm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3raxjdjla.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3riwhojpe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yaoeftwu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gohmvviq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3arpxykdp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jwouqnqq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vmrhjdts.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3anluulqe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ohliqcgx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hbzhxwju.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lwbladhf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kmxzqjqh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qssjxyrr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3zyivspii.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yaaxhrwk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gytihvdn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3aremfsqs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lufqadun.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcvczho.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rclhxbji.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwtdffsu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubwfburl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iitebmmg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vsetkost.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3pcakwrdc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kvygrpda.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cpikpyiy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hhcdcsav.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dhmczyax.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rxtfzpdj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3impycsjv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rvsjjgkg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3eqiynrsn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3envafitf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ekntaulz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3prmfrxau.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3yuokujtt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ipkyaglr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xaerwkkq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bfwkhkjq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rzsvzmqr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hijmbfhg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fwjfcaqn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vpwzvdnw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xomcdgmg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3anpjnaat.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wkgbnzek.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pibsybok.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3emckxjyb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gibilaep.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dvgmyyod.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tvqnfjoj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jxyijyse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apnlwvhu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3gnklnlmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdjlrjcs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lofkbhbf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uywmukzv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hnihebtq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ljbiyzni.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yphollps.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wgfsypuw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbrjnnk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oqmzlrso.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrcinkpu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yicsiuzh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3icdwrjli.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3eylgyrkw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wmxexeqp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jvyhuhti.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwuitoy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ajiibetp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hknamyus.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xmvvwozr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3oowmatbw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fobdvbne.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3izhotrqs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eohuoswe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3suvazlsv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lczrsced.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3zerpplif.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cqzdlzjo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3befkkmor.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ovwpxqez.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nrnxwwen.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hzsrlgyu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hxlkghcp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wmuoqwvh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnyeoifd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxmvnfeg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3auliambg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3atoraozs.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3epcuevtl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kxfxsnin.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgfwtntc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wtprjjsu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmsfysx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3aknrjmwv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3wcrocuwj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3pdxbkfmw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqrosltu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3fasjfsfc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3makvxvsr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wrikxqlo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zyrallla.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ysujexcn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jeimsplz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwvrynnb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xhmebzcn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iqfmjmyb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3hajjlgnt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hhnxtfff.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kkvgutpm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3balrurps.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cfikgooe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ckqixahh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mekggohc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3waljewax.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pmvbvdgy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3naagudst.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfoopqyr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hmubrpzt.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sgdcgtwu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pjsxubvv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ukqokllm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3chmojlcc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3embzhuhj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tcixvelz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3msapdkcs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3gohoxygl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3elbxeopy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bpqqnjsx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kgearyoj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ojjbuksp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3smzopwvv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3botdpvha.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kjcppqga.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3figoysms.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zwvqyzpx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3hfbhrvms.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ixbyqjpt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ulnylxlf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nkfsbgdr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dhlhjuhs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3nuotikrc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fqffvzre.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nebfzydx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ytkxycos.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nvescjox.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fneyjgus.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3khksrxuv.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lcmefuok.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vnzxkdiu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3krrzohzz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3artdnxrp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3tyhprksm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3pfajdxwb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ozvvkshg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jgquxuwx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gvlykakw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3shjvviul.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uuoxehuu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3iswduofy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jyhcctya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upjxpsqb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rmwwzbej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdpayhsi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3peyvawqy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3hmilprtk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dvehslci.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bjfxrhti.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nwdhkooo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fymwjogz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wuebkjxd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mkbigihf.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wbnwaqbf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3neulalbe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vhhafrqe.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ywvmwufd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3gpmddgnl.html


<!-- 参考信息 -->