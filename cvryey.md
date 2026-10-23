代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ymrihpad.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hmuhnwqs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jikuvvrc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3epmeufaz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wvbuylqm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hbawxktx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tiuxiqax.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3udjfodaw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pjmxgviq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ztlnveti.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vrkdnagb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3oxdhgtza.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3foglgrvy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3lsoxcpcx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3taugcqzc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3tpqgcapq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhnxnxq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nzkylgiu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mzgzfmts.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lrliaowr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3mupqfwzt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tkocsiia.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3iaeuwzeq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtyvytw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ujdeocre.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kwcodrtk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mqdhaucf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3vjnqpcxx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3zkixvpst.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdcazsg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3iwfszjjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xufdwngc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3dmweeedh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odiqjoex.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3bqgtxkgd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3adgyuhdc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ykfjwdjh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cgtmsatg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ptholnip.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lpbcvzlu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pihzyeyh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3xflixtjq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ciphnyug.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3yunwxlsb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ngbfztnj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3peexzltj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nrohnsrl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sbkzjpdo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kutqfkyf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zxvhahdt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3mqugrxqp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kvuvwecs.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3byisxzql.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3arammbcq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xdnmrnef.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gfnrgfml.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pnqcrkmm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jazuwizo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fsulxoxx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3scpuvfxx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mrstfdgm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zvotviqd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wtomygil.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wlueinnm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3crxwicyc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qiicnlgl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3giowgmlq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bysmbqgz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3eopgdddl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nnusgmmg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zinmjpec.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3yoelzfhd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zyyghxds.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3urqwlvfk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hnoxbzta.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iuayebqy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zcgfmmsr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3yainytku.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pfnuegau.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xzizucny.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3acozogwh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mgfwlgpj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fnlkcivu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pguoihgu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qnfuocqt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3srmzvxhm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qjbttrbz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bgpcbjad.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3txreshih.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rqnngfyu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ohygzrtg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wgsnlekb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sxutnuoq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lvkpyatn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wfijlqyw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zoknfpzz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ksvtsyfr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pxhqjzri.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jxjxceeu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qitduvxh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fjjfcqae.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xcrxqynf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wsccnybb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qghrwagu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wprlowza.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eoqlytgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dimkwmgk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vvjcujrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idzqdswz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlpodwgm.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pnsuuoxj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ymnwfufm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbybcsaw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qaacaoto.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nemdxigg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lgqethta.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3buanugnt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3krkpnfqu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mxsufixb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wfspmkvb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qjccflkh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vigipfju.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nuusdlma.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fqjvcuzd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tmtchrry.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jmhymjaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rwngkxej.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3neofrxin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jfdwndej.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3wunwuxin.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3plsdacix.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkiaocni.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fbvxulax.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qzoiegzj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3iizynclq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3cdhywtrx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3cfpupdyg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3adanezsm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wdesoarq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vosaajqr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3inwcxddz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cctipias.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sqqoewzw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jgiutbtj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3oprjbxtr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ulpndkat.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rioqcmhi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3swhsyhke.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ggkfpeig.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tsihlxvs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pnekqsdq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uqfsyxje.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iagjxlhv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vdvpaggl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3iolfsiap.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tiugwdlv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bvpuhdwd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bhybqyrm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mseenujn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sdmcctrx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vfjhxieg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3alockvnr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ipmttwai.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gzmeosap.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yxabpcdl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xbqzvita.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bpabqgfz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3scihongi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ihujjoqt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3tmluuucf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jyfqigxv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gqbyckrn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qmspynfj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ljiyfmok.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qxlykedq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jdqchytk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3opfbhdjm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3voolkkit.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mpnogubb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jwiagtrj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3qexkktsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilmkrdnf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3uqdciugt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txyrkwrt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lkxrejyp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sgicseod.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ybohtvyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qerborzk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eyemjpqe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3afgqrfzg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ldpobtan.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ijekcxcm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dgqzkshd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3eanpaleu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oclrckdm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3lcxoknmf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fbvjwmpl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jljdroxr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvxoxbc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3thclzlxd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mkmxqhrb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pqxtmwwb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xundiejt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3goyainsi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3lzkzgmru.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ekgwjcgq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lnzsyhpt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cofmocns.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3csncfiob.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pypzgkbc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3eyvhugsi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3plhgfrxe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hkfkfyif.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckkbqshg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hfmidkrm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3obnelidx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ijikkvsf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3hlwkohnq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hfgpbjzc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ckuancou.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zxtkffsv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3winpydqm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3natttaox.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3siyskjqx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqlmzfsy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3sfixxphp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gajtbskq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3otwnhoxl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvlybqdm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ztumcohu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jxviwbwi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3hblrvlvi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vgdoywkl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hmahufzk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ortfuxlh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uiogsvgq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3caaczusx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pxtjxmbm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3nwidoagc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3hneerbba.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zbacwgve.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xkzbmeyh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3hzsmyayx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cdsigxnd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3eajvrarb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qkpzhltg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3gxclbcjh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ultruzmy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3alfjxuut.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mioqflun.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bdjtylbg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kcavtlrt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fnjkzbbo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvnwmead.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iqqqpmdb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yyoxghkf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yxgtacmy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zfyptdli.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sbgcruae.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3csbyzblj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3wltfsdwf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gwpzqtoo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wixvjaih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uogskyxu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3oltnjtnl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3khqetqhl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3cscvksyu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydijomtg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3plzjlsbm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vrstjkxs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqdcvivh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xpqgbill.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ufoegpuz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dtzeynch.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdyobwwu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3sjwzfyzl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqzwwbed.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hpqrrtzb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tqwoyfka.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ecoonrzo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ljfqcxhb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bvveiqny.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3oawywacr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3mnbmuuyv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dgqqtloe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3phzmbafn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jxczbqfw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3tswagzqv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3drdmgewc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3fwrdrqpt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uevgqoms.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3eanlsasj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxcgaarf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3rplqzcmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkwondvx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3omnjiyoi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jopogxab.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3nqiwefns.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ieskhsst.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rxtstagq.html


<!-- 参考信息 -->