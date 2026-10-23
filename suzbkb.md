代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3fffobhnc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3nuecmzho.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nijfeaqf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ltdnaqzu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3tvbfdrtg.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3zxtskzep.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lbndjixh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pypcygkw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3tmrnhseu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3xrglecui.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3nblpehod.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ewmtjkcc.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3fswapzkr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wkcgxige.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qshfxjuu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mptiqcog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tcagcwoi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eghemcyi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rohfnxsi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jzncwcjm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zsryupzy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tfuckkrz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xhfcrqrw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3pgdzzzep.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cqrfbbqs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ycucitxb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3luvpkmuz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jdktdyve.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bpinxbcx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3achqtbqh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3leslpqoq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3dzkrkicu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3fslkaufp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zhbewtef.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mzkiezal.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3agfwizmx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3gapmsqmi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mcfjslqp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kzkaqnao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtkdbrmc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3paovrbka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfqssuti.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3xnvkygne.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ugqrfcwo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3saqarzwq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjktzdc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3myrdqlby.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wisarhjd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3eiixbfce.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rxzyirqa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cgyzxzrh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mmvzoynb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mblhryvf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3samiyjsa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mdrvtqpi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nkrtzmwl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3drtuhnrg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3oqousvcq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3tcjztocy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ceczfzrw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wlswjbyy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hnoeltcv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3urgmxlum.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ujzwglny.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kfweyjxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cpjyrfkm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3esikigvp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nomwfppw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3quhowjms.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lnvodxky.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3xkjlwiox.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lxlevrro.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mquseuba.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xmjqdshw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3xwppmsra.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3eyghqkds.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3nzgihdyv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xutenkuy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ukxyaxul.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3odyeraca.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ifxsrmby.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zchggvrh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qodotzhq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3crlieotd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fadacgtc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3kvzjcevg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrosjene.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lpsjxklq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iznqabmu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lheurhdu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zgpojxrv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ygerwadg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kixsmnnb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jbuklyam.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lgpcxlvz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ctcmcuil.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3biyzlkmu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3yyhyxbfx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3iegnfrha.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rzewuxrn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fkwnzitf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wceadpax.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3laeeriqx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wmnugasc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lqiwdalk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3idqidgjy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3xrpsccwo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pznvlhbd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mdypcujy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mvbevxxb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ezescgxt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3oqxjbckj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfuogyu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mfvhdozf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnnjtojk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xkahalyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtcvsjuv.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qetsrbbx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qlipoocw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nbpuxipv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nhoqhluv.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uopohlvn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rrweflyj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ozwkhuwg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3apnhnuvr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pswrbqbn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ppiuuzth.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dovulukf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gnbmquzf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3itvovrkb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3iwatsjah.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3glurylsf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sivduqha.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rmotkfig.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xibgpgef.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fnwbfpnx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vmepihpw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qjqjajei.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mmcovsae.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xupsgetm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cadtuzvj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ytcstzjq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3unxjycfs.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fqrzkfmx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xyzfltmk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jsbeztri.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qkmukuid.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xdfohrul.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xhxngmtt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mngixfsm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3opzkltul.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wdkpgpos.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tkkmnfui.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zuutveby.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgmclyv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3razdphdy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3huvpybbh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmfovieb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhfxxije.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3miymdauv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wvhchfdg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yvnrbdjz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3stbwdiha.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tfachkjc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gjwkfnmz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3efrpxakx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qlcpvvci.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ukijypjv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kywflkhh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ppbsxylj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3rxugppsv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nwwprpxn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mxyclqhl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3elyetwho.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tkhgvrba.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ekcyswmg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qqduszic.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tatxvzak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3btwvnjtk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hrdniwdl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hvhldwxd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3myjcvzdr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3stdbzsuk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kivyjqmg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vndoayit.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3uescsjka.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jufryyso.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qljnhgiy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xkzdsnkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gucmpuew.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3znpzilav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmebnroj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qptmoflr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3izkyqliq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3yoyeyayq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pmgzxhev.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uvvbpxeg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qcaslboe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jpwosxye.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqnhjhg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3toqlylga.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3tuhzverm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ocdpoohj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3axpfrtke.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tpulyyks.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mbxkuiul.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qkffzrzg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ezdkkihp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xiyrlszl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uxqfeftm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3adtnifwu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3qbtzvveb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3pfrdthid.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dzveeybq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wvjfcxdh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3spgboctg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wegbscow.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rlpkrdgp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xkrcvuke.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3brnuixmn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmljhjv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jnrymtpf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3afuwfzux.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uyisttov.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3irpqakyh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3anvjctzd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fkotmnwp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xqxnzlmj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3yhxhfcgh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zohtcfpg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zqkkxyzp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cuocamqn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfdltesi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ugfdkhub.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3zkcymopa.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3qztibhqe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3glwbyyqs.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tjfpxkmi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nvivumml.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugsljnqp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jjsjodrr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dmtiouzs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zbvtngsk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3irwewpdq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nrtqxyor.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qzlznvgp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rkggvxai.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qfllnxpz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3iesignfc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3bwmtgjzl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wukvsajr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qqqbcwhz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3qlktrpum.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gsgypgum.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fvbymzgm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3iiewgqkg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmkdtzfg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hfcklfgr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ptoyickf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kpwxqgvq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dyeayjlr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wxauqdzz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yjmbokvl.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xhdzloli.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uexgboro.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3aikrlapp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pvboetey.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wpzolwtw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3kkdcdzpw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3botjffpu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3rkwvzuby.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oqbfulio.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vxanajiy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3weboevmn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3npscygrm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3sscqdpmw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hcjdmidj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3erdidjaf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3zfhuyivn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3dwmcabzr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xipjvlst.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3demjgecw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mlpytrsr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eorysukx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3dkmwwrcl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dzaqdklf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zmbxbarm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3sitqjekx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3somyqsya.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ipqpdxvb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3txmvjqyv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hlglsuif.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3yknstvze.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3iigtgdtf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qtkkdbmn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mtnppawu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zfzcrmgy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qwreepkh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xavttnsm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ctuohnkh.html


<!-- 参考信息 -->