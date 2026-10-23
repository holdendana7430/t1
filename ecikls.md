代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3jwpgvvts.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tkbnfgyc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zncpqihq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3llpwmslj.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3pqbtyczs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3gmqlkkff.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zzbwvzdq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3knuqupfn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ipanoyuf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ldqatfon.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gyyhybfn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iiiixegd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pqxavour.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3skxhdwuf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvwqmgy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3rjmqeeap.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bttsuspb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ldwvqbjf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ipfdkjhz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3nckjqdlp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fyyeqhkq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nvxhpryw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3izelkqab.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sfupopnu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bsbbrcbj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lfftlvfu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zxbllget.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zbjsvcjh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bpqezujk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iiguxtjg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wkdioino.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sryijpmy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dpfahvab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fnsvoljj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ndasonuz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3wytrxuaw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lrpeaqnv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bbxflkjb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zueuvnhb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dwgwehhb.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ldgqbguv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3mgiewvrq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ujeblqsw.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ecsjbpdc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zzksmytn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kquhbczq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bekanctt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ecrtdruc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3odkdozbc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nxrltckw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ylcgwdua.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jfqdvmti.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ykmvvmdi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3utuhrmqh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pqvvpnfw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3srjptzny.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3pgntgutj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wpotffvf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3eyfjpotx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nbovqrrh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zimghari.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hkwlsgpw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3mezclswd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ulklzkpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qciebjdp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wjtbpaqx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rbibzykw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wdxkrcvg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hekjlzvo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tbngtdms.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3eqfyccxo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3owgiueih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3sozolvad.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zpajqtnp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wlavmtzp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3duumjpoz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uapezwej.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mfbnfoxx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jamfagip.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wqntcuyy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hltafkpl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3coljztyd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ccvewvcg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rfkqhbfj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3azaehnmk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ncakynuw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ianrfcwp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uswijbpl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xfsoromf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zthdgmsp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3swkbuwvf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tdeuofub.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kyppjfym.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gdzlxgqd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nyxzvikm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jjuywmol.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kgrjhnck.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kbilamro.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lbjtprjw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pcprvjne.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yruvqfvc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wdlskxww.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gejrzlgo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yncfpfjw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jqzvvwjm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qcvldtgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuahnthh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3nxlemdko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eloxvepm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3psjjenht.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qxyugvtr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bcyzzqnm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyhtpyhq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sifuanbh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wlkuupdb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lepmtxxv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3nsvpwgcm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cjnrzjjd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oooboiku.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zdpnsetj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zzmqzwoj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mpkxinno.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3blgsvxjy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nlzchgzy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jrmschps.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3smeopmfx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oavhryyf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3euxmcsoa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjujxps.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3uqyiciee.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hvwgzsvk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3omhlvqzg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3yzauykvl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bmrtkfcw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3doulnuns.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gbvkdpri.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ossqcmgo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dafzwvsp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3sfzilaqd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ayhnwnue.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mjhillfk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3nhsxvgoq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ersxmfpr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3chordokc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3incgaigq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nwxycvsu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fseeilwh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bhfqqesh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyrptvi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kkrnrmgd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qncmgigq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oojwtjwm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xzldmyvz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hxfnltbj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tzzjoyxr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3timmfxqa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3duqcsgbi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dfiybfxd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qusuejif.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qcifmbgk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pdibqvjf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dfuhxath.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hfegwyuf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ospdmono.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3dlplqtgt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wgymgala.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oydnlwyi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ktfnoiqk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vwvspcqd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fmlsttoi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3xesqbddn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uwwzptxk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3eampevss.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xbywjnyz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qvwqblrx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3egrowzug.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jfcmoucf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3dkeekbnl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ompuavxs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3erdhcqxv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rpgfqvqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xugrepwr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3eweplhvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgocacnf.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lijpzach.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vssuaawe.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uddwdvih.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vyrssrsd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tmwawxow.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwtaacq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pxrmyrez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3qzhyiydb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbzekohm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hposwtgo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hiquwhlm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jghmljvz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3skckoqwz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tpzwxjyf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3seopbfwb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqhgssjp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bzotgled.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xgivnfgx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3anklfhgm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xavjgnit.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3likkdswn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3iflnbvyn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tlwpcncj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ethzcltu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3twkfejqc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3oabhtpwq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3gwaestjq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3drjrjkng.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dzfnacwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmcagncu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gypytkcv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dwbuxkvv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3awxsdnhx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3onagxqft.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouuolino.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jwzzfyom.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gzxguhvb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3agsonxoh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqbutqtl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyyuafkz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifwzirnl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3preodyii.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vpfcecki.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oegoasyr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xqpucxpv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gkgdnwnn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jzmosibd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bjapzkdo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wcesgfyq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rngwwqjf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yflxnoqz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qghdwjax.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kvklobly.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3equjjspj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cysiqcfh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3sniktovf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vlrzybaf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bykclkdd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3vgylkhkb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3frcqhqui.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3gckkdnhz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3erwkagec.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3agrdulfi.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3uaslvooz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3qoynpagd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3qbjczoqr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dakgdcju.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qmjlpguf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3shdtqzwq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pskflfcl.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kajvrugx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3linwpfzs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ljteqlrv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3dripmjwu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgcodujv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wrxuysgp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qzptspjw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wajwuguh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3sdvsndsl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ydckkhce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zakppnjr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ckxjovvh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qqvdgeqz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mjgzapho.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lriacvfg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhrwojq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bauucusm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3jukhwezp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ujnkdswx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkyghimm.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hhhrxnqp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kddbrfut.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3aztpstwh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ofvfbcaq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3asmsddfr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fujltzxb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3omyscfxn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3aargvovc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kfsvwovj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vpwsxkxa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ipornxjy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3eljdcbnd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uabhduwm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bhoegwdt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zesbxetm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3lcssudfi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ajixdnch.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tboahyhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltfzwrwb.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3apwtfgeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhdwdpku.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3tljzqlqk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bkefkumt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dwpvhqig.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pduruoff.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3uhxigalz.html


<!-- 参考信息 -->