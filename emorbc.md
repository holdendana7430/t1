代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ofuxfwpp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pcxxeaza.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3nuievcec.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3emwzvufz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zwtejpmo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3etpptdjk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3aunbjtcx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sfdlyjep.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uhfsefou.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3sitftxki.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fdblsgtb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3fsiwellt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ywzsawkr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sarjgvky.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ujeisixs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ttflwuzb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3oiwjezxr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nqqzpmut.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3isqnojus.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zjgukvrt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wepyzbgp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3otsgvfim.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eauvoglb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ryyvvyjw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3swvfeixt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3uquxghhx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3embfjudp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecsiyaag.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jjwelpmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlbykzkl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3cypzoynw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zxswpdiw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3cfrnrgii.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hvpbvhtm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zbwixbnw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3nzfufsbu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3fqnyxkus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3vtaaopue.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uktzlhkt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hdyssesy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xrxmtiip.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3aprejrdk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3yglogqqd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3djcyamnx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3exnohopn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ipnbdslt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qyhioujl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3tgryewns.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ixcihscw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wiedlaao.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qntgxptk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nnvtpkea.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ellwwhuv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jqdteris.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gharwrbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rwgowluq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ibbxrzzd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bjjaafsa.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3tneseuou.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eqdcokpd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kvqicwcq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rrpifqps.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3scuzazej.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qeybpjel.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tgldemhd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wjbvqqld.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eixqdvsg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xtzlfeqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wsiqgrzj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rcgkrfom.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zdqiugyl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3sqhgruoh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jelugbso.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bmepbzfa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hkkkzjex.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3osthjfpl.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lzvtmrjn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gedbiqfl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cndxfgom.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jbjwowoi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rjyyxsyt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3pekefgpr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3bveakbzp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bdjnytap.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dwiasjed.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xomtxuwx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3metpnoxg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vthicacu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fuuuycsi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jxhrpzic.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rspwrffy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tktggkdr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nphzjswu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ssfrwbew.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dnyvvxdi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ualwzzdl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nelqoegc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rrmirnmd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hnaywrah.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3mjqdtfbf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vjmzzatt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hiauteia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkhdqstp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ifdyhivi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufjjxsva.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3edscvfno.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yxtqnnnj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ohfjhlna.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3sfombdkq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zfqmxvvk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rsrshanb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3paugfmbi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hougrvso.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tfdvmrzr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3drqsaakw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3imtrqyhr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bvycpqyl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lbbvubvb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xorzykue.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qoiuzsfn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iezpoebv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3gdnphhsb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wdlconbn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3vjpuvldw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lruwlfdm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3omxkknxb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3spjxwgms.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lzwhzbxl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3gjwdwety.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wvrsyvej.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3snmukccz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ijxfeacm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3shutedom.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3akcfhqnn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3onphlmok.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3busnjmxv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fkankrwi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xgnmylxc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3nxdpotkx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ybjaspwm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ycmxoflg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lxntfkht.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3irdclelm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cskgxtlg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rqvhzswc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3msgjttlg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gowmkxej.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwkkbp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqxldkks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3rgckomox.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bhgngqch.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dsxdnqdx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kjlkiqyp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3asbxqyiu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rfxiqlkb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zxcsnzxm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xyiozqfd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3yuqisijw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fzagblsg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qtgenrqn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3uosgftuu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ndhmuhel.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3peatgeti.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mvnrtitd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oefkmgry.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3squbyvwf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3cgljjoqr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3taeilxwd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rfjivbav.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bbtfdgnj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gfhlboid.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ropphafg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3terldypk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3spdanqob.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3avtpxwop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kaqmnckr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cgaaxpkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjiwsogb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3buflikio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjpxioal.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3efvzwajs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3djndaidf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jsjiirkx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3zttnuwar.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zokrbort.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkqugjye.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hxpodqlm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3cduqkict.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iccjovag.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sydqygqj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jeqfqszc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3otrdylic.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyuqjhyy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3uutfqjoq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3klcvkihq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiiuqxva.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3klyoqdet.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kdcinegz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zmdivlnv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qdjnjcak.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wrmebaje.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dbwyrbsr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yyncyhbz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3munyxsok.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cycvzwrb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3iqcjzmxd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dkuymxuz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ycfmtiul.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghnchrcp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwobulcd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bcfypyfe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zehhaalv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydjrcrwq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pesvmtfh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kttunvqx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ugnxcihw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dssevhci.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ephzpndk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ekiwnatr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxsdafrf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pscgcwrz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3sfwagapm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ymmirous.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrsejpys.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3oansdqxt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aqdvqcrq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ofnyrceg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3icvpspud.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gucvgoyb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pgvvjror.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wvybqbss.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3llfbhosy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wlsdtanm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fxkkxbnu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kzfhhcql.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3clhbbzij.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3sjfbkerc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cgblwvdl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ctammgsz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bphlasfz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3kencxhar.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3wcrsrrlf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hgbjtpin.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3oughobfy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qjxtalpu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3somaicbh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fzifzxgw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ydujorke.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uififinc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3guguwbqf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yednfnhz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pmuljmfz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3efcuattg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3diikndxn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lfjqmmzg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bvnqvxqg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ajqmfkig.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3twxtzoqz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3euyzuxoq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3orscrmgi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3edlwffew.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hpqoqhfr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3glqntucx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3jwvbupiy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lsbujrur.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cuhndwtl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3elbvsyke.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cdmmsrmf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dfttkkgo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rffdbbdt.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eupfrhiz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rnuzhhfu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3giqdawdv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ujeqkvnr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wtpqvykp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jkvytecn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pfqovmwc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nodspjiz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nryzjvxm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3iimbttql.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vckgjaun.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3agggehsz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3czohbime.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kxacftti.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3edysqvtu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nghpilus.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lrqdnjmc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mzqsxuej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjvjvcrt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3govirdoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azvcbniw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fohrpjub.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3lqlkrfpp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3jaciflgy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hrsxdomf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gvvrcdlq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3qbqaooxx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jeitglhh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3cdndstla.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3slavntlt.html


<!-- 参考信息 -->