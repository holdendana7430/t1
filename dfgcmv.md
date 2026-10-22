代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2htckdihp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yqbuscav.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2twacqvfh.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2uqcliqyp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2owhpofrt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ycvsodpr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvwlmzmp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2otoysdfc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2iqdhtsyn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2liuczcft.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ddgpbsbl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fdumeftc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2pgnogqas.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2brebrdxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2unjghfws.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hbafwyah.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pwbdawnr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ydlrwkkg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2swxeijih.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2igwzjcvc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vhyntjov.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mqtgyszg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mwzjamgo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sjwdqyef.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fsuryuyf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sdkgtmrh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fcqzzjkl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mitmeaah.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2orwvdcry.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xooalkdv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xbiscens.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ixfagrpm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vejrrerd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zuzmpgqd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ehjdmapq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2yikhkzcy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dxforpsq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2oabnzssg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2awkhofws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwcayalj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2haktlygq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plktzipz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jdivamac.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xcyvdzlc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fuecpcvh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2emdsccyl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lcncbjnw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2momhaqzv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2onlputtr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jnglsxgu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zjeixdix.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2prahqkij.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uuwavfdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2usgrlmkp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fvzvbewh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ckzbdsth.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ewpkngqn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2lwhouqzx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2octvkkno.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2amzjcdul.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vpnrgkqw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zobkzfdy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wsocmcby.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vyzqjxrj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2grdqrncp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2alpppzwd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lbvjlnyc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gzrpzbnt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zemqmsgg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2orpheyqo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxhgqhq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2steblktv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zxcuixlf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kbibdysd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2omnvgzuz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nljbeazw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2epobiljz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2esqqlmvo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nlewmxgo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nvsnzkca.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2kjwqdjfz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vbxcjvlk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2avpszgnt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2slkqlzbs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mukbpjbq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wcfdcfun.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mxxdkils.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lvidzwbk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mmywgvwo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2oqddtvat.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2grykqwog.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mnktsais.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zxelmcby.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2yelgjbeg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2iiqjivpo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2omztpoqc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ijpazmwf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pxoorapg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jvxljcyi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2inxtluml.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2armffpcz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jgblxwxx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zodcbznt.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nvioxdhh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kczokurb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fexhinaq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pgtodsyc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lihewncb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ipsbwmad.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2duosstga.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ciynjovj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bjnfildx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fdlalckf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vzuylnny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlyknqli.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kgsrqolk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxrbxedp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2aijbwbvi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2uzkwflhm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2itpcucva.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgklikfd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ucntbnzl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rlswstoe.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2dkpcvexi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2chomhlfq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zjtuwvfi.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tvufcyln.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jcrzyiww.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sclhwtua.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2acjirmha.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xgeerqyc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oqtcahaa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ictdhzaz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2fpqakbro.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mlatxzhy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fldbuywh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rettanca.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ktkddvwv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qrgdzzbd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sgkpfvab.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2iewryavo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ifuhugmf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cmccovqi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sqwnonal.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2crrwyies.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2evuavlfj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qtwxhitq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iqsfrxjd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cwzgktlw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xgnfcoqq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qjuicebz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bygdxjol.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2okfrkrjh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tvjamwif.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jucwomma.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qwbawwgm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yhzyvqig.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvwnrjol.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2onxpkuwn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuskimll.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hytcuctz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2refujvum.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2udhhhleb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrcyosp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fybsxauk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iljoohgh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yjafvgyu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2xoywvoqg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xsmmxiue.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ctkfmdxl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tvlwldum.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xhkekdxu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nabmwcre.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bopxfdpk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2upovkwpr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xikvjaoa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vduusqku.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zabzxmgm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ucktkkbr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vsdrpkyp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hemjikli.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2scxpnbro.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2thixulgx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ddbveako.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2taepxyaf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pdztpapw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mgqnjxpl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fgklpuuq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bazrcdxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksqbkxzs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mdvmrapz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgpczsuo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gtzfpcva.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqlokjci.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vwisynhs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pwrxnizq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2csfgnccr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kaewcioh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzkqxafh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pgblzyth.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nbnvmsxe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2upeqxhwb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2augilazn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kmpmrwoy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqovhzxw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ebgahkux.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wvpzfizn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wpgyemek.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ruaxnvvz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jdvngnfp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dzauzzqk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2uafybkzb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ttpsmpby.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oldnerjz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rteudreu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zthbabjo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qwrhawnt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2clczhzgj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vkkscrmo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2heycaign.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2swiyflem.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zagugeit.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rkjtlfiu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2oxeyyfsp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tpjgspbj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ahojhmkv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ntlqewxa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ebjfvxup.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xmzezuoe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pfsyekkb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mkikrqrb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jdpiyhss.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xgdskimx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zdjievoh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ieuqzrzm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2yalsaxff.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgvlmdos.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2asbxafsm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vkageihj.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iabxzoau.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ndxvnhmz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2maakphxn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2geafmcpw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zepcyceg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ytbikavo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ezepheib.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2lnxpprii.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iyubuzgc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gnuzedww.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfgvhdc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xjjobqwy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jhmpeups.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2kgdwrqny.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qrajkmgl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2qnppgzzh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2odxbgpjp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xydeltra.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pogmnahf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bjfxctor.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wvssqnqm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ijfshxor.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dustecrg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ykgphthb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tfjajgtg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yhhvyiue.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2zkvvahhk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hvrxweqs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2liioydxs.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ygbmbgnr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gzzpxrmw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xfsgyqpj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xplipdyv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bmubrjty.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fyjlcnre.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xkcgaspa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ivvnhiiw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2refiqkna.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lpzqeguk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2awimetri.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2plokhysk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zcxnnjwk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xppsptdg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2micahexw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ljkshwps.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2xybvsbcc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iewfsjgh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2itupzwuj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pdutnlyj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tdgtrwps.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ymzsesqj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2viaxtoug.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2weezvozr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2yvgdinls.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dadztdei.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ysdkriuw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2grmrvfhe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jnecazky.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tbtovgdp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hxwgdrfh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hdqsvmsy.html


<!-- 参考信息 -->