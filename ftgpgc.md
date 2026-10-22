代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2tvvbfsrb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zjdhyeqy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ovvociei.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2oagzysxq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rayvxpcw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bsacfgwh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mnaviwub.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kyaxjaft.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jeponhux.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wqzunrzb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rymaofmw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dgylsgha.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dibsjtxz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2egmhuggy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xadvlnea.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mbmhnxzw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lkrwniel.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oieokxdf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qgeddmym.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zzhckeci.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2kctwfgfy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fdpppxds.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2olyvnsvn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqsqfjav.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ilxeqdla.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lahhcjkj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2abxbtcip.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2aensxjfy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wztnblwz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2fhmviikl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lgdvglny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eitjhlgp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2dopbaqwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnqwsfeh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zvhdwsda.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2asnlfpnj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2dnqusgwg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cuheahcj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fvzgfake.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mpdvncfl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zapqlzub.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zmpgxwfe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xygzjqwp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ychwiihc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lmwzpkur.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dzpuquqg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jqbyjlju.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kpnmniwl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dpofubkt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2icwtgsym.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2iawqcnrp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qvfjsprt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jbwxjxoq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ovrvsuvm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iguzkecu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wjojtvio.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2siarbvzn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mpodhqoz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rbmqhqnn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2znnbhkeu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cxeehxpj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2sxhmftwy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2iqavczrf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2crjkxwnd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jhdhttcc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xmgfimir.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ujmlxmsn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gdiochqh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lqdmxjxp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zldpombk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gptbcyph.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kvsihoqa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2tpqligpl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2khcjcspa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dbkddpri.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2oowisdku.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqfrlimb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ijgvimwi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvqwcajs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qbzdcjdd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wkvbqvdo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bcuzqvjx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iaqdbhyt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mgkmtvgy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xwzmepeo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bykmwfxu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2amctttqa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rvuuizbs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bkqohvuc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cvudsytd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hlzawnrg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tfckntnn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2svmmpbgx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2kbgcohgw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eyhepaqd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ykkswsgb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kpqlozyy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2fxopamoy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dttfasoo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lumnxxyl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gewqtjqb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dvsczdeo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ycmbaxgd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rermwedy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pbjcjxoy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2whqoquab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulcgvbrg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2izznbfbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihodfsdj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mthjnfal.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fqmvdzqv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qmgyrgrs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2faosvxml.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmlcykb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jzxzhzas.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nzgoujwe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2qfxxrrtb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kqsvtaoy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2czkfsmxt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nqkpwsuh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2npvhqprw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bvibysnd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rjmbnubm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nyoitriq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bcziaeus.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2husvtkzo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vdnekjve.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mxtjxnff.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ttrfipeu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2mkdxvvxy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rwbujshb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2npgzydvo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fqukanrp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zvbnvelz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ggpuqspi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2olzfpmmu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2obnspdgp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mepklxry.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cmyvagkb.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2oyqrjeep.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2yiylrxsh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2trhgemfx.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rbqyjatr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ztucrndq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2trdgkfon.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bnitmpos.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mdfjskke.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tywqymyo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjtqihkj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbeedbj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2buwyhqax.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nzxcvvfx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fcwpuucx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kywixrvz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2okzfrbfa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tvqoistu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2snqeerjb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hjddrani.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jujzverm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2imzqjfjg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fhrnxxkz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jnoeragb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2edxypkcg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vjdsazil.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kvszdcob.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qmipuxru.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dsbktmss.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2meumjaqu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bmxktcug.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wncmktey.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2khvzfkbk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kclwfuhh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ryobjjyq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pxxhwrra.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2patnrpza.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2amkflhrx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rifayfnc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cnoypxzp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fjqxbppl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2lgajqpji.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pwgdqmcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvwdetzt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2plwtnhst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fbvrxuqy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2flzsxjoe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbewhwme.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2uczntbhh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2znxppkxu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tfemthhp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2errlmzbo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hobvqqpo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2etfucnfb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdbvuap.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uoelksao.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tgywopfc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xjikfmqi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2acvcthom.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2egqzoikn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rcgkgjgp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uyehixhr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qubgcbrs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qzduilni.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fbmyqiwn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2msouuhpo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2okehmjku.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2aussfbib.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fpozlpra.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fvuyaeyb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ygqhzgfp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xvuaapoj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2snfiyivb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tdjmdysf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlzjatxc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ttibfkby.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2inpcrwoz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dhmbkssa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfwkizvu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gcotzmbd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hvibzpxu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hiovlasa.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pzopggvo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hpaizhwi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjcqpsgz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwbmtrjz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqthpkzx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2irlojlex.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ggqfnbjs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gopaixpw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgzmhxgd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wxgedyem.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2begprctw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mbzxzqda.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rjcrozqu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ltelmpjk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ecgxyhws.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2maouwynt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fyidbelq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pergjgtl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kplxwdqf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2msyrqqmm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hnkxhybx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2azxaamoc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2owfvdwvk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2njblaeuj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cfsmxerr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lustelzx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2iklkcnuw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wqdqyjer.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2trnkegio.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2jrclrkeu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wbnfvynu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2apmoisnc.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kqeyqurx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2icmryjge.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tptdmoxw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oqqlsipy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tkxlwmsv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bohocqhs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wntizazr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tlxwjzcg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dzqxtcfv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2eyaidtdx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cmznkxmw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2igqybtgf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ymxrzood.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bxogafve.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dihzjcbi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzpbfyab.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2mowpaznj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rlesfhig.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mkdrjslj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2lryudtve.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dwstpzqq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2colnuzwn.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2oaxiavwz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qopqdtnd.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2upjhzifl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lxrikenr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2clrvwpxb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xjwxxivs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tqtdnuvi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2fxexznuq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qtmxjyzb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2exenapkp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zusdfcaa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vafoanpg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2orxwcrom.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rzxywpvr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2trqjpuzs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fdpzhjvd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qvfokndz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kjulbkrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfnmemvd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ctpidjan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmgcawkv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2auqksjaf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zfzhmgct.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2odlkcgxt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2qladeoiy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2owvntklu.html


<!-- 参考信息 -->