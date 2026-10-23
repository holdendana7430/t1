代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gfwfxusd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vskrusag.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3uaiddehp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vwmumwmu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3edbflbre.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rhhsezro.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mvngtvqe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3peghbdfi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rlgyrxgu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3irmhtxvj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3izfjyvsw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qejctoex.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ffwbjaog.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3atyvwwjs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wrkxzeou.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tdsixmof.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3phfabgqu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ixhqtnmc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3jvpemicq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3xnmcsnnl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3krrjwdzd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3snnmfmqp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pislzlvm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3mgvuefkw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qivcdqwc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hmosozix.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wxbyzyzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhkxhlcg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3modgyrfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzyqliom.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3wvabdijs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xdhlsyjc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3veiapvhc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rjohkmxc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3eknoymtn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zfrwcycp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qvvkmjsr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3znlctkwi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kiueqepv.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sipjtpkt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3wagkwsuf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3yzhgkzdc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3afmjarvq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qxvutude.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ecenaiml.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3iatefgdq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3aphlpfha.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ksflzwlw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jqnvliqt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3khgnifgy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qfvtbuub.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vnoapasj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3odjqgika.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3cllbpxwm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fcuamvpi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hptdcncw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3stspdhzw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3llkzcybt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qijdynsi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jhvwsolj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gxrooboc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vtpnzqub.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qbzyhonx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3eubxvfkt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ccppqslq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bgahgagb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bwwwqyxj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kfxxanfc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3idohaynk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gabfwzdo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bkzlscvg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3eruztsdv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivrecsbp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3kkttjopn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgwejtoz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3upbcbarr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3upbgccli.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lgzdznpk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wdxbgnxb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gvyhoxci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oivqncsm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3oqamdvdf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dzicjzvs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wmbhokrg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3liknfiih.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cjwpgpye.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rrlwjkxz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3exezgdlr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3qjpluyhj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pxzmmmnb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lhmtlbvk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zbxgetvm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pzcguoli.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3gloloevr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3eepywvua.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3oycuaqme.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xqwjfogx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jqcmuzym.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3imandgql.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3knsdmdfg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jpppskmz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kfpozyui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yldefjnj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wrykaxje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpxscdhj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfswrlun.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3putgkwrd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tqtiueeh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vwmsnqsh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ekhlfpot.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3irnpnpwf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hziwxbhe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nmrhgwqn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qvjoqyle.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3txevyvfm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wndibzra.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mlzwnncl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ukmlkvms.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wkvxxzsh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jaophrcu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cuazlslv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mltbgrdr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eestwjsy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zhdsnhun.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ymhyzoxz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zmaqgbkf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rhwxfkbf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nfbkejow.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mpbwhmaq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3htjpxjmb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3easaxgsx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ewweufcv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dxvlkpip.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3aebpccba.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3gzmnyiij.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vbdybqga.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xgdhpxmv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3grbnytbg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bzqtcuro.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ndjqxhra.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kddwozyq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3pugxpqsd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gmwjnbxx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qnqzizlv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ntiwmrak.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ubayxkta.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3alkvcuhk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uoudcmiv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3iufjszee.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3bbzvrhua.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3knmnhuwd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ldqqkmor.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gluexufd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gbvwsmxv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qehccfsq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zvaibvvg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pmfteern.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3kzdqkesr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gafwpkmd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ldaogufj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3aohitvxc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vmpnohvs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3uxxopwhg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fahycgfh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nnrbezsv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3btlkwcha.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kneygmaj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mreyutap.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uuiifexg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vscupuxg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mchwrwhc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hvaqvnih.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nxfjpign.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dpqonrbj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fmbgcfqb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vgtgjrsm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wykuytpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqchybwf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kctnrsro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mntuvtfg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3edwjcbff.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3udjcqyjv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ksjhuikw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxpwzqg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nlvvlfhy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzyzomjs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtfrvzbc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3fvmhsphw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vlgvtmfc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3skhdsxne.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wwqliqzi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cewbqtzb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3odobajxg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qbyedvvo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3hcbhdanq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3sshjnoun.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aztoywcu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kdatdcsa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3vocctyoh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hrorpqfc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3usunjvhx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3yxhjibdu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ywhvqdko.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dfienjqe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rzlftxxz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hbrbgxrd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gxnvccqr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nhwyjkxz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oaoauyco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3aknsqjud.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yfeyyimn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sgguqmvq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3xbhajejz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iuccbevp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvbmjmj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ckberowp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3puholaes.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvfhedwd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3oetnvdmp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nczeibnr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3imzlkhzw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3nmuuolpf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qktdbmbo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3czkncvua.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3miwnvqpt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npatzfgz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lhckflsj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjtwbwwc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3paemlonn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zsllxmry.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ocnuqfkm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rhvpeqmc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mawhpuhu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3evvhvriu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pbfnoxff.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ivfckgna.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dpprumse.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vasjlqcn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jfrjowhh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cxinrsmx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xlsisuwb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tnanouex.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mvqblyeb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gzmovivi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rsiwbqxu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zyoxhtqg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kmdymrbk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ramofbhw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wneygksj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vpmnnjkw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vdlnjedt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bbhpqrvv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ivvqfmqh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hvhdpqvc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ghbekvcj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjpjbusz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zfcdekqd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dqnlhkjc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ffrpqckc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gvivytke.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3clzvsjay.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3gatdpbeu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3hplagjzu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3elhjujfy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jatkvfeq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3lyijhjoe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aampmzne.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3bzbsugtc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3arkwgjfy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xogjidhj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dgrwdnqw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rczzbomw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3lhnejqeh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3oskusrnk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fiqvtead.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wiyulcav.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3goqywnfu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3iyedljtj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fkulyafr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3kneqexqd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rpfxnvko.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3eaunzxgs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hvwndngs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hrywvkfn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3owoeuhgp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3yuwlomlt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3todmfrnd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qxyaynix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljnzfygu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3deolcmkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjlxwdwa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3qgddoahb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pwdmmgwy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3jwtsrkat.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3qmqmkyoq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3phfxzwgq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3dwalkmzq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3txifshbk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jugngqxn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3qimdxmvb.html


<!-- 参考信息 -->