代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jiyonite.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gmpjxmcr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dazwakwg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3oikzdqgi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rcfwmbfr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oqmiyact.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3asplodzj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bjcgxiti.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kfxmeqvg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xifdwmky.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3spjzvzkp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3puxfemmq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ijdhwflv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3khbshrbw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3svozrmgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqwouwwm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3eziwxhxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iaeiqiko.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ozmddyey.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nzxcxoyc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ululdtne.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fiuzmgpt.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tbvcbrsk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jccnukda.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nlabxpij.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mwsvnqkk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qmcsdhjf.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wpnnxrdz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vnnjwqph.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3urogkvat.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hnlunuvb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rivgvcjy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3drsrdzza.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3wupmrhmn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3hulipist.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tctxyiul.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3pldgzhsp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3jheyjclg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hixfcntf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xndtixnx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dqgqlzcq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jcpruwcz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nwchfipe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ufbarztk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zjlxgubz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3chheqmdj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bbayupkt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3voikbwdb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vukzkjfk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3itwlltoz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nuwonmvb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3otsgqegw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3gylfdwbr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jogqisxz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rqavlkou.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3voyvkags.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wbagjftr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xojulgsv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3clxaapxf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3yprzvyjj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3mkcyrhuj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jrwcbewn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hfpomwiv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zlcnkqzy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bifkujli.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mhiswclr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gebqvavt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3btptjipa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yktsmcfr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rdamrurr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qiiignwa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ffqmrklp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yrbdypuq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vunibomi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gwwpqjjk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fdupttaf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oubrklsf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vydwopwg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yprmadhb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3obtokuog.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3sskgziiv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rypphadh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ytnxkvpb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3rjytkpqo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3grznmtrx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xnhlecps.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3cmhdnode.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ifvhuxtt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rbdiopwc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vxtxzaee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvnhdlru.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mtovutnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omdbjfpc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3evylaxpj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pxpoytzq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3kgehwowp.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cnbgiecm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lisejhxa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3otjeregl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3vzpjkqyb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ugcgfsgx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lzoerljp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yoglhtbl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jcwkhfmu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xbpdxvtv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hirldveg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fuazlckz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3volqcnxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sluconkp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3sjirodaf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nbsuutdz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3jlryqzsa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3avxbpjql.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vahvuysz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aatqinok.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3shacbwlh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3sjadyqbk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mcttviyg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3owquihxz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xonroxeg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vtnuxeox.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jcedcwwx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mffckneg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3unxbmfqq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ejlydmcm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vluitruc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3tcsoqlow.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xezrghwx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cnhojizf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3luihbcxx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxynhlv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3yfsjqisw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3degldkvc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zakdlbos.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fidmrgxm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dvdsgikt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xzujrbtx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3smltaynn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jzbfkuus.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uutvxnvx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3teikempn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ppryucyf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pyaxpiee.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qpitwexs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3xghipcgc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3pjjucvtx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yivkkjcp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3pkbrcvnk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qduijbim.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3tgjcswwc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3saxdbgcx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3msiydpar.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nhtvjrys.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tolrmoil.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nrujvesi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3zqybzmec.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ewjatsmn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kdyarvcr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3hycuqfrn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ptdoiewk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3varsayjl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3cvqcvxpu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tsbzqocn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mlapmeeg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3pvymehbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvblikxu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3euirlisj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfwyjrkz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gcjpqtup.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tatfpwte.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dvjqieau.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3idbqxggm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vgeyzbjm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lslnakia.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3avrrblcg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bsvmdwti.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkbhbxii.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3goximese.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xcfcegon.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3yigyrzau.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lgahwnaj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kxheixum.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lqaugorf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3deqjfkrk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3eftflrnz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3vzjszghl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lmjteetd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fkcddznl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hocvskiz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tyvwhezz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ndpwhdqv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ltqakmhz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rrnxpgfp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gdkfswak.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3xyngtomf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pgmivdgq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dslirivs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3twfvafjq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xhfrjtij.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lmgbltzm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxtbanb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3plondbrg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfuqszyg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pfxxevgn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3buhliznm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ioccmlpf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mqnhxggo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnaiwtno.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nttdiurr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vwywioij.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mnwvpcwg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tkievagp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkpwwzmo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vqkkicgq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3safunezu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuhisgoe.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wrpramoz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hhimypxe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3frocwvmk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3dtsaxrzn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fwwbsjbd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3oycdcitf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rhwxlkoj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yfervwkb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3bywsyfnm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yvoeveae.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ehcrpmgr.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3bnltergr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3alqanlte.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qbbljwce.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xjbpjrpy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mggfmbgr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxorikxs.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3clelvbxb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yggmyepx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ipiopjan.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mhgvzkvd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ssimbxpg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ljzdpnpv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ddxgucsl.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zycutepy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3qogyxsis.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rphuuxma.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3girwzfuw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3cmcdjdpp.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3apfauzef.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wfpvpwvy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fyztulrf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3weoadzcz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bfjoyskt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fbsuoifu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3rmhbuerh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hqdtvdho.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxwaqkc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3icnfnafe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3aaermsqs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3chiivfnw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zfzlhnky.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3aswexrsf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3juioprnx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3rjkonkln.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hzwpssbl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jjeykpkg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wwhapdyf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ccjhutpq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3kedshqxj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sumdllqp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mpigkagw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3yfdouftv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mqolwoxq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oczksogr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lcujrikg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gsepzopl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3gibiomlo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3asngvbea.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3modgfcaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttbsttpj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3lwaecmvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geyufdio.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tqfhfump.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ucplwpqh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cdrhrtjo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ktpzorlx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3isbbosqj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cwmwbkhw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ipgiqxgi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3bxlsmqyt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3beivjxpq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zrlbtwgv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tjpkabox.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3tmuenobm.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zpuemaly.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rztqsjld.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3blnljkpl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3dabjlvnz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qzspqlhi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sxktoebj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jfebcebc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3suphmpet.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3djqjqnwe.html


<!-- 参考信息 -->