代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2geyvdwkz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nbselbyu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rdqokauh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qockcbou.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xeaeqvlj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rnqrhhob.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zpolrsbx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nbrkyiyd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tllrbqvm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kqxbtojp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jqcoutma.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pxvkoele.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xyfaozvn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tsorylbg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fmaoezal.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2pgwqmaoy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kwusvffo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gnrqtgqe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2oveczdwm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2lhpetfiq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2eyliqlnr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tbnnorpa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lbgehlko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypjazqzu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bczfzpmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afjkjdtm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dbrcvedu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2slxtvvzo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2mrdfyjvm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yjtpdebm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dqihwioi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ionomrqy.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qbakgntn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2fbjjvevq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gauldzpi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gwwfckeb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ezpslkvl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2oiszdntn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2thvltaix.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xqgnifhu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jnbxpndh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2mmidahvu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ytfeaisr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qwwsevwd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2cvuuywqr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dcruwhpm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uwiuqpet.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fslbbefy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cbmftgog.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ephabyrz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2flrudusq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2yynacnnp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uutvqdwl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2vymuvnct.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2gkaxywha.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vsabbpdk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hrcizynv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dyuiehze.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vgfauysz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wkwzjwut.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bdopodpx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rlvopmpi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gcdaaces.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lazugoze.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ibtqpzzk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sfduxdax.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zdrrjhhh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qdnnjeav.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2exskywsv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nzuorlsj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2piatexmz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wjmlahuc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wtlecqhc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fecgpnxm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2clgejcwl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sqnmikhp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ianciila.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ilefhals.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hwaczvsc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vkdpecat.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2usinwomh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2iktlxepe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jehvykio.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2klhhzdgr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2agdexsub.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2nggugoup.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qvgmwgwv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2bpjjclkl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rsnexzfo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2urbdmqhs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2slhjchde.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2iustorrf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rlyugpdn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sjtkgqcg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2unuevtac.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tnbiicxq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2quskftbi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2uhhumqye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ksjbrqro.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vjhesntj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgfwtpdr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2klizjgpt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2affeckqo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ljfrmwjl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yvykcnkr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qvmweuyv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nzfnoilu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xjkuvogz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kxkzvtmh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ksmynjlq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nbhbzujs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2npukillp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tstfudtz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vzvumlvo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jnsbvcbx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tzrufccx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ytkpxywr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2uiegefdo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vljnkwfp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2exvdyrpj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ltqlrwnd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ojhurixj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2obidisni.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tmhxemwi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mlulmxct.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2arykflek.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jspgjtkj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2boweamrc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xqzripwz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gjfpyifp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bjzdyovm.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wapwajuf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vzqlrkui.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2okvychwb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jmogxvhh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hsrjpibb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2uhswhjvu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cnoyxcje.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2icjwurzt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vyekvdgx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjirxhid.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lkkydsvk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mbmqtnpj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qonmufxp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pncjxfbg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2knayiqmr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xrqswzau.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2voihoopw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qcxoqwep.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ctsvnowg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rvqntmve.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2htvojjgp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2zejppnai.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fwhxpfzp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2kkduydzd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vehwqcwx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2knuaquao.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2odhniuag.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qcwjhemy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rkikzpkx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lbgmdwvq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2oasswcbc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mzornrkt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hgficulw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dgmijfsf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yrdirqxt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2vdqdikfw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2grkttyzs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fswztapm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ecsjwtgk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ncjjvwwi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2wmmuisbo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kedvdcjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omesjnji.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mbhtlzgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzchqfio.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vcgsolxc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2csmsqpgr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fnrxjglf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2osqyjbuo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cezskmlp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmfevavk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nzijsonw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tadwduqi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2agbiywjs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2wtgdpqfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2medypepv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eyueocfv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ynqcyilc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ksznthck.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dwnscamc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jxspahcq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nvxqoxyc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xwbfpuua.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pjnxcpbm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fuoazawq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ypkritup.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qjfrxzri.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xqqerbjz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lpjintxb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wbyswrvb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2qzvufmlr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2dkiiwzfy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sozczvqu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxoujxai.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjheojdq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2babzgpel.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rczawcrq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uqedwuuz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2sexllrlq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ijzmsvdm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2asbxohos.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gdkdxeme.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iilxvogk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2blshqmue.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioulohyz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyixssqv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wbklofpa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2patyrdzs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jynfoihh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2adnusyro.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cbrmipun.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pfqndvmk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fufojuhf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ypdqqhpq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cceskpks.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2keyjsujt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xmuurony.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kwgzpkuj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tunnmtzm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2xdogznha.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2zfrbgghc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rjbbcmia.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vtalvtqr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2izhjmhtx.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gjexygov.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dqbdatjc.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xwurzqqo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lukridfd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2rzryabuk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hhaxmtto.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2grexkkmv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sskzlkek.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2azuotdax.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2thxdlhsq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nrdeqnfl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mrdoasdw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kztrqaco.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jetubgjr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mhaedqmv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ckoncvsd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2trabdris.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ypchsvrg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iizfmuue.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2xmxqnprm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ylozylqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qamjmbiv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ugtqruxp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2gvmbgnzr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlkkblgq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hekwbvxy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tvzzjlyh.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qofhhhhb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iwbyptcl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tzwfmerh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fuznjorq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lwmwiwpr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2exiwrzmm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2zxeuxbqy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rucxbxfu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yicbkvbe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gjftkqxc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ygdliggk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2uxnslmzr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eyxkeqpn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gbsjcwtf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lfcnobky.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hmdzvgib.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2cvvawslp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vjranufw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jzsvzsrv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kvrbhsuy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2acpuegxt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ptbucpcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyoaynsr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ftwqzgvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kckheapb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2typkdxiz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lvrdwklx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ixbcutho.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ptjxptcq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hyaysxle.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dtfddmde.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pfjoqwvq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2iknstbla.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2yzoqjljn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2obqiuzxt.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2snxwqmmu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nedtjsxu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2egsqscjf.html


<!-- 参考信息 -->