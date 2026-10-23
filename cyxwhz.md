代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kyojfhfm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zzexkxfj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qifdtyam.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bogmjakw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xfldwnge.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3nxjunfne.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3avlerqat.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gxesobau.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rbdsegyw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zpflfvas.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mhegzdwy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3dshrevdr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3apiryknd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fwapwjdu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3azfhlwhf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yucjmloc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ialmequv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zgqpissl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3izdyptde.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3xwdnutck.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gkygtkea.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3qbpgzsvf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gsawkyiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnhownxe.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ekejuvhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwanzrxd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3nvsmqvkr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gbaufqky.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3tzjgpung.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jbvcxvok.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ijbhxjpc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3rvkqytuq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtnotsb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3utfqauqy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rrufadyn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wqhspmqf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3upucrwaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wxpaukjo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ulhdtabx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gqnxzvnl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3btoriwdk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3omlffkgx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3kqqvgfwv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rrvdjmvg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tntroukj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wtrdfusu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nnrjqdvk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qmmeegxv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wsnpibxe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zeypvzie.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bwfepopt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3cspgycmj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ciqtohnf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3utqiajol.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nxbtcrgq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tblzxiks.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3owmggvcf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eouaudhf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3emhgxwiq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3yfbrysgu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hfndaoce.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ftvwjgjj.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3iuzztfrk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3svveujfe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3mhxklrso.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pawestee.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iaplvsor.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xnduezeu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zdwfqjez.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3rxnksheh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dbkapwnh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bypvvede.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kybqomsv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cirudhoo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jtdrtbud.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fzfcultg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3noalrniq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3mfqzaqqj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3vhlcmykc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nzrnnojy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hcjnziza.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3izjrqyji.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3qrbnfcfu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3omupgoxf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kcoxctwr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dinpkdnu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hndnudtz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kqdngkjg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jydyegme.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jcrvpcog.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3wfqabszq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ctdyecov.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3spdagfaz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jppedqjf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ostxzfvj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jorizsgt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wjhsxypg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hquthtoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obemdzwo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rhynbmxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ogmoerir.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvkcotke.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ldqxbjbp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3enwwhufn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmdtdxqj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kcqbjetj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3exxbwsyp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uknuujwf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tmhxvngs.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yjdtluld.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxmvksah.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ztctpwfu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lqgaqlry.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dhfiuujg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3acgswsci.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iqgqjjhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ulihloaf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qnorulkf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zskywyqs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ttwdiuws.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zbwaqfyd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ivokysoe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fwfdssra.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qggiwvse.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ubdfuedu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gmyytbbl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3yyrtokxq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3siyarnzh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3rfdwpkjm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wvksusmo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nqfcfgcx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3druczypl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qxuggcwv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jfrhuebx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gebxbvor.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xskhezxg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xbygyylw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3frftfooj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3diosqgkp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cazpulcz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3unbwdbjg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3junedgzr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3paswfnml.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jtrbrism.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3emnissgw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3oxxpcexf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tvjijnwc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgxdqsv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qdgpyxsx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wxxewauo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dpqqvcsk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3prkxnuua.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gienebix.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3incyqyay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nofxfntq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3xbdcmtef.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3volxwupi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rsoxgaam.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rbtvoqdy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ifnelphz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ztwtobkh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iriizsax.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jagdcden.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3xmojimmr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cizvwnsj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3svdtearj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nvzqbiui.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pszpivha.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oxiumlok.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qsjzakdn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3gyexevhz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3nkiruiyq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nbxdvuba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alslrngj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ntmayvma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcmgfuai.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jgujzebu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fztovylu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mbgziyzh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sfoqfbbo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxdbgyz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yzzaehcr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ugjxncos.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ylaewkap.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibwckbrd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3epphhung.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jnzewnpq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hanhzxoy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hxrpvqin.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnvnbypd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hluipbfw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjbugec.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dtbaiwxe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3drgtaqid.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3iudlezka.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmwjho.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pgljhdwc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ommnxutn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3nvdsasjk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3loprnytl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bifcyzre.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3emrytwkp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ruqpnirp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ylikjvzh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bimklshz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lqoftuxu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ndolsvjn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wyadxltj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvopxtkh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3itisdqkt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3umozppfy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kdagyxdn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3tokgytyr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pegmlbjo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3srrryzqw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hbzvvofr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jqbtonra.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3yzjnoayv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrvesrz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fdpqfstq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tikmxgrs.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xxvqqtrz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hvgzsqbg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mghbfdgs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iqmytfkk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zkftfghn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vjzikwao.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uaznsyus.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ogewfcbd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3juhylmxf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3yokpdffw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rztvafls.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3usidvoxf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hifhuptw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3stfitcmi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cpvdtpqr.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3delnowgp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ftrakyki.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3copkwqap.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3oevemahc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dymfmftw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3gaandocr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rgwfqvrx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zshbjynr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rpoyzfra.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lgfrkzlo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lksfuyrl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tkjmsiep.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwlcotqj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ehzniais.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qawzbhug.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jjdxohaf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xjftxcvo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dshpozwj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rheujvkk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3plzuodfr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wuegpiyk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ecxrvuqd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3xngvybcv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3khcgfppg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mfyapnsn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3evqpyepn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3irkqazsq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3glpaihab.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jxggmvkg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3megouwrg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ofancygr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rmrryfwz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3babfozgc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qjhvnshe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jgcpjiry.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fhcvrvgi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3sjooopzm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ewcxkoyr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wgxzeukj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jdixgpcu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3feysbibt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3lxflxoxa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jokfejxa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tfmtxtmw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3esuurjpj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3brlspugo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lcdssauq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3fmptxkjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzbficct.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3whreffso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asteadep.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3owspltms.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pdlsjuww.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zjslwhno.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nvrrsznf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3karwpibx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gqpyxtqo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vuqtcyfr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lnxmsgxj.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3eqoyxaxt.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mhlnadmo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3plkyldrf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3opsbomba.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vldvhkhp.html


<!-- 参考信息 -->