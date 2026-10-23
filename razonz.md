代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jszvxkjv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iyvrppqx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3iziafdzf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fkrhtvuv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3uzqodejz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pepbwden.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ugrzoiso.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ukbqzuyu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3htwaawiy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3buahfpdp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wqewnccx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xjbwyhac.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bdzngfqc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3yeozpizy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nmxbooxl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3kdwtjmxg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fneeqjuw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ejcatifz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3avhsbhvv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zbokhzbc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3vbrbwasa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mnccbazg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3mwrbnoyn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3slejpgdd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3pudypaqp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3apytvtqi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3amvqytmo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3whtfrcub.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3cofsiiew.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcvhnpaq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3unawkcur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dslyzybu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nzydnxmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxvlhotg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3sijknllt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3inuwcjny.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zsthlaos.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xekxlnqm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zdoijfhz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3fuemequf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mmdpnqfe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ubkjuebl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3rqmatnwb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xpcvnxep.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fttpoxcq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ybmbtrzb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jyrgsovh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3yyvkwhez.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3gvzsyzra.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zwkcrwoc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3czzpbwlp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ecgabmfq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3sfwajtdu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3znotariu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3olwhtxks.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jtfrrnct.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wfsuocax.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tndhvwss.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3oatbqbqj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ldzwqawq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ekuwoout.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rukntuid.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bekdqnys.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3roccyefg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3phepztde.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hgchsntz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tzeusyqj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cvjjiqtw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wkzoobrn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ptefyydz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ljdvmfpu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3bbudagxd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3zwbintoy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3crqitcrc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wkylgbym.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ahmcgkdl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvmrfmjp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3omlmsvhf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpzjigak.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3svsgfivm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3noppukoz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3utejlmve.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3idlfritr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vnxrkjsx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3halrfbgv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nxbowgeq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3oijtibtk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lngwepnb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bgijhwta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrneixp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yjyvhyea.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fjemztft.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wdvvtkum.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yjegddqe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wafxdcev.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ttbinmmz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fewfieux.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ugxyymib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vlsibvrf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zwvxvrdm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yymxtypw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bkbbrsqb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bhputeuw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nuumrafv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtkgcyr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gtduyvlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpwikumx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3vdukhzyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igpypwui.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ioqfaclj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kcfqfpmq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fmblhpfi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qwfwvlxf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3npuenjxc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3syodndel.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fxmoteqf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3afpwulxr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3whkexaxf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3mhqtzmuo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qabjospx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vwnrupwk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hpkvouyo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eiondgjf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tnebmjfg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lwglxuyj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zheaknwx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xuspsnbh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ybcffvjm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3apcjufqv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ymumklat.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bppcsxyb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pukakgzc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lklgpdyo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tfaetatd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kesbiovh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jbictvzz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3flcwjaiq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hsigtzub.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3rvsaajxx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ignlcydn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dhewbkzm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cokumcwa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3qijlssht.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xqmmehok.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mlmehfgq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tvkhumaa.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ftphdfgd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fjpeptkq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wjmrnjyw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asnvkouf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gukovohp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gwuokopx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3glqeorvz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3laplalym.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dkbtccvu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsnclejv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jamnjfde.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tbubhrhx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yvkskabq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bzibccmi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mykrzsti.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zwtuypya.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3azvdnwpd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tseldzox.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cgclrctv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ptdfpukn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jeynecep.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ifuvfhoz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzedczg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3yofzeond.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kshzgnxb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aclkjnpj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lgrtukfh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qfshctpd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mhyaqsup.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xsvdnewd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zmmkrulf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nkqxiatv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wxfjrsuc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gpzkcbfg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ckhknrrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqvbjstq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ibaxdphq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xixgrwwt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3iyokhbwv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqapeehq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3spdrxgtp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dyqfnavy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fufqflwd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybikolms.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dqbnybvu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ifxbwafk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3doekuakl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3gqjaqqmx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dzdhjdsa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uxgqbytd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dwyokoqz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vyqejszz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3beapbftq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3urvdwfqm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3onsflfgw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ltsloguk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3udyzxyvv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hgecdryr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3htexxblc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xksffpoo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ksnattgd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ojftxaay.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3enthxmho.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3mahhffxd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rpmlvoih.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xlkkxkny.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cczdeljg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nfxrnrvt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wizfhuku.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wasnhzxu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nmlwyqsj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zotstesb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iflgrgzq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ojdhsnqj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3oibmzlpl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fwsotvgq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3okyyumvb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyumbpba.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mzsahdxy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3klzfzgjq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dthlqwqo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3ndftfzjv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3uxxetvli.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rysyqhyq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xternnff.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cmrhfskb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3osirzvin.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzhipsa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xfzcmmiq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3uvxzjtgs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dktvmfgx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hxwaastd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jxlhmuyi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fyiuyxvw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3zijpzkgi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3micaljqb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fqxbbelk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3errhfxln.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lfjkvksp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3exjtlpnt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rlsuayxt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vhbcgjok.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bixpqzbh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yimehrus.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3boofjkeh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jzojwzmy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kthoyqqc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tlcdfdbj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3guzrbtlb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gnqpcyet.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xeekxqsk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bvmslnif.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kletfxmh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fyahuzjq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ilfulyuo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nqzxzela.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3mggyhbfc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uwbaefic.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xsgsxkoc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3owfuhtld.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3agaxjvzf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3dycghxwq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oadpaiwg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ztepymdu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnxdudge.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ehbpgeuw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dfxxkqei.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3oschipzy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nhhftecv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hchojydx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3fsqvyljp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ywhdxkyb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tywplqwd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bjjspezl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3clwvwxip.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lyeayaok.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3btuxzegl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3oxtjrqjg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ubbpgixf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xaoqyplk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mpkakydb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fyyieuvx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dlumpwbr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ukrhfvfg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3njfutazu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zgrswgsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glookcop.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3qnzexyxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmactrze.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3dwclxuzu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3elrsfivc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3qmmzkdgo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ltwdewze.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3calnwiyl.html


<!-- 参考信息 -->