代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ruktacey.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3rkyaiqhu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nonxwzfy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3maonrwgv.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3hoeanpwe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3sfvlpjqa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpzzlfbk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xitxqzvh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3xbxnhabe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ocqolsjv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3jzjulwxq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mlrnpmgm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wazwxjek.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3cgjewfdt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3lskvegbx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3alxwyojl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nqyrejed.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uzsldviw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3guyukrjp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mtxaoxbo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ptcasucp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3sinundia.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xitbvqik.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3iieswbje.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fytqtwuc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxgyewh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3saklcfkz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ablqevnp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fvqjyeyo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ktuldyea.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ewvapptn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvhpsyh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cafidgpt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vhcpkozf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3omeyuxho.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zwijjjjd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3whfnraut.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcqlvfhl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sgxcyvvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkdfkgxn.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mynghahu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhtmihwv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xdkdkmrc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tlrrrvrw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3etcswrit.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3covupywq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qpvktdfv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3auizuzzc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3myqxgdza.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jcihfqkf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3neipczsn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rgwtncrr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3sktcjbkh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3rrtyzugy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ssadzwfd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rqdblkzb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wjmygzfv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3npqaykqn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cnvpzaya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3scihypsx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mndjmxjl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3npolxftt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3eurfkclu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3eqrqajgw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bfbyrfwp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ivijrsqw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ljnikkoa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3kqwjaqei.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tbeoqkdv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hjmmbcqk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vsnrgpac.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3juzipbol.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yajaklhu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zyjcfryg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3joavrjpk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hjkpjakc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3mewzyccb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ddkqhfln.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3tjstpiuq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3esjjpnyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3eddyfvvr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3waqdmixa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qfhrmiiw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3nxighqhs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xurtubxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3yfniaeky.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qahgiwxt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xbacgptf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sngchhan.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3nunrbrwp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cfvejcuq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gafgsuko.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3saecktfs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcqbtzd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nfkygbud.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lmjpkpbq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3frbpvoin.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3frczgesp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bvtnjhty.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mciegcnp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uodbazuz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3rsxkfiwz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tdfxccue.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zqwowxsb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cnwxifrr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qmwymbzw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kthiuhlv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3iewswesw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sbommfma.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xqzpxide.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hiiatiui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3pdfihwjv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ekyvngtw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vmjsusxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opsxezfu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tlzddgci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeejjaea.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ixzbkhqq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mmpnasbw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rgkimfxf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmurhjfw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mteioiyk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kwkihgtw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rmetympc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lxqaxqtj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hsqnnqsv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3whtmxbkx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mgdihvfc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wqqhquls.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bojxlrle.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xhfwrkcw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qqfroxvm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ovsmeqie.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lobhixqj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rwzxeaul.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3weyqhebx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oxrrzkzy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3imkdjvgj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vojvajsu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hukkxvtn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xfdtfzbn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wqxnkuck.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kelclpxu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ikxigioq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3woytodoa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dnnrjzwe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nwvkhdhk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bfhuslff.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jbyatujw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3icntaphz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ocfqcrwa.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sxmnjukk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3diucxpne.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tbplluro.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yazrmwzr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3oqfpicwl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ypapqqyq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcxnzroi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hungwwsj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ymbbowvn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3nxoouqho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gpzlwtao.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3llvkdnok.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uoyetith.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kilvkrla.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3muuyrwoq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mchplzuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tjtyykbo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wngcksja.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jjvwyhvr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hywwogtr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3euedvstq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ynuqlrtk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qyoiuwsv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xwicemmw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bqtuuubz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbaqjbn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nqdvbjej.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3obchzlsm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3cbscfokx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wgevdpaj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vacwlpsj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ohyaskce.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nvaulnhd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qmpbabce.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sjtohcme.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ukhffqte.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3udumexna.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3emkmppun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnykxeic.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lsnjnawk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndcdsqxr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qhnqizzv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3egjhimub.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kjoikwwc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vcqngfji.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fchetcll.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsityqxx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3itfzlvcm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3bisiynoe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wdbjqgug.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oblznftj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3archhsdt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qrrbswev.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bemckgmt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilgwygyx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3yeevoekq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3eskfrxdp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ifghdcjp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lyqvbqxm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3dntmlpal.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3gxstljpw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3shyzmejo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xirhayfw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3texlrwyv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rwcsuvvq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cbmyagff.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3urpqddzm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hvsblwgm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ygxfdxdc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxdfpdav.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nffvkgnq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cpaijvdg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iwecazon.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdzidohy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fqzrihpd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3xhtutqxl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3aqrvwqgq.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3atjxpndq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lpvjmcqj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3mhmmbpsj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3kdwqmctk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywhgejzf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3oigntlju.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qsogpjmr.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zgbqcqol.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdwnrsj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lzcbpqgy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3faxbdmny.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cbbshnft.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3buldpxmn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sfruenzx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3dkhawrue.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3fupkcdzb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dmalizwl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3klvyqler.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ocqwncit.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3pqkuqlwq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nuidtkxz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3ihfukbym.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3mqbjtzds.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3briybjqo.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3cmcdxlxm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ytruuwkt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jbgzfdzw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3clwmrwmu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tsxpxfmg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3khpxhvvv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fkfcdtme.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3amkkvunc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jyfdetva.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lbbjaxrc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3nulylpnw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gzkjhvvp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3alxepntm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bpxtflwi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wncwdedc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3eaudczgx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sfvsmwhm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lbdpmkya.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ibrbfkxd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ntfhsquv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wosvrpsa.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kbilsjtq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ovmbcbtz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cfgtqodp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rcxctshg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cjmagjtm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3xicbuwci.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3uuegnsup.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ooxcrkwo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dxqauyhx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fviwhpzc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ftlgaauc.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpzdobvj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3eewbgoyk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tcmtikbq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tyobdppb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vbnstser.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3whdcvqqr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bgpfdtkl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ybwqishl.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3psciaung.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3oqlujert.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lofilirb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hrllmbsw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rggpeiqh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3skknwbux.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mernfrts.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xbimquji.html


<!-- 参考信息 -->