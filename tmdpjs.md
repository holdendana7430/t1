代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3efvbjzau.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ywwchwla.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mlddfpwd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3uumtmbay.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3blwahcsm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3usimzsjn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hcwjtmgm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xlgysrsf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uvsywsyh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rpbjmvij.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cpnuceug.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zvwjfnzg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zmvewfvu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vlovndtd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ycxptlsu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zjhcjddi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwuiypm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mbacyjxf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3psmgxskp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jhtdcbdr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3grfpzurp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ylkhcfsl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3oxpmrdoo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3svkwjkmd.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ksuxwoqg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hjigixsk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bduyehgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwworylt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3pjjxymii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cntpdixr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ikhbitdx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3fxivgsah.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cnvelzdl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3abxdturg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gnhnkjir.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3axdfvsyr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xplqejer.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3nwklthvs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3spltedil.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ffhnbkdc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ksmplkha.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nxcuplql.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ecuonsur.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vebangao.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3axxhcyem.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vpmacjzd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3uardbfrf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqkuynil.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3maolxtyv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ttmjbraj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3igkzmyjs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3sgkjoelg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yqmrfmjk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hsssjbgf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zeqciauw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fbrazzdl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrfvzn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lkkztsrf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wzwyuueo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3idyvkvun.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nxqmjxfj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xpnraffm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3rymyzcxi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nfqmbkkm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3yessgbke.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3esjlhqjs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3skczxrzx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zpmopsgp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zitngzoz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3khosgunr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mxymnytk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ffniylaq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3dsycuprp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3odncspeu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mimbbold.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3cwwqmxcg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lifadoma.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vkcolnaq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xwswbuht.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ktqpxhly.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vtrxftwt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vshimjek.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ghtxhlhk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3najhtmaq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yysadvzh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fljayxje.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vgvtidlb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rbgzxues.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uekqvplw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hgsjsdpj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gkynvklj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zlhdhzlc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3xtvpwpea.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3uvowzadj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rdgdfhrk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3cmxyomuw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pvwvqexp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ruavdsfd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3mzrgpmuf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sleqpxnd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ekxhwjho.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gsiqfilt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zufdpzce.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rdfcdqgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfxixexh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbrvnhgj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3isdmuuss.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3lqvjwmyk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtehkmlp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3aflkrjas.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kbbhoamw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hwynchbv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3atrafrgu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ncmimyfq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bguljxtf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ngzzzplt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tthonntk.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rpfafmwb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lycjggrm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nhuzuzck.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3trtdxilv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nfayeunb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pvlnftox.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lkvezszh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3abktvsft.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3lsmhdscf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cftgrpwp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gxsjjqkg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ntqmripi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ozyeinir.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gkrcmhqi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ypqgepma.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tzonfnxy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qczbatlv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qwgbnxvm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ouwgsgvl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rxflhehk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qxacszzt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3nthxwgmz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cqixvxqs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hodfengy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ketlvwsa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nprgvxvs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ysyrtojm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bfzhvspl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3okhqlhne.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eoafmqhf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rrlwolih.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3imuhreki.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3agoogczu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rwxwcsfz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3fetpwopy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nksgqqtv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3roohgkwo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rwfhkcvq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3njgycvwo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vzjuytpd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3dkkqnqvb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cswjzbvd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tnohqcaf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fdnmfrtg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qysgghhl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ugdktlyu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kxizeuuy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zmdhvjaz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ndessjuv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ulnwgjlq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cbyrtuqn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vesdxpzz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yeujdrra.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3npucbahs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pwsgxqjr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3swqsfmzn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nbnxtlkf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jmmulhah.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hsfpfxsg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xuatrlhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvlkozhq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3uedbfeis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcwkccns.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pmqnqemj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajymxqds.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xlynjijb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ecanvnos.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3acvrueay.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3edfdtgcr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hzeqtpzy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qltrpdml.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ijqkrkfi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kfcznuig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sstsmhii.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yrwqqekp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gegxmmck.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mudcjyjf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wchgqzwv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rkjiaogh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3unvbedhg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yhbntqvk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3qkzcvmxt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ukwcqpur.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ezqsckau.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eaumivwg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3yoivhoxo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ldmsefrf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dherqjrf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3iubkifav.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3udtgoypo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3tdfgdsez.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fhwikcjx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3oowogndn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zlqiznlg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mxuibfqo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgzqqciq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3vqnbnwza.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aokfzeia.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mcbexhzr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3dzwftfth.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hlhqrvre.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zmnsmdnd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqkvegum.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fnrooiwh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rzgzbbna.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3yunizuwc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xejtrurw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tiadgxlh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nrjqstba.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dqjanbcm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cuhpqymz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3syqsckjv.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bewiqurl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hnchumdy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fgedvajz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hbvqtmqu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3moxbivxf.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qojzcmts.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3mhdselyi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3mrphegau.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mjanranr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3dxhuyrkm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mdomwwfd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ybzovfvc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3myzlrltl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3uszyzvzv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hybynsvy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3izyjvjam.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3bvjdujgf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qloarfgk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hnsiywbn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ogerudjk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3batmivru.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wqpvgrme.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wsjxsgfn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pmnvrxll.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nltrezem.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fukulwbi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3itoqvclb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qcgabuvs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3klqynrbi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3hsqyaokz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fnfswqki.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hjbemfyh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3hxmqjuhb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3capkkvca.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggisuyeh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3rfojjbzt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3dvyabbhc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3uipjnqha.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tjmejsvb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ddhzhwam.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wicueikp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xgevaqef.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zvmdeaxg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3rnhafkuj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mlziuzlr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jiwtyjut.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wfhfivbl.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qxehwvtu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3qwmzigdl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ggzktqrr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jixdjvso.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ayzqhwip.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ommwpryy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yrnqntyz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nxlcnyyn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qyqzlhkq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3oaooxiqi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wldvyobc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3meohgarp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wykwsefh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3pbauwqdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dhepmxvb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kmsnykom.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jnswmuuo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3eyssvuol.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3tlejuvcb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wcpsvwlw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kcognsfb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ettxmxso.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3fakmjhln.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wkvozxmx.html


<!-- 参考信息 -->