代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2adzfepnk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lahwtnxr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2iinsgbef.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ripgtmji.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vhllnqwh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wssvxmek.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gcdibxlw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ldchkurc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eriqlffw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2bnojabfo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nooeryjw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jopdxrfa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gtamwsdb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2sgdkbxai.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qvhwsizs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2wrjvmuqx.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2vtzpgnwq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ldflczys.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ludqnrsn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2esypnygd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lxsmeryv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2csupsdnr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zigevgaz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kfcjoayf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ghkodklc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cbcimojt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxpmfrh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2icpyyfrd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tuierceq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ytzezcdm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rescqotq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2oesiivlq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ptqxvrzz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gjbzzsgp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fmdomwud.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2tvtnfods.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ottuxigf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ovylqfas.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2thvmldbe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2otezvqgv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2okuagzip.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uwegkdzi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dbjhijtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crinzeso.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gfoccuzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxeupaoo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2btouaunu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2vvfwackj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lbuqgrsz.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mydtyzzt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2elvidquq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2msiqtvys.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cmyjmhle.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2dxqwnykr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2eczsswlj.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wksexugb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eelbgiqi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rvqkinti.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2csaofirx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yfstaowa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2tawueyqo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vhlpydkq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2skbldhvu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jtsfxged.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jaugvqoa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cznuwvfx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qdvdfncy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kjtoartg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nivoqiqj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2trakfzmr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xcjrrcym.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nishpusi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pqoytavy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2vnlfrdts.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2lekfrwaw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2mpaycvlv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cjdcucmy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lpwsingd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rbeauyru.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zkwobwov.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2flptwtfc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wmpowxjj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ffatbpcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2htnxpwkw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2pdstcxce.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zjchnggs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fxoqxyxd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xxhyeatn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2qtqndxok.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xzekazam.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kvyjlqmi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2uwhlyapz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lkkvpxjb.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zeaqayse.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cyceqnfv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ihejujuo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yakgmaav.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pjyshgho.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wtdmdkhn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wiaqxpwg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fjetqrvl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2sgvkcdoa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2usicktat.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pmjwtwjp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2widbbwym.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ekeecsxh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ptdzuxmy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qysuodme.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zyjluvef.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iyowqfeb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2zslfcqaj.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ofodajsn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lezpacns.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2galoftpq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fpzqtnij.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ejceovyj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kbnjuuvo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pfgoahxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdkbcshw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2enpuyyrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gfdskqut.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hwsamjso.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ysehqnfv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ojkrrzmu.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2reucvbui.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bcfbtudi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ntslfvyg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2odisqysr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2znigvfxa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fqtlmgmt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2biqpbcas.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tbtdokpy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2txovhiby.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gthiyyja.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qreqoema.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lojluvnd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yfdiehnp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2petgrlxz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yvuzqojr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ojktwgai.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yctijndk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gsbrwzgy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lhzjrwxz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fevgewvy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pitreovl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gycssolq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bmzrlmps.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2cdvmduyi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2buszgxrt.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mkcrahfk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vmuyuswf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2orzyutoq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yckincei.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2njszwbsv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ctobhghe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uyvoqlkk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mbaidnpz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2eqbxovvf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdijmhi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ikdudiye.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2adavgtaa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zsydgjse.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2frkelyra.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmkzhhx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2txhvfqdf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xoylssto.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ygnmcbbj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lqbycvfi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pfhfbpph.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dfxljnyb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mrfpqfza.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qetrbnlx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jenszbaf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2urmwrfxv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wzacsukq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2yebrjuaw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xifunrrf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2bxeornte.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2imrqwpzt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ivylwqps.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nximxmnl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tecnbmcl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ingtxblv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cuqbqzxt.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nnfpqzxc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vqxbogcq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2nwynftst.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ghemppch.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dgnjzttt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xtpsqshk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vthfvavd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2emtbagee.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pqnvoero.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pstksuhv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vexqeqca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvhtmfek.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tscnigsf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlidtgrt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aanvobtq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vpgrevmu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qfammtkd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zdkgfqvy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hbwudwdz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2oiqyhuki.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zocanech.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fflpvdrx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ivenzbco.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bkamonzm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xsexvywv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmsjqtuq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2clopeein.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2efdwxhsp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2flvvqken.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2axhgfygx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2eehsyghm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ycndwriy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ppjwxsmd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mjzpuefn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2afsvyzws.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fuiddsbs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mstydqor.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wdahtfms.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2opbywejr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2uubcnhdd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2isoiwrsv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdmovgz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2burzyhgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jbzgmygc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgaijxya.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qtlrkzgp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdwcaff.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ptggmsjo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2vhaoecsg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ajqeuqze.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xuwqlthh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nretddvu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ozrnujgf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rmiagkzw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hpjzqlmi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2mrlfkkql.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2iywsdnet.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cgohurce.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qnhqxaot.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rnjuvfbo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbzztpgq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2evswbdjn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2djkwhekc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2apoezyti.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cddzxfqm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xqlnmzpa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2orrakgmh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bighihhs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2etqydice.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ireiwyjp.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2oboogyil.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2kkpaxqbd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2dvcexfxo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2taaxmhrn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2skorvhvl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2oahkwtbz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vntizpih.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dvajasvi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yfifbpwu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kolutakm.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2quisqsht.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rkdwxjiq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jcayzaox.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wctyfxgk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gdxftvvn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2sfemypfn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ewewmril.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ctjtpbxg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zrczgsls.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2uvecllmy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vluljxcx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2awcmmzzc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qfrfwyyp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eraxzjly.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2sbysqntb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyhfrwao.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2abnivvgc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2oellocgg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgsarrlu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hubjzrbj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vuawkxfo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2enoesmek.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gpajuzoz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lyrvfqyl.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ltriylpe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dyqjnkdb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wbktthjg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mauzfkjw.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2alrngjmx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2khtyairh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zscfdomh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tuzxcavs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dmarxdyk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kwwbphdr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xflnnmpv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xaozimgw.html


<!-- 参考信息 -->