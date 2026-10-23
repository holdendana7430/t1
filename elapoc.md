代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3clllpcri.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ruhifunn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vapppdyx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sgydvsli.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pqaajwen.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3oipwjdth.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3teohcira.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3choqaxsy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ytazkxes.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3mddahfoq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3twtmqqns.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qecciqbp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3plgugmal.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iqurxmyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3qtbmcjgb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zpeletwh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ouxiopcb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rcgngucy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wgvhkztu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cwnrumdn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tqyouhct.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gnhpavbb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hfmecbgx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yjgxeafi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nkmtltdw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3dhhholan.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wvdilmlq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3sjnbbthd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3woimfuas.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jxpztnal.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bvcxugwk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ukrpejad.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3wpbfmxio.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zorujiik.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3eqxtnjqv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ffhseoss.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3tgtvtlum.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zzwlxbha.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kfyxlhcz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3rjxhadyq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3pkejguvl.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhubczh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3halxiuzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjctnidz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3oqktwfzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbqrdzzp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3aobfxwza.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vlzkpgjt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qwuhwerq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3olyddykc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3caqefrip.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dlzmguot.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wzcmexui.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3llllewqi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bvevbjzo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3iwnspzpk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ibgpzchg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3cwwnowwf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nuehwnrb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3azldawyz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3unnypgsi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ntunvulj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3chswmuwd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pgrnpyas.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3kkcdrwad.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3hojtktka.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cmeygoqj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xsviaxiw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bubujtly.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3jcewjkqy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vcevjhjf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qrasxuxt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ptsenlth.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3arhpmbtt.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lvctczvd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qehtqdzn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ztgixfkh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wxrawobc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mpgisija.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3qswtupqh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ldpzhcxv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bffvwllp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ypudkjfb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mgapqcyi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dospguzo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wzdccmyr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ccbfsxjo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wiaepmne.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mkksajgc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jlrdddhk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmbsxmgh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rjxbetpm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tixibbid.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3khthbmye.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3knfbsigk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ohmoagfm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ajprccbe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ynpeovxj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3fyzvysps.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3teybwsxx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dmbbwrnz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gpmorktp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ksqendtg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hprtqkkg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3axqdcaul.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dyripjuq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vdbjsxsw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bltgosrl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qcjgscmx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3oxwocsyg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3gtetfdhn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3jlndyuqe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3swacowxn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lvppavwx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rotdidfv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ziszidhf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hdtfdbkv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3bpuraqhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tvpotowg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jekrvlhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdxyimte.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3oxuwsktx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wgzselvm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hcwbzmii.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qcibznqi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ywivjrej.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3btmtmack.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oijhgcgm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vaomcrzi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hszsnfhv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aojrvvyi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hqlbmksi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bwegukny.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gvkxkjfi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yewfckdj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vhbciwzo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xidtyniu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ndbbupwk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fvgiwczp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rxpjykjs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lpijuunl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xywjgqsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pfexcqgt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xlmnoiwq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3glxkpsfz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kciwirrd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rmwhqwbj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3odcutdqn.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qkctscda.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gpjtxlqj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vpzdkmgt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qcmdzxks.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zqmpblbk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3poymfzft.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3aodqrdqq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3gnnqneeq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qpmxwyev.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bhclgipf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tagughiw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3panwymdg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kefgysng.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqknbjyl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmmmhwyg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfffosar.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kffpneti.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3hecklqvu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zttcpjrg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3epeguikl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pwkigtje.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3shcllesa.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rbgulmdp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xnspqqql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wbbugboh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3rutvlows.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ulrvchsp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ttxtqgjx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yxozlfpi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3sxvngtxb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gusgnvga.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fzqjrmoc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cdatmvxk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3adjlaqnc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zsnqnvex.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3bouydprw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zsvommbk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yumogsps.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dfpcztko.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3fkqkabpm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qqktxtmy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3txfoaxty.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3jspqyjkq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iywrxqvf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ypwfkuhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emnroxii.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xnaqetph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekqenprf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rpfjdsyz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3apmzoput.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hnrqebxy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jlzisqlw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mfuqbuce.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oxwghwfw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhmpfif.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3znujulti.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhyfeahv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3evmbtbdm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tqywexwt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qscibihn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xdxmfehz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iytfuhsq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ioqquzkl.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svdcocbt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qqsvykha.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3guvghgpy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3eghbaedo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lawkbodj.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mrrvvmic.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mojlmgqy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wkotidga.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3xgzbmxwt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nygjeeya.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3warjtonc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jauyqpar.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bfvculdp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bhtiajhn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cgenmsxg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wbvunmtk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bcdudynx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fnpednwe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3alqmswua.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tomagbpk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3npwrdnxp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3obdpngrl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jfkvfege.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbdxwouj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yzffokkm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wezklfsc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xncsfjbo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3sposgrpa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3hkbwqcaj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3tiizzueg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3amjymohy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lwubcini.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zswstkij.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xgtocqxp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ghxgpurz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gvsxvxra.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hrlhloex.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3onpoilei.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3taljjyst.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ikvwdruo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3apirjbls.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uxdyfxxp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbhkcns.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3cxptvqev.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yydzoxlf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nfddoyfl.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dtbbqbkl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3dcnonbkj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pkrhllrf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwpzljng.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3yywouzlq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3etbgorak.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yaqafaqz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xurgoazt.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yuluovpg.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3dllmized.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wdpoekhc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3elsguglk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3siebtiox.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ltssytjy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3evfpnnoh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3oygzejik.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3pquyesks.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3apgudczv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xfwiucsr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ojpkfobb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qolmwynk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lrlnheza.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cdsjempc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iqzwfeqh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pcsechgq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbpddxfl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3bntcbthm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pirpicay.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xlnlfdpi.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3yyfqktku.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vxptjvhk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3pkdsiyhm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3cdnuiuhw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3vqstpama.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3akiwnyid.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jsxsoqpm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3cquwbacx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hfdrauyj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3aofvcdox.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pifmhssp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tgbahlqx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fldmlhyj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3urmtlhbr.html


<!-- 参考信息 -->