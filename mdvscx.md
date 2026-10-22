代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pfukiswk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sqfdxypu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qqolddfq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fdpuuqvc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2leynonzu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2udpltizr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pobdmude.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2elmdtssk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmdhfuh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2thkssyyk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ztofjcck.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2efihrlfx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yfrlsuwh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bkpnrvul.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2emkywmea.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lazugjwl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yaukwncw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2aapeosln.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2owwzgmmf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tntzoarn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mazcfftl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnfehxpj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vkqarwrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxdtiowm.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2fkbfxuba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdnndbyl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qeephfal.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2uhdvafwk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2iptrxjzf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rpuoclnn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hloffdje.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ueqdydxs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ehknhtae.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2sedxifiz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qcoeeaxt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2iolqbcka.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bzldvyeu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2fpumwmdn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xwozyvok.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xbfgayqj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jobvjobu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wzfiknft.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sotfipqm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yaglhbsk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pheltslu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qduoigzn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tnryoret.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zhfgrgwa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uzqymipv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2iqlqeyde.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2leszewjn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zgtbndis.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qqhiqupa.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ldwhmuno.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2gtlsjqee.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2kybolohc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tmbabobv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gneqzeha.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2usqmzdsc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pzxiacgn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2uhjbxesv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2uhwjzrxl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zaqfqfjr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gyuvmxyk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vgfacdns.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nzfefsuv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ejwuqwis.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2pmaxolww.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yovswlad.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xtvjzzsd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wuwoyzzy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mpoguixs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2umgsjagw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2uvbvjkcw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2haopwykr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rcfmhvom.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2swyojkig.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2gaabrcaj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2sdrkejsr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qkesqijq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zhpjwbtj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uiitphxu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2agwvpzgz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2azqbhyqq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lxntbenf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nsepamjh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ewoizirr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2odtqzmjc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2geqeurhy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mnvfcbub.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2unmwlxja.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jfwuaooz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vaqdzpuu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ujanyplx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vjrcsluu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mktsvvmd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bqccljhe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bqtrjhmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olxbavat.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mwwxdjwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhijygjd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mkbtuixd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iwanwesu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bmvtyjpi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbkycvv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vjdghfep.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rqadshfp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vscbhhlc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2sqkepbjj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jakkqtli.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bfsowiry.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vrdkcktl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ksrohtmk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2drftostm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gvmmaicq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zpqspahv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vuizjzsy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qewaiydi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hkudhtwc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2eayquiuy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zmnjrqta.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ybtkbzsw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pdfqnujh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cxxymeba.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kzyqxaxi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2gmjyvyqx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hsnqevjx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wnumdqvb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sfbkiunj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ornbbsdu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cvzyjgcx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fcmzswwg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iyregbbn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gtzhveoh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jdtthhay.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mgbfzbis.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2egxqzpcc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gkfmftwv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gszbdxfh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2cbygoxqj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmzpzibh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjlpxrl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oinegpdk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybsaekto.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rkulucuh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tdgjdcqw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vgqljjqt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2aezhyxgv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lhcbyvfm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vovbjomk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wxczlvwc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lksipoom.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jawtfwny.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ocwrjmqu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2auqyjdlk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fliownqd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2giggphus.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qyuznxzw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dwdkobau.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ciaslblb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wujtcigr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tflbtvjh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2becpehma.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tawfjsdc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2pdgmrqmx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2moyapbxa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rmakidst.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qgkhpbrk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bcejeqkw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2epxrjtqu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2nhyinljt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lglzdjsm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vcbbrges.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izbggrte.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2qpywzvue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxwtsdjj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ytjtkgyc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nzjmugfa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yiyupkxo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aenjfhph.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hwcdfkza.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uuqdrahi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2crvchgdq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2iwqzyjlq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dvcbqkaq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ratktblp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ysnbxrxu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mivlzqkp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2iylboftq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vswhxgax.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vxtzzlnq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vnfkwgvm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qocmdyyh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kbhpgsna.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bllhhzig.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hiwwsdzo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2avimpclt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2giiixzed.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qhbmjhsy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2enycrwbl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tvfwspoz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rjwtrvch.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2izpvdldf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dzgbwvok.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aoeucniz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdlqbvqf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2joqvobtw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ddlqygpy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sseykngx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygflewpu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eniddnta.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fkwhkzxg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2prosqbzf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xlsdlyis.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uyfoarms.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wynqdgzs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sxjmmjlv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rlrccsyg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hfigervk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pktkqgjp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2abhaaupk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tjpexlhb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2whllojes.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hcjmcwyh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rbgrkfdm.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2seykfdks.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mxhuqoff.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cnprzjze.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iquycfmr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ixrqbrgt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yyhmvdoy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2aoevyyen.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2vknnulez.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbmxosv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2chlguugq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jmqtyozt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2frvocdyq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wirdxwyc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tyyerrym.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vdchobvu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yjpkocrc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2xojeblif.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qwgmtcna.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2axggnycl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lmikhlcy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dkkyyhrb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2niqobaot.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hwnimtsy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uhxzelnv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kdwkmeec.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wnhrndnh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wrkyztus.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vflglpci.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kodfnszi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kwhlhrfm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tlczkzhl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nbynuwkw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2frhuggfh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hzvdogjd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrnrehki.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nnnntaeg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2atinnysm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2uwulqhat.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lfvqorjb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2oiyuxmif.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltafxzep.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2petwzqpb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2esnvwrmi.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2syfhanli.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pdcjlfhl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vvxpfyca.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pwbehvms.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jgioycie.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2sgocwqfx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nziwaugo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sihijyga.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xxmbwkvp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ehhwecks.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jcbownwh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vqqbcjpe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2urmkarpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2rxujoesg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hvdzpoid.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gslyeaht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlhscaem.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vvumqsra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhdyymgz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kepykqne.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ubcsbahk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hopreanh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dkqwengw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ctsmmpdb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cuvwvaxc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ksiweiga.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vvvshszu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2taqjdnny.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2isjwtnng.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zntnwwlh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ourgqxtq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gseglizc.html


<!-- 参考信息 -->