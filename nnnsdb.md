代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2iqdrlivt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sdqevvrx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zaechomv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2xfcgewkv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ttnfwzky.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gfqwiitk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cwsivjrc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mnfydveq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xdtxlnso.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pelfraxg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2djpykhdn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ooyyawcx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vmxaeopf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xxtrrqxk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2huopqfdu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qcvpxuui.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jfkojexo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hombulwa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ujzsflxo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2epjoyfjy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhksgjvm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xjafkqla.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2joexkbzq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2fmzogqwq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2xrqwsdgg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qahmysge.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2iubkdhwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygmokxau.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ojjuzfgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efnvdgfg.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hcgkflrd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2drkdphtf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2prulovnt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kvbevlit.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cwneckzx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2mhnmfvsz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wxwaipjf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2yrxpthsw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dwuwzjej.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hbyizorw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ogeovjin.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bzwmpkuy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ufkqyhot.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2iqafcjfg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uhpglnkv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jzkwxlvb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ipsczofr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pthsafgh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ovhsoqnn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jcmbqnzj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bnyzzaxo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vqpmtiyc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mwmcdhnj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kizogews.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ppghvoap.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fagztreb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jnkmtqqq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2sdnuvvxo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2turdhsbd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2aiiuzlec.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gzznpabf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gfjykuwe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ieuvlugm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ocousrgg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mmqsruwu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vvylkrgs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mbhngnfs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zrydijdn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dtrsmsjx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jyromkeo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mzpeboxm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qvfylvof.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xequpelg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gomcemwl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rwyigdgy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qpgmbbpx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wtpadrld.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rwrmkjrt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ihoblzmx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mpxadyeq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xnhfavuk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bglhgvsl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ctnzfnzn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qaqfyiws.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fxldtkpw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fcwbwgra.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lndvwnbh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yvoacmmc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2elcfrgnx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gacfwost.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lykepiyn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2frsptilw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cxnrhcrt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ixneqqzq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ygujklac.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2laumcotu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vpxvztrk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ngwbcikm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hikfjiwd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lpwyedst.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xubbonvr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2puscezdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oobsdmse.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xrowsrfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqbkdozt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2sonwqdkh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ewcygeei.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qcxqbpcc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gyljyxvz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mmsdrrbg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ersxsmbm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jndfhtjz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2miyazgxl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ezbieoww.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fvmltpdc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ufkgoino.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qigkclml.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ekqxobwl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2oxrwnazz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ubussies.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fduunyej.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2purrvwmu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hqxwauwq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qpcbdcke.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yklbtphx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ypojnhmr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jkxifswc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bfbvckus.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2shghqnpo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xbtuxqrm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nwiwivvw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wnwtzswa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nzztcfas.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yemunbdd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hllbqexf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yppxpnxv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2meyhuhaw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2mhjucfcp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2aoctibld.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2swjtujsk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qrrquiqe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2nifwyvbw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yzevzaop.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ockvtpbu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nymiqdwe.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhgjyjxb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgeptkns.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgcmpwk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2welduarh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2eoxrrzwd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2hbanugsc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aybfplwy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zbkvtdfo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lurlnzlf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mthtysrz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lunibngc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zhpgmojp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pqgrlbcp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mdgfuryc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vhecaljn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2bcusxhfb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2lmxcumjj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lyoilvvo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fukdcvpj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2erlpmsap.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fzzifqbg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2hzprdjwq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zupjhjkq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2musirfkg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ikaqdnfj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mqovvknq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fvvyaiaz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ojeichvq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hhxckmfm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ttszyxed.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2iemaqgvz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cwowgbgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddtffqxc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mjzysmmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxlgdrvr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tpxzccpv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gdopcmpq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2teitvdfu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wdodonfr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rwuplrem.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbkjawvd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2crezhgid.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2yhklypzl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kdfxjznk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qgvdjdib.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zysgavxi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2lbrexwgf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uhwoooip.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2otirucmh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yuhuqjvc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xwuqgxyw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kvwfszpz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xrbbspjr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2whgjgzhy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2szdqzvce.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2efocshyq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fefmkxns.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qqahsosu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rywjqhkq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qgadifnv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2rrijqups.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bldauhum.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bnnygrjk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2siawuyuy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqwqbfbb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2niexywrp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibnygwny.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2isgogflw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2virmbobw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2guzhjbyz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fdrlrofq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zupkziic.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rztosusb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuwwhngc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bvvpjjed.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmejquvq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bthqhsxy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2fzdclkpa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ltwkpynn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufuclant.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qqaaqqyf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kwimcfnr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yjkfssyq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2btdaitys.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rhkpwgop.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qzcaapta.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ssdiviho.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vimanzmz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nbkcpesp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gwslewoe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2uxovogxn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jbalcomr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2krtevnvz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gzcodqug.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2raqywqfp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2lkqarxtv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dgocmepj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2srewivno.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2eoxuxyok.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2isvpdjcr.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2bkpxknwr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sjkckbdb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nihlnpgy.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ingieiww.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gxxhjoxf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hpafrvac.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jjqdjqqy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ikbxrbcd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mfkeyuvl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2arfnqgmc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2qrtibswz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hhqvqktn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pjnrtsmn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xzabogxk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yrqujwfo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nsdzkrba.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2idwpqanr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jtvriqxp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xftcsldi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kaaxwiev.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yfdjsxbp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mqoysavf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvaytek.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2yxwnbdlw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2gclzgjfe.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zdyfhkjs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hkmvnjzz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kiwiyqcw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cydmbkrq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xpranrru.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2uypfnocx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bmidzaup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lhcjjmtq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xitulenw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cmtiqlpf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2qbzvbmfz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2aehbbaiq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ngxaotqa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gqdjecge.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kryzjhya.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gcessfcp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mvtzqmnw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vajtscuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgvpiqws.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ggszjgef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyopbdii.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hpklekik.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zmhbjrvc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qovrlsfj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2jjrxjdkc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jquglzvy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lxfajrfm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rxkmrdpq.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2imovvlfi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2iaphnupp.html


<!-- 参考信息 -->