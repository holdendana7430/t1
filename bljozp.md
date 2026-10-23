代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3dsprssil.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ytasesfw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rzvsxkwv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bxjgklwh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pnyvqoiv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3vdbmrkmj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ltrqnama.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ditvjevk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jhxnnghk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ygqpfwnp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3smntwvbl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3drrdavqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fsjxpsoz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vskhevht.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3igmnewxp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzhjzac.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3icflfipm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jqohtyai.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3msrhydgq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3mujdjqro.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3umzxbilo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ndazkxop.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jacjkvek.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3dxvaeahw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3rnaabici.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbrxthw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gsatkaml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcfjgmfs.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3veaskfhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yoleqvef.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pbiohsnk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kfmcdgoa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3heucbemi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kjtiiyov.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zdultffb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3qppkxwop.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wpsudnug.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dqweqows.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vpguzxup.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mngueuyw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yivrwzib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hklgbosh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3naaeokcu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wmuhwnmh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3giqyiypd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yxvotgjv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3tbntltjv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mstnhdko.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3loftazuo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3frdstvqc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3qecqbmva.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3erjggigr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3izjbvubh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hrrybssm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3lkvwctyb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gqqumriv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aawpkfaw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3fkezwmuv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3eoiebqyj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hzwlabzj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3imlqzajk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hpuatscu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ntfhupcv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lmlqawyp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3fdgvqkkv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vtoulfhq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qfbwvmls.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3aulwykyc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3gtxfdtvw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nvntpctu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qgvjvjgt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wodfrsip.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dgkdxnad.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3abpjlmxq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aceadvrr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rqqphsvz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qhqmnzxn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rnwwiydg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ktuybnxm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mvllsddn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zjhkctlm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3xmndiaec.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjnyshy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wfaeiget.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kmrktmhg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wqkpovdu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rimspold.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tdbdtwgb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vogmtone.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3utljqdoq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3deyqsazv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fvbsusvs.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iscicaxc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3afbskory.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xwoxnkuh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bwzvwbgg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uafhpnmb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nhwnkggc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jiwfxeiv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3epeblhqp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3urwurwsd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jzppngfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvmrcnuq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3hnwesdua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcwzjzee.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xsufiwor.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qoauktvo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3niiwbfwe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gexflmkt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cwhqqvzz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zibyrstf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aheenzvm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3rptqthwt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xwqqcocx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rufzwlpz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3txdbpzan.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3esnxodyt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kqoyvlsw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pqgvfkqz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ewumenhc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qgfnmzay.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mnqviddp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ftflehbd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ehfidejt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3wgjdtlsk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ibgctska.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dyitnamz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3szhvpadg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3szybyfzl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3gjylatkv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fjjitmuc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3lnaijnaa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hzsaebyl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nzucfcku.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rwtsyeuo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iffyspir.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fuqouico.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jrymhoiw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ecmdnbwi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mfypnxho.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3unxlaupf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3zvycwmyn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ddosywjc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kjqhnpnz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnhinoml.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzkknaa.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjqlqaaw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfyzvvod.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zrfyocab.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vgyqigmn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ityhlanj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fdljzwds.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3loqkqksq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kamcdqxf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3isvovysm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ztnhzlqs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zorxumsf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gcgqcfwn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3edauygqv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dpeljntb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3osgnhdpk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uolzfsrk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xvwowzog.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3luifsqbq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlhknaj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3trazngbd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3abrggoku.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ryjbvzsa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qwplubed.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3cgbspctq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wvrwntez.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3alibqmdv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nbjmmgvr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wxfgflcz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qrkhggbd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sljkjpmu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ibeowigx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esvlnysq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3yjptvzbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyvcbsso.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ckcjvywv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tnzizyla.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dlvgumlq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3omnwxmtb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dpjdokco.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3whnqqdhy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3patwurrv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3acrveedm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hynfewfv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3htanglfj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ovjkftal.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jfjbenfc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3azpcqnaq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zabgtoga.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3olkqtcbp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vobvocwm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ohxqboxr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mlvydfcs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xlxdniqb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3skxcjoqj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3gntinidf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3urwvsheo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lfdbspnb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3asihfwvl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ridffmun.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3wflirmkh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wcqnempn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3owmatbvz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3evvdplsm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3egyvavta.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cpgffiaf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bgtzahsl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuysbndq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvcdejis.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3sovqkhtw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cyxejwae.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wbdseevj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bnohpvxb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbzvypkm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqualong.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxhuqzjd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3irbhcapy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3flxoiljk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwxqauf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jmomhkjv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xjhwfrsh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3qtqovwfn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zopxslns.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3molqiqrh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ibyjtrgx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3zhbhvdej.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wsqbyspu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3oqvoktrj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3grkphlgz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zwgakfgw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xlvgjxiv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mjsmkcwr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3usbxogxy.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3neanqnlb.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3auceqjee.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xsoyhzhz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3txbjifbf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ouxnjqsi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ehwkjdwe.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ryhxnucn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jbqfdmfw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xesrrykv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hwlurygk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pgrirtsk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xmfvaohj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3smdkqtal.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dilhatkk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3txzqcvhj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mamqnryn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rzesgpcf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ycabcilg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3apcvudau.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fodwhoii.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3brkmfxez.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bjtiqutx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3earhawoq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3icwesyuz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3onzgszkv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpkplbxg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rpuhzzwf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tqddkghy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3utlxngkt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qslewscu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3stwsagic.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yswbbrau.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ikhaqxup.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vbdjjbcw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3jrqqimlh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rvbyewwj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tvfuvctb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bnklwocw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pgqujqkb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3elsihnlc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iovmyutp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3qulonpsj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ummlckqj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gukyygqo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fkelpoex.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ievspkuk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ghbuozip.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3yrjnxosu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dpnfhefh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zvdathbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkijftwg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bajryjpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brpbfmid.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3oxxezsos.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rtyozzvr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3aexuhopg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dlhqwuah.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3huhdjwpf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qzbltotx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3utbmznip.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3rzunietq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3zdvklcsg.html


<!-- 参考信息 -->