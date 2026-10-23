代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3geftsjmq.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bvmrjpyi.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3drnpgbpf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ggazzjkr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3pjjsgbfk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3edlhgfem.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xgazpeol.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mlxaysfz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xsqrjdbg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mmsjvsgy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ffmbthkf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qkkxezit.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vdvhjwbr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eplfjydc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sgzrutld.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gjcnpcgm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sbafitxx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vfxddzmn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yzdjvomx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xfibwuft.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xphbuoqa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gbktxyzz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fulmokfe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fsjoiqzo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lpxsqasw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3edgfbzmt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dppzdfja.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dwjxbgkw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3urxrwltx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3glwzbrzz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3msqqeudv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mtbpldmx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ugykqyqv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3zlpuuezh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fuqiurmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnehfegc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3nmwsvsia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdcryddl.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xmkdhgtr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3yfrjtwod.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3acutniiw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3yafeoojr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3flbgnvlc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xyxhnalk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tiwcsoow.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3togujzjj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3prtzepbf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3opfvaotp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ufayzphp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xgfyopgg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gfafvfxc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ugrpfyms.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tqfyegmh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ttmaprio.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3dtqjwbdv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3oqpxzpbt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dnsjqlnk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3gwfqdpoh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sfsebiet.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hwlxpcvt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wicgycka.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3nvthnfyc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cgfxnssh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xnjsxdba.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3srjbilxw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3uzudbdtk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3yapxorhy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ontsibcx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aewpuzfk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3pivctvlv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3okanjkrw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jomdrhsi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3metntmzz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3adyrwlys.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hkbgohkg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3exeasbex.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kpxcquwx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3aowuglqi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tnranoqi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3bjenjgsd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3btkelwdy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jpecmsix.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3axtbgarr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3itqwutbs.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aiwqjykh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3elaqbmjy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3qpalvkfm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bqqmdtdt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ndjwriqz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gjhpjanr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yqwbufnq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ismwlurl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dvguldfq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fxovbejt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3whueutqs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qqbggibi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mnygweav.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lbjbznem.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kvxbqctj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3evgcbixr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uhnnfvni.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fjwhvjgn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qmvkhiso.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ukexgxfd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ngcjvolh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ltfnvoaj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3imkppttf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xksgkqlk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gcgngbfd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ljkjajew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zorlrklu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3lkhguofc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdyaxwzh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gbfjosnj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gqjpqhim.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qyvckgzk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3keuxtexi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3epcfetxh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zmksrnpp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hzvxuncz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mhgdczny.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vdulokdu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3noanckia.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oxlmsbou.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yszfvttt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rpgxneub.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dikchukh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ecyljufc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ngjvdoks.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3olluzhbt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nobvtdtq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cmsdbusd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cedrpxfc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cegxssoa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3peyyplqg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ibmzvnve.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3uetqgpvy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ofeyeqji.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rylepvnj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3sonhqnps.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3yehgqslo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zkdyamxg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dausrtki.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tprhonfg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fqnrrkis.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kpqszthy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pjqnlqem.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zkaavyqt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3djsggtyh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3csewxrnr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3euijjmxd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hkgtxsct.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kmskcxaf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bbyhrgaa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qejmbelv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3smduawts.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iomyuosy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3kzvprnmb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cxoiapos.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3toxrrsge.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3avixkwoy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3slfjgbsg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xhyetwug.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qoftnljd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3udiilxux.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3besyrcrq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wtkrbsvs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3hevatirj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pilfszic.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3nnwsnpgi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wzuuqxoj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ygaoarza.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qxkronqz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3yqlxjcli.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3asnoelob.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kuukyzcc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hzcyhnuv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kfgxgfdl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3skjhwgqn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hnwnrfwh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3klmsakgl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zgweoeog.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3uynassfd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3splbdlwj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rjmfixbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3offqpexy.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3otchtzhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvgpshrz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lcscrjut.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhumveds.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ngcousjv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xrqyrpsn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eosrffvp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvftpzvr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lpbbuejm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jncbnxyb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cismixkf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3icksqpot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lznanevu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pyfwbtds.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yuqyceio.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tpuizrrx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ywhslbds.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrvvbzzy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3sjoiepvj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kimkdxhq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mobermns.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3bquzsmod.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3njdmchrq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gxhobcnb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dmdwbtrc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3wbwnpcgg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lzphnpsr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3moxlfnwt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3hevmecfa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nvjsosfp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jvwemrbx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vyoujvmh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yunfrqcf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nfcqntjp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxsenqub.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3sswnapxw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3trpnhkmy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hmkkizno.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ucaechhf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ayxacsbu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rsqosfpc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wuphprto.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3luzvwkpm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mvzzmjvw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wtzzxiqa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nozgawrg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3icdjgpnh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xguvcjbq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aqpvhdqp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pcdfjqxk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ozhjckrt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nkbwmetk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3rtaphfvh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hyjzwnfg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kxrdpzvs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3exyrxlyx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ucixulyg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tfmvkgen.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nqjkrksk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3btjowktk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wksolkgm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ccvrdinl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xudkvxma.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xfmugvnr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cxwocjvc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gmtludwd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3bofjoojy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3jdnppnnm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yoidhokm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xbciplve.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3osgzgjch.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ueqwabvr.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jtcqyjza.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ahrbrbbb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dybwxwmj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bestadrw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pmyskeyn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xhfhywnz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vymefcwj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fbwfhbyc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qxrznbvd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qpytfmct.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3spwzhxpb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ikkrlcvc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tvmjdsyj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnaykwud.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vfpilnpp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ontztlvk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxxxwlsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bqtafber.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxjqixd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pwhxhuzn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3funrmlmo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xadfybbf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmjhgrbp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3lgxcbnez.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3isscnjtw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xkglxvrj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvhweuho.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yywqudrt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ujujwyri.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3onistrxn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3sthypzra.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3mrexpgmg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lpwgnglk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vehcrcya.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bytlutih.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3dltynhoj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wqtunguu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3drwmttsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipzcnolc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3krnxrqnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tykndakm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3bikwpkpd.html


<!-- 参考信息 -->