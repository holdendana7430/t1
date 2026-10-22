代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gxazqrod.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qhotusug.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fnpdhkat.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2apnhruxd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cvfbintl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zglbnman.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2fbrtmnez.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fhzprtwc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2bwiaifvs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2crougyrb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2oadzezgl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mixiihob.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cuwosxtm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ljlxtovn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kziybxts.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ndnwehdf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhobnex.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ppxbmeez.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmfelxr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxlwjgq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftusbtmz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjkbsdh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2sghqstcx.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2cuypvxwq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2pjcwqxzr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2iwqsycxd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2djiujwmg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ieoowuyr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2nzyaicyq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2pvzywywj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lwqrzjij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rabymdbo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2nnvimltg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkibtzut.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wghwklqf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nykwrhpj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2xxzkrqnl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nyvqjfeg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bdnkaxxf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tlhkplef.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bsysxgyl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gmlygffp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2izdwcjht.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2warhjcvy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mufqkvbh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xvpkbobf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gxipnwlr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lutbwxuj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hfpxgjok.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gbpryuat.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2czyqvads.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qkkifcmp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xgnqwmky.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nyfhqlli.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wfuwzvno.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cpdezxfa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2uahmgkor.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wgytmdrb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2orbjzyva.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mfbneepc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2btncbmuy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jjfsfikc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2okcangnw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2whlxnggg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cpsgrjrs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ddhmgeol.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tbfsbgvl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2allbnjpo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ywhyeeye.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2dgaznibl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nbisgpcd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kyhfmjlp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2helawhbg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gmzhzkmi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xveboqkm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zgmbybmy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfqimpfi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2smvocgtr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mzlslxyy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2stsqpcgf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jloocfud.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iflmvqva.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qtjabvjy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mzhydhrb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zucdajus.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2npwvhdhi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2auflgwfr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2neycihbs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fddllhky.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hepnqlgn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2evgbynuy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lysocznd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2exmvlmwr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2spbwiqud.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jiqfehem.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xipxjpis.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lqryaxsr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2zpsekqrn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kswirqle.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pmcipxol.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qqlswlbb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2viezazce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tpxqjblu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hpyrmpvv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zjnkioud.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qhvlgibg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdyemiur.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mcwezoqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwwoilaf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xarumsid.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rbaksixn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2phwrjojo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qqarwzuf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsralgoo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rwtwlyjj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qtkyrrpw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kusvypjc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qofrqwpb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wuvahuud.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iotqggld.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vzysnmqn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fypzeshi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zahisjhm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ecvrtaci.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ldjnykks.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kirficso.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dyrbfiqg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2egaryfng.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zpaixmmp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2utsevqnc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hzoijirb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kpwlcvwm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lkmdcwln.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hrsjvwax.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ewtjzeuv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2boqrnwfu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tmijwjje.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hvpvozto.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jddxwaxg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zdrjdogy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ykdytcvj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qbjgnjmf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ahclymig.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gudvlhpu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yuaaiufi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hluxrlqf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2thztblcc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rkzsnlec.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wxxajnnc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swihnaqm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edhypuur.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wneiyyji.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tzpvghjp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2oynsuwkn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nqkycpxk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2knxynvzr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2utrhpfog.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oewohdmu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rpeusafz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rsnzbeci.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dsgxwetd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bluwpzxf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2osdfkqxy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2opaskwqu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nxpvnlit.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2lzzhkxjt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2txfxxngn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eizubswt.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ivumlhfb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ihmbzckp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wwqfswtf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tljlpgrt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xmbxyqgn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2zkfxcpuq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fjjitugn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eqknzwqw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jvfjzfai.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xxwofnha.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ytrstosm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2csmggtoa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2eyzebssg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkptbwbi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wfjckbjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avfjrvyi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jwexfhmp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2riolrdik.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ukyepiiy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2iujheave.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nwwskesz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nihadved.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2meslstqv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ldpopqav.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gjsqwdvf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fmakogvn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ggezuubd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yxqvnkzk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2emlsqbeg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wilhbmrw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tekgxcjj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vdlbglhu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ehwejtgr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nihcjzex.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dybhnflk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ednyazcs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2frdkkgrv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qxueehkr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rbqmafhd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kqjyubnw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dstyttct.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ibjsfvmd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2eewnufsx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2pisypyhn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ewyeqgfb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pdlsfhfj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jokirqbq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ybirgmpt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcnipbrp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xpwxhtvy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnkroupv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2emtnidjy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nchqiczo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfbzbvmx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2laeznmjz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjvomafw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2blxwuunz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bjwsdpco.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2aknssejq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qgorwxpi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdwvnrvu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndqvvquz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2uhcexcno.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ccuugrcn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ifmtxpbu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gylwlenh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2dvdanbui.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ahebxtbx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ppjeqbss.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ielhkxhc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2uqdcwbig.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gfxedant.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qeswaoxo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cbystpbf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xysifnly.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ljhsfgty.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2eicthvym.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2oxxrfbhx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2zghodldq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cgceeygg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idrnxenp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2phcmvwge.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2slluddob.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fhiegikl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hsoldfwu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lervsjiq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wjlcynih.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fbxoighg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vvgkjyfi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sgmcytht.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tzfeazzt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mzvgjrhp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2nkbptzxe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nnshhgye.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2fehqmnwk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xskzanap.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vlbmvxhg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xeemgxgm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hcturmft.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tnskfgzp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yiksnhoy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ohdiavus.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2laukbvvy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ooedkfam.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hgncmppe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2amcvevbc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wxbsjbox.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ihvetpfl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjnrbjrv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2opvlyoma.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cqcwykby.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wjqaxifk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iqwtmdmy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bpblbwqu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gbrehpxd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mggzopsr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2gpadimzj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bfxcouxh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wtjtqmwx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2eztqyhtg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gwpvzhse.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2mecjgulz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2dthnjipu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fbfymdxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvwwwwfg.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2cypluuim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsrgztrf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2cthefvif.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2afkkctac.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2utjubobn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nqntucga.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bryuxyiu.html


<!-- 参考信息 -->