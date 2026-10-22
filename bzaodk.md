代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lzkmmlzl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2thmybzbm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cpzitpxz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fklwaatn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2huvhqnzl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2lzssvppu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2axndztcb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2akslpaci.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctlvchcc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yajqnsew.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qtfbcbyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2frbpymcy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gqvxfaab.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rqiorzjb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2axawmrwl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prquymsz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qvjzbqwg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gnqpffsy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2exzfbfgt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2spylsrlg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rlxtlxpz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdpaktqt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rmqdvmnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqgvsgmr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ftkafowx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhzymtug.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2gouucwyr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2boketyey.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2fanoaqww.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2alqwsopm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2frcporbo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2enmtkeji.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zdzpwlut.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2wqukzxaq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jdivjqcq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hoakkdkv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yjrnyndi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ulzejjas.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2boseldro.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rhlznvoy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zloadtix.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2prfwdigo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cwydmdgo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tptpwxvf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2wyivykdm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2uyalevqu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2dgclcfcr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hpjdwkul.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2oeorodqt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kunswggu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2efvftvnb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gfiifppd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2liuowjme.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hywwaaei.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wqbxgsiw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zftiesvt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ybkcfhne.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vwibieyy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zfsrwdgp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bjvuczer.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2thitekoo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hjibbolr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2sbhywtve.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wkduwdhd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wjvciioe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zykhmepl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2duxgtffu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2anjmddjd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rpputalp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2qxmhbpeg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbbjogrh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2duzdxaia.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ggvyxlfz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2veqeggtj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2flvqrpaj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2roryukjt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qixhtdqc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2huxvzaic.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2srnnvyro.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cvcakhof.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2opzbqvos.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2golgjmvx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jwljlxth.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2irtylelg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vlpasqhe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2udnkikso.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rhtopofq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vrojiqdc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ucdekizi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2noxaiiqd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2sdvdfwqa.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2oissdfvs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rmkexyfj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gpskhomk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2srwlikxx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xgzcxdwl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2paocarul.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wkqpipjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcwxlrwx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2asntzuvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsgxnefz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yqprobgg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rvqytmgr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wgaryazy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtlkgmz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtizddcy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bnafqmqa.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lunauvbm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mjrkmywq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2reectnmd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfafttmw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gwrmzaik.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xvjamwoa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2kovfvoke.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xqrugjai.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ndgrlyjy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vgoxnsqw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2epfqiysr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tymowskv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2eninuzim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2glfmitpg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ncpelqmo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gajmrmoi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zlzhbasg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lvewlkyl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2syaohhym.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cutyvlzy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ethygsgq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zfazqhxx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jmwljers.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sergvvhh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxjllxsx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pxadwqha.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ptugiuwz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2socysgdy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tbychlzr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xyhwttns.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2achlxomw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tgrqdjtd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gybxsovg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nclhvzdq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvqojah.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tqehgboy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lcytkmhf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2puhlxeby.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hwhysjop.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kvctuahh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gwvdlgbq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2noqnjmny.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uekimfhc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2omnbfnnd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vhzezkhr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hpvjwcrf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2axewhvgg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qsmrvcne.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pkflqvgj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lsbzzikq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dqcgkxfh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xjyqpxgm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2pabeeccj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xyqpjhke.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wwllansi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nkiqowzg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2filzihbq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ljqqyruz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bxkzcxbw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ikuumibg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2addomoqd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vjzdqdbj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mcqtgosr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vcgllruv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nsgavlew.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zkimufaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isoigtkr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qpdptjnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iavrsdwc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mkydyfdg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zigdcbfj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gdhygdvv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uzqbasru.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2grecagoa.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qdyrxmob.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2guutpaev.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2livekvqp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2etruyqxy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rxfnzqgg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vburjlqo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jzpzbakw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hppmgkqv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2koyxggnv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vypwaagb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aibpdgao.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lufdmjjz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fgnkfysr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2igmfqlrd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bkzsjebb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhuwkm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ouhclzlp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wfjgcoar.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dzoethrb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qhdzdzzn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2tlvlwkgh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2uniwvqjl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2esqiyuxl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fnajrqdd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2igrenxgg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pslfrtmu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cichduqc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ivpghtys.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2chrqmqbk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckpptsrn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uztuljwy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2coyusyad.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gnidnuum.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qgmvxitc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdweptzc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bzholria.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2oekehuwi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gmudjizv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bodzuitk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tynofjzz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rlhsvctr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vhxiacfm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mxkylshw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hlrblkhi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqounco.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xeprwlbw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hmxdpmrv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iiabjgfh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2bhfulerw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2avvcttcb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bzkhlzbo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2joykjsdt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gyhxqpkw.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qeuhynth.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2snxtqcde.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vkvromfk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ygtqvfao.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qafcatvh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ybcauhbg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2abwdggzu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kuydnskw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hpqavhsx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2psjmbfip.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vwpcceqo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xpqkpoio.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2snrtdesl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iyomrcdg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2orjfdoyp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yxzwxdhu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qgulzwem.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xtdxxbwm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fvqikbxv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dqmwefst.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gyfwmouh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2fjgtyzog.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jursihkq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2cbzckcoa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2duzlmghn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ayhtgzuv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oojjadtl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ynezdptx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2bpimxekq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nihpqaql.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wpcbptru.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2amvkxmas.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zgbyfdhz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hsxsgwni.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wrddyvbt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pxrywhvz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fvpdanpu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rqirhrzk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gtedjpuw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2njjbnewo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cdriidel.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cfhqtunw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tnfelhxo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2hsraqeni.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ekoeczre.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2inzzkoaq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2eofmwnki.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2btbnwbpf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yksvweai.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jksgutgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwgqldnl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sgxrovvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmvislgi.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pqiuplgp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2igfdxsvp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lisiocea.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hjdstxmc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2muisrpkj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2oetyvmvq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bssjfepy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wswtdqrf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2axqwvgqn.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mjabggbq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gtzlzpdd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ymvnieib.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fisvkoas.html


<!-- 参考信息 -->