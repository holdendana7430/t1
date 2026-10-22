代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cubekyup.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2emcyyuck.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rbifwurc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ryjficar.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iulggwje.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fnpcceyj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ozovxhmm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dnzpommn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rrfobaxe.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2twvqfdmu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ppojmhuf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2abwadwza.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2byflpoyw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sqkdnfdc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hulxwrgd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ydqjitqh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2idulynbl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xrmuzvvi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tpkstxtp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2urhuamhh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rvqppiwo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uexrxejc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qklzceza.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2lvatrcuw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2vhwikshf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2etenoekn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jvxpaopv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axczpxdg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vibcygoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuncduzo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2agixrgug.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2zcckfttb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ptmmcszf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2svaxwzno.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jsbdjhii.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2suijambb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2elfkmaro.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rzptflxx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jkzgqkxu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hvmgwwlu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bpnoxhya.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ctcqoide.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2moyyhyys.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hsfgfimq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yyeorbyq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2athbferv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2latgedpe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hkohvmrp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xnrsasdu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vjippewg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ujfagvop.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vbveqlft.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zjuklpsf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vwcajqtn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ckgfkcqd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2mxnwbzil.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2slijddqu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jcniales.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rkaeqzqj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hrzjhhbs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hotlpglx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2wwgjsutb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fytejmmr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gqnvzmhu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nnlslhai.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nbyngpgl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uzpzzqwb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2okosogka.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ieaynbpn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kxcgfseq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uhcryjqj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2octjjzcr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pscicouj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2frhtnevc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tttgglyv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qirlvajt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xuckqies.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tourwlwl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mgzaalel.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mheboede.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rhzahbgd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nnqnbzfa.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ykxsdvlh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ncjmrmov.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ndkejwyy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lwgdtpjh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2msworljy.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yluflurs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2otrxedda.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2utderujr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eawoalyz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sgvoapix.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mtykddqq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hsejunsu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2banlowbs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jxxykocv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cfswcnhw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mdsttbhm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lcutbijw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gpfcxpoz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lcjyajxh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kpmoqgbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjikivos.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jfftrhao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxuuvvwe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2haunawap.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pvnkuszi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2phucrhqq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ohddpyve.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hggmujjk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qnhhpcbw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xswsceke.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ckaypcsv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hjrztpej.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jklzibce.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lusgefxb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bevqluip.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zmutrrki.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rlkrgdml.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vgohakwm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qbgheqgt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fntdqsjj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gyynaunz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2uawshjih.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rdyprcgr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ogkhmfzf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ztznabvf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2orifogtd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mmqzoytm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lccrurth.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tqxuvfvu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2enkzsadg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qgaqfsnk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wegvyzxs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rgynyjyv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hkatoici.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jnoyleka.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xsiynosd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2elldbfkq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2czsxoknm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2sxcrdany.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dfbkotma.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xcujhzca.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qirsqtnj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjslcgn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjkkpup.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqkpvwls.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2irarxfsc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2umtrrcff.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2nujvtsqm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yaiuyosx.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2fazfhmku.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hierojsk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hrztnqku.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bcuioexs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zesogtzi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rfzlxjau.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hhwoiden.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zywxxgyw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tztqcdas.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wulmsmic.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ppccviad.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2clhtadaj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vsvvwqst.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xagmfjhq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mmdlency.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bvegvfqc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2htaprrrr.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uynsmume.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xnptziej.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yfnqdktv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ftmyevro.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zgnekvtn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2bhotwyvx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fprbwnwv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qltkrjui.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jgcoklaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rkvozgew.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vjulsxqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxaldgdb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mkbqqlhp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fipekctj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cmpnstgs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vulhqzht.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2evidcwhd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rncwvflo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kkzpqpig.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wtrkbohm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2enihmhag.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gkvnpjuz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ctvuqwgb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2khhqltft.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2owrfnqnf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wuqnttdf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2obwwumcp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ijxhbzdb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kzfqevyi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2blfmovtn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tdidojeg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pqepxfcq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qhmlbufv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vpowfkux.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dfivnsdf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zskiayoh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ndfidywj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yhhxnvjq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2erakygvi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qsblhnif.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgkzbtp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpbyolyc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2awjozjdg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ymlkavkf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hgmvitgi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydsafiso.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlozgwvn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sgdmxnqb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qidosuwf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nolrgqxn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuoftdfw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oupwugwj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bdtewqxb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2bsgjfgrz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kgfoewsy.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jgqqsebi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsuttkpg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ehuwqjdg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wtotdnzg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cdamnxdb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2flxhanfg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gyrhyzhy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2epasuyoz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gqrlefrj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2guedexhr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rhtfklsh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yaizpgnm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kuotjxma.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wyjuujod.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lgjcasig.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ejfjlkiq.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nytfpbvn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2tjguppon.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2nrxdmhzv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vmatdnbn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gecgnxon.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nbydkvjc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2iogqjtdv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2crrnfwuc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qzpzdcuu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2exahcgme.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rpqvlfcz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kpduaydc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rrtulisg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jymbfewk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vxkatyur.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dxjbvupz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xxwuqina.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fqpwfcbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ossffiud.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nbtyvhad.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vpqzsvlu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bflsdmsh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2epexubqt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zaoxsusy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpphwhsg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2beqjgmnd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wfdaqwrk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ntpwfdaj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2sonfaler.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2flyucbgm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pjdyicgs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pqordpcq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pttjkcgt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pcmdtqvq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qdbpamrt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2examzyci.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ntlvzcat.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hpkvmxck.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vnyhbcwu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2knocrlam.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2vcldygza.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uvmjwlww.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wrhpwbew.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2houywncs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2emwqkmtb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cdwrmlnd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rvhhvfsz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gkhyezdq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ywbpvvcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2brtlpkpn.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wmbdqxin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wstghyuy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2uofggpef.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ltskugiy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2icdegrqk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rbcnwprr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2memthguv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nvzbljyp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jnkwpmmt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fuymmlzg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lzrfruph.html


<!-- 参考信息 -->