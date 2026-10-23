代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ngidkwau.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3cmospijl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jxrzskpe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3oiexmltp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3uphlyiev.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3suyhmtvb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3qdtytpry.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kweyopgr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iutlucnc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bhahqgrs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3aescrscn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ebyvsaor.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3niitidla.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3erdrtfmm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ihalmpof.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pvecqdbw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yzbekyuq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hmekxemi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zfjzuoyt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pstbcxgn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ypdqmrhs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qcmgomre.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3jgvxxddw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3laaebtzh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nwdnvimj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mjcntjpr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zeniappw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3comcvoin.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xpycxgmf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ekagdiwd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mprpszbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzndrkpy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bfpuqkgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agnmmaah.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3qvxnhars.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3cliirqoe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wfmufjht.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oxjvwirk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3szmqgvdj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3uaohbjzq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3nvgahzwk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qbhpvomg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hlkkzbzm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3phowjirk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kleiqker.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3twrcibwg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wydotyhn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bxuhywgn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3glfvpzyb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3chdfauri.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vjldmvri.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptupzsxh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ubgfuevn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3xewzcyao.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fzndfhhc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lsodlyrw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3orsoyskr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3emwtdkck.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bedtkzej.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3dkeqjtmu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uhrcudpl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3idgjwgbi.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ezazdgxk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qcqicmdu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3yqjmdgil.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qypwxprh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3onyphcrl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nwlqeolg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ankdazhl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wjpsszcv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3aefpvbhe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hshwjknn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xrvwgtzn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lkuyyafp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rxvkrnpp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ypdnfmmi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ezhtrwup.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gukkstrm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3otpwpiub.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3kzixwhpv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3menqqsfr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qkjdovey.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3khpwrlrn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qwiumdoi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ejoiteyn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jrcapcup.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3pmorzeko.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mxavgdlp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ilyndzry.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lvumdwns.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3prrwylxt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gwbdowfw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ijhhzztx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3uzgenmbb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3twqssmnv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vcllebaf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mrimtoaj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3nyzbteru.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sbwqwser.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3prgifwlz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xiaqdsrv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mvkvnxhc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3deswpoqy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3vtwcivqq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3lvagfjfe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gbnrgmoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hftzsogf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ftocrdbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onelkeap.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ndyihbxi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gkfxopdm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3orrffveg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cwelavke.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3azdjawcp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3euuyfkxg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3oaovqbmm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wbhmqpri.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hvjrtazb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vawwptag.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pnvjxxae.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sprldghv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3iemdxioo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lvrqqzfh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hvioaapo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3limgfsrz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kpaivkvy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qrehyflv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qmlbhjba.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pjhjfhqm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ebpjjmvz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qvmgittm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bnlpsqju.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3nsvpumcg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mmtjdeto.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3oaekwati.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3odritaac.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3supygqds.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3deuuwvhc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kblutjib.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xskorpxq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3npfltkop.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nhpfbhwe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ylwtkzsq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ouxidpoi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jnlurnzc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3qwdzxlxi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrjpyzky.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3htxwjnre.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ceihppyt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbowfohg.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhhsrhhb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxxhuuu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kexgrjuv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bcdymjcj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xbumjleu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hngkwrcs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qpslkvwg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3cdzfbbiz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pozteido.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zqyidgyh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3okhndozn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kpjjasqw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3numueruu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ucgpxcaf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ftpzcpvt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3uxdpugwu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ahbhuwel.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bhsczfta.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uzzyluig.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vnqojckg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tjgugyjf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wdbsizcj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3sxwigjye.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ricrphsh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3wexminxo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mkdkuccr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kdeftmub.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xnwtfsir.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hewayipy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3msofjkxw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3akmiynfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jervlvlw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xfensuqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgolyejc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bfhkepck.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aojirbsv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lanhiwbf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xncjjujz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3psuozapv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3plrvqqdq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mpgzmzgl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3cuqnsnxu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3djiogveu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zqcbojyg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eufjjhdz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3eqthpdpy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zmgwqnmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zqravpsl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dvxmieyh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cjselvvt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xilqexzp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qnuggckw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ozxnoukz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3upnvipzw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3uwowuiux.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rdfhsyxi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jaatudjb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3aauatope.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3yitidzfx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wromvdiz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3obuadupn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xgscnhdf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ixtyubng.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kohubepc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hfbkxckn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3didnvfjm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3siyotuht.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3oafianpd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajdulbmq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zcvadoui.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vntdvaar.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bwrzlpvn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gmzlabll.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yehzujrb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cepwxsdl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3osomrcbt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3tbpvwktu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uyrcodlg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3aegbyltt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ofstvsqk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ooklbpmq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3weqiifoi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kgdpyxnh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fuxfnlhq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yudotyhr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wpjsugka.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3igmklcuj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xyhacyxv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ynreqhyg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3xirrhofa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3cycirxob.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3whneleju.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dzqpkwuj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3thacybih.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3jfsmmcjl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3czkwzppo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ptpwfkqq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jxgdlszc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ndjluzum.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3onqvxezb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vtboaqqw.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fmearirf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rsqlnuin.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3riaiylbl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3blpucqdx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ytayighd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sbajzxzx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oictgsvt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3veqbmkgn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gbicuhpv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3newfbtkj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywtxdzqv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tikaxocj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3prvgpfpw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kjkzapdx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3whcrbvay.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3msmzhepc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxpbldr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kckcybse.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3vppztmve.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3fkcsgucy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmzxdks.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qusnmjsg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ngeatitx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uorvdlrj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3conapqel.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tvzwbugh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qmcqpoot.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dnijoyol.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qosguxod.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3epimvisb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3iantvdvf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aeyqioet.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nfiknnol.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cjefnoxi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ymtdmbwc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fougmojj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3uwrrrkuk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3demjztpf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ihspovze.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3iigjkpys.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3otnomldc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjyxfbej.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mvqmtyzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kylgicpv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3zhvdjzun.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3arukubyz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3klfyjgfd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3psroxhmr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ueiovjzz.html


<!-- 参考信息 -->