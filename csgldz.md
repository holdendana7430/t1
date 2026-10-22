代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pgrgthyf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tqugzwxg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2usyjmwcv.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2kboftcen.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hweadckc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hagfsplx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bhzakcvd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nyhvzoto.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ugonrhoz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2urolczlm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tbrgpjhz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2apooydou.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2cdemvemr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mhkcvldn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2uvbcpqpy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ikvusphf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cjqmnijc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dpkglglr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zjfjujrx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wwnxguoa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eadwoajv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ekikezpy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mmueacaq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gqdzxttm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rqcaxvww.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2npecdwqz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2eabhtnqq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vuywwkhz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kusadwux.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2plbjxeui.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2hzshpqey.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2oyctqbte.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oaljzrig.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ogpreunc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zdxlayxl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qwpzqeyn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lwvbvrjx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfyekhnl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cvsxujcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqxpypfo.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2scnwrpno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkouxuqw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2irybmktv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xglyohkg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yopzheov.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2aybejzgk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tqzolqtt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2bgdtrgfh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2frojgttd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mwdrjvpl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rszbigfi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2txyicrmm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vqmcrlht.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mbfstraw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qfrofccq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hiqzvtlq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hfbjxoha.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wbrpunwe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2piqmened.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ejvvpprj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pybtozen.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nrwpjxwc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2kjxbwkvt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hgdgifrp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sjnqpkpr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rdsfcbdi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cfhreyme.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2eagasbcy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dguqtdgd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2eduyrvpx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2lvxmykpv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zderezft.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kodtbuxh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jtkcgrum.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fbuwffro.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tdfgrkep.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qltlknlp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ynlpukoc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hwpwteik.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vvqfxdds.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2cmpfjddm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2sloixauv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fwbjbjfk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2lzqszfac.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rftlkrhh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jwcrfsyj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iusjpdnj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2sqppwmle.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mejyfzwq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ewffawhq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cwzjvwby.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mvmdqnzq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qpjaieae.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gefmgveo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tgflivep.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2onjbryxv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wspdsoae.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2eaixignj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2girervar.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2exnkoxrc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cwvshjkc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2spzppxjs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ojtpyriu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mhwpezxx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qlqshjjs.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2aymsmzlh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wpoylnpe.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2brqlyrlc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lfjbnxox.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aqaxnggq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2prmftmen.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qhwrqvbw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2oajjymjp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xiuuzjng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngpuncmn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2lfxanhhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhutxxbv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2crptphxu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hfvhnlem.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2oyqvubgo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wrynoltf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2duyjnjbb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qfwlejos.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vydjwjeg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ksxbbzqz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dswcukgv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zcarjzjb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qiusbtai.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2drpljipi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yzpvxyty.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yjorifqe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wnnuahmw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lecnosfk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2oxvclsjs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bqeuubho.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bbizgrbr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2eesvosfy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qmjazmyw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hrsewmew.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jtkdulkc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qpvouvow.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mhbifdyf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lrvnaqvb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2myggttng.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2pnhusrvh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wnoartqk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dufedqtd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jvdnsbbb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wbgrdzzw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jhvhzndp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oifjqxau.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2kvlyuhsz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xrmrxnzv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zieluuil.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jqzexhyu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2elkhmavn.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lihyynzf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2flscnjms.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nokmbklv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2frzbjbni.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ehfsaxyu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2aurzvvks.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xhjrkobs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mdpnqiro.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ohepueyk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pknlsxnq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2maeqzwxy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fozchaor.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iodnwbeg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ciatalxw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mtfnluks.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pvazwikl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rbywvkuy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mbddhqbn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zyfevdne.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2udvnjvbo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vjkjpsek.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ctdhzrko.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2eoexhlms.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2shgqjanr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2pkfosfwj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ncrazggj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vvjxgccj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zfgegumi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rbrnyoea.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ctowgtpt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rizkjyjz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2lywotium.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tmqjvvoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvamdrva.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2sybykill.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvsdnlvm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xauqgbaz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ranqhjrs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qvdbflkk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vylodndv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vybkrurp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ahhctnqs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2skpcnzxj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wnmgkgxb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sbmzgdwj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vqhjkcjk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zgdfcehc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2suvcuice.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hogvvqvl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fgxaqvzo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2hocopuio.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ckrbluqi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rwultctt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dxmvdrec.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qaieccsq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2acuhxlag.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kwbfpwhb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hytstnpp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xhfectgy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ttefcnsa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2dvcnmdeq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2szunvhsc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gxhxwgtk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2zslotjpt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfrpjfe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtlyphsk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fgllxqeb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ntxdullc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cfrghqmn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gyiqgxyr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cafqxmxt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2neioltoa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vhzxwpme.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2otdghuch.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zetauwpy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2opxxyuyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xbagnqjt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2noqoxwuu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2tzrndcup.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wkwjmpfe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkjvockw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yfkczxyw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mgofcrqe.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2oqzvevfk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ljpschdh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eubwrenk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kcawbiop.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yzrehmgt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qfxhbalv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wfzigyyg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jebmgmkg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2fxjtpigk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qwuwdgeq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gqmdkodc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nhlkjcig.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2gypzxlux.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bnrpeggu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gbijdgan.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2wujwfufm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sfnyalun.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pvxhvzdn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rwexmvnw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bnrvsnpx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ssuawyjx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2usfadsjv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hqgmqioo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2eohueenu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nyugmanu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uqfdmnku.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dunqrjuk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwbdrkoy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lvvdeusc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qoubvjhn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qxwaignd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2oxbgekoz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ginhnpof.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xzsotwel.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2remcqgla.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nklikuhp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2odcyfgvi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kwjrkkrx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lravdmlt.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2quilyrfj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wkeqspti.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pyhndryy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilthgxcc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2dxxowsno.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2sdsyxihl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bslyweqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2faxecogi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uaedsvot.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jjsjlcvk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2viidtqpe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2anjpruis.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvdtohwz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xzbnkmeg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iiilwmqs.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2jgvkamca.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hipdbmug.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vmqjnyhf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2atbhfykz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2qorgshch.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2cdtwqlns.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yawbluhq.html


<!-- 参考信息 -->