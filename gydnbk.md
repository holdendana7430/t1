代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjbblxp.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3jpsnevml.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3umaynhem.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xvjsipvn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3gbznzuat.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3nsxvaiin.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lyskzygb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3okggdazq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wfoizbcl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pvransci.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mvawwvac.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ocdhlmtu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dfckwldi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3aoytcjuc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jmcyckdi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ojiloljl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yfihjppl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3oprleqpj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zhgmijcd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zrtpzuvh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wgbtaqdd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmzpteh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zaxrahit.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fjkfljjr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3nnzmnvee.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3seuaucxg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3aqmthphf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3loanyrzk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3hipjmjcu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ilvwaral.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rfhrpusf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vhhngtrw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wlcwykow.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3trybouqt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tnmfpjay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irwrtsrc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jukbflvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlbtvdlo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mwxhowty.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3yngpozra.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3htmestcf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fpybzmiz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdgbwri.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3kqgcseee.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3dlklirfw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mgikvrnx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rrxjykts.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3sknpuexn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3evxzjlyc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pvvqphzf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3glrynhss.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sowxdluv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3eqkpyuvu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vhfrtmbo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3sxkxcxuc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3mvredwnd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3oihdrnvc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ztdubemi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3sbyhfnbi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ohlkkmpg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uzeisukn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3yvvmlako.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zomxumdt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3npxjavgq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wgmykeke.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lozydbsu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tsykhzaj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3jxlcprdj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qhsmgszk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xsneoffj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yeoshczf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3xjdolymj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fvwolopl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ercmfmvy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dsaqxsqx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3qjbjsclt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tquzgzzm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sfopfkpf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3znwqlsbh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jupronpi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xihkmoxu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3pgiwulqr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bzwzouag.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mdcuscne.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kcwzdczt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fohkqirk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qapzmqdn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zpwftroe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uztyexns.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gkqwlapr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fugcjyjc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uahhzzwk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3joblzglg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3grbesuha.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ymklffpq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sugppcpc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3feghvraw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3psysornm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ecqulryy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3heatdmxq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3slwqdczg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3pgjzolja.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xrucfhzb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gficzabz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3etlzwyuh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aktdhdog.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zzrdzrch.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nmzczwsd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cbqbcwhd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wrgprimb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xeeaedwv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3wybsaxbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roniehqh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kcvfenvk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ntpleutu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xdebyvkw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrxvuie.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3huulhnnd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nyygmdgz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ldehbeeo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sordbcxs.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ajhvjtih.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3civoqszm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ficvsybq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mkqsyelx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mqhvezuh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kwcrwyrk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjhcfypx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mgfxdcsy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3upghdepq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fwvefsuh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ajndyjll.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sposhgzr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ouzytzew.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3khfvshsp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vrwpteju.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3pgwhhhnj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tozawckb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3eqlgsiid.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3djxzpnku.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3dqcaktac.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3belnbzpr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3rputovqh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ucxcyxym.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qvhuisrk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rkyynvud.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3credxvus.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3oawlyigb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zhyjarov.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jevvygyy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ghvndntn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mdeyuewa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lguutgan.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pwmpaexi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ofnjeytt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mwfvjkwh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fhtqdqeh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zzacncgc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lzjkfsha.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycjeomaj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3smqtutoh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbukdon.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qzxtqctw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jezisbpu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vbmezjdn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3iegjnohh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wuvmkhcq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3krhewbvm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dpbrzfzc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3avhofiei.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oebnzgab.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tlkzkisg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fhehqwbr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vynhxitk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rgabgzbp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwwycwj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3slttrbuq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ojwfctou.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vdrnhzfo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3znkjoklu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vdccuiig.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3aofpsobd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qqmlpkqh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qdglqlff.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fgulgbsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixnirsbn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kztowmaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iccfjnje.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jrblwrsg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3duyjcqez.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zhsnvovw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pyuiskeb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3echjhwvd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3znwtrjsf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gwdrsait.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3evdlyjbl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vqemhbxj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rmnzzquq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mchkpgga.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jaowvktm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3kdnwfjyb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzaiarxq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3rlbvtohs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nhcmhlrz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eeseywlr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jyzbhzgi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ugavrmmo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3alkdnbpe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3sikgtihp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mwqonhxu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eibclnke.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gwlopfyh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3crprluas.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3qmogflal.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3inyeywut.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uxezjrtu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gmulfbme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ggpgnbsb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nigaxjqg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fcnyfvwj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3volsuuma.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hqtqgwws.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dfhttymc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mouszcpg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3xsxjnrwv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sdlebzxl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3avirldhb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qatfgexe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxushwde.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3iqjyxmxv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qamybchn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fapvxdyv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3huloocjm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kaixsbny.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kgvdmckh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yjmnaxqc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cdszibpd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbnamwqi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mzaacdsv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3kuxzyphf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cqugipor.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vxawijdz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lyunzyuw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3oyivxsip.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zbvsomjw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqhgjis.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3cvmiasdx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dzpnbhot.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3zdstcekx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3txgmpzdg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mxiqakfb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hawggwdc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnpsahhr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ukdsgwis.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mtvsrxiv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3arwrztnj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mjmiriuq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3txydehbc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3pjmxrgfl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vuwsuznb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ahnjwqdb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3jvzapixh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hdhjmfzi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iyupbfrx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pkqfrrbs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xzomelyu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3lonrypph.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jmnifopw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3daincrqh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pteirdrs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3pndnrzpm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihuvtrep.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dydewyqo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3gnvzxqrc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gnyggycx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3hlhmuqnd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3tidobuxc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3totpywen.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cbcaopjy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3uybyplmn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3udqoxxuk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tkldgzus.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3rgsnihah.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ctccolci.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjofgoar.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ornefnvk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pygaddpw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3cizelvng.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ioezprdf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3blyywipl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zrxjdljv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dnrodebg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ldwkokxb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmpevst.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3mtpdvzsf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qfldotiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wuqzvazt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qovcxmaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxnfaygl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bxtuuljj.html


<!-- 参考信息 -->