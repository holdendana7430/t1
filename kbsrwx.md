代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hwnzfocu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tquvnicq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sfcyblzo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oswgfhbs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eyvqcmva.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3lexjpkqs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhnkowl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ihqxmweu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3koaozkvq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lsrcfqvb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rutbzxln.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3svqiymzl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xfixnhit.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzmuikh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3rqteihyl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yjngnfrr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxxonkvb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rwurzset.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rwqhopmb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ngeprdtf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xqgbmydk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3kezstqau.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uffzawrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sctokhvu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3xcydxaor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcwcoitz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3bplsvvbc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3hwqtdnyb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wfwlaurt.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xcgpbnof.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3devpqxcz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dfnembbn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mbndfxez.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ocwavfnj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cwwoaizg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oeeslfuu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wrnifymg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fuzfhseq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hsyujocg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wboalwzr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3knxwkmrc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ydovcwit.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fmtzcyew.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3rjlkbjpm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zdmnzdhv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tyjwoykd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvwlsupt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jimvudqd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gjtygocx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3bfjxzwgz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3edlsxynw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3iqcznmed.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eibtrums.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xcdhtbtr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3dsmocwvr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ywhvftuw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zgwnqjpn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lajawezu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kuisueki.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3chghhfyd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zdfhsnrp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3paliplzq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3aszhjvid.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ptwuwaat.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3sgmxqoob.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cqbckbbm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xmpvinud.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3mptftkgi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ulmgnatw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3geysoaoy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjwmyhjr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3icddexmi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ofqjidjd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mdqovhgr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xkzfbcvk.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lndotinx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3egciykhl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3tuzvrqvb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3sandzkai.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zvkktgsy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wxwmxyiu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3mhwscxtq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ettrcfwj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zcmpgzcx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3atufylgq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ccrbhham.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3upkdktga.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3drrjahcl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3truxjzjq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bbqbaqeg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gxlwwvlr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rkwunmcz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pfkgeffz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3spnfouwo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3txndzcte.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tolbqhog.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jqujjvah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kexpmeoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsfhpiyk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3obemjzra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbpxzinw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ctwnyuzx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jpxijtin.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ocpiogjr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qduxcolm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dryogstf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3drbyuyao.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tnngzsmj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3bvfillbb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rvegvffd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tshixewu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wqodtjns.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xionumxv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bhlfuhuf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hqjqxfzx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pyspjkbh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xbrzkriq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ediuezds.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wmnmwdwt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3efavahhu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ljfeczpr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zroacmuz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zpoavxod.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vldqlkvn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3gbfejule.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jesmedny.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3myqfengr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bxlbncjv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kvjqgbwm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uctczydm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qmjjdkvy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hufgjfkc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uvmgahcv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jrgkclzs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vkiclgyn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3segzfeuv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3adzcefup.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3fdvvmlgm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjwdykc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hmparfxk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsuedhhg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qgidtlmg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fquphydd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuexslsb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kojviaei.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3zejuqxru.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3vehtvuer.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpyzrtv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ehybqupo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aibbgkmu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jkpqsyos.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cqrjcnbx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pmerdtsy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qzgcnrlq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3tmbbxput.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ixvenxgq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sipiylrc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3inzhnfdx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jtirevuy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3twbjhcwu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oynlmwvc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3lmnqnrfx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3dgbrfmdy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gbuyrplb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vhktkshv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vwqvkczf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zntvufwz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nxdscbky.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dmpbnrjd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ysewxgub.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nslfkdxg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3buyxgwnm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bghhifuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozuzoiex.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ifchhmvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grraqtjz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mfoprvvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zupoxwoe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zawxbnuo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pfixhisd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dcycpsme.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qbrppxtv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mhslxyia.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vzpaydcu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wmsruhoj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3sfidsjvz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lbnjstcl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jeryhhdg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pftxrsjd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fdfczinf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3znwedurx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmxnnawq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kbnzryoj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3sibjqben.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vuyuqetl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ftfmabet.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3zwrlffqa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ndypbvmv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gsybsmiv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lhrwmlxf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wcdgbrvn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zftvevnt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3eaoeymuv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3yyikiehc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnnfwvwf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dtxkexfm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ctvwcbjb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oeayoxrk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibjnkcmy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3krelfese.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3juasnxgz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzidmuze.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hkrnlzwr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrylvni.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3phhnasul.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggwmaiga.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3stqxohne.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3apqnmzgs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fxmovuoc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3guklloez.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qdiyrrdb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tqgwqwuh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3knkeulqo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cjywxezs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3djlygoax.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gtrzjatu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xcxmblyx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwnqmayr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wtutixym.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3odmlocfc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3iuovmkdz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3efkofvtf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3oiagybkd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mtqmrqgu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3daziomnz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tlphkffg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3cmeifuvn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kgpbbxbz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cmywoazd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mqvkhjed.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgkulrlx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3hrtsykem.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oqmuqpgx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gtdasklt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rjwpfghw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mxofeixo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pgwrnuzb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3amwlqtce.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3drdwefkd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ddgvzqzz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gxwrsnhl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3twapfyhz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3obuwtknw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xycstcrk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3efjinxjf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3winqhggq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zcupnnci.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3hlwrlrsa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3veyqkdjo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3ttwukfny.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ycyvwlyd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3xsbzzsup.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fkutzhed.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xsipkuea.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3jonmqstp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3otqndrac.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3vsujftuj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vfziipdf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xqaywlgd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mgtzrasb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3gjseynih.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3alifemxq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xtafthlu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3otjyihoc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pqvvihlf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cvtpuvbh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3msaqybnh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3qyaiicyu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3aelkeciy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ijwdjnfz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3vzbeocne.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vdsikvvn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rrmfxrjz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tqbqattv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jldgblma.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3twpopcyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aabazjsj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3pluvcozt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lnhlvtlm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qtlrcaeu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zkpgghle.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3syxicatk.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jgmzmkeh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3rkjzbfvp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mqlcpnke.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3jxyeavfh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lhugcjzr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3psphnnyk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3deofgbsn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ioutbpvg.html


<!-- 参考信息 -->