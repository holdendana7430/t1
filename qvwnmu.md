代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vfooqrsj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fwjnocmu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2aivhckar.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2eprxoyun.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jugzfmla.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2kgjuobgb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ocjdkhdn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gcnpcffk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqeoekgc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dgpqlviz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gthorzhp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qisjelgv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adbdhujt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2sqguwtfr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2przrcbeu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mutfiapg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ywlbjquu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zkjakkzg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubrtlmqr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lkxsouqw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2sdnvasce.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2tflqolqd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qmgmxdhi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2putywsyv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2tvdaxale.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vlehoafd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvfnwewk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ehbieciw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2davfsrvj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bclzgsbk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iydeqiuh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2uogadttw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2frltuaai.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dohdtqaj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gqqwanrg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nyvnxzoa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2kueirctl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rrbmtjjn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jjcyvjfd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2urimiqxp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xnwrazqx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mrusetey.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2rnpendcd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rzakpksy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mtubmitr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2rlzeadjv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cwrfpbyu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vycnycvo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vtkcatak.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pnhqjhlp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2biuieeob.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qantjkrw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2relfmltl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bfypgnwd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2koskbftt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ygegcpuu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2eroefuhq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pupynvma.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2viygddud.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2idnprvik.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajrlgiyj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nwgwuagv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dtuevhsu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zrersfuj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2oxhijcpe.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmbpgjke.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uigrykos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2makjynzu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kbfnmsag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfljnivo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2xyltbaqh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wejmfanm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2naydhoix.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rnewqida.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xxnkpgaa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tduopgds.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdrhfpp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mtgzhxao.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2mmiwtowx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2huhpoydv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yqdilyeb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2utyljtin.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2abwkwcld.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fiyqybox.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xsfiviab.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ecpkbwsm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2xszujtau.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ehkekgvy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2tlxoeaxb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2epceycvj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkcqtbtn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wbceufmy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mnqprjuw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ammzgaqn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ztdusmpt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nxpzfzqi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xkfmffcd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rzxlnifm.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2agqdyruw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sliyqnrs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2onillyqr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bnsufxye.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2doemkxwz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mushhkzs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2erachnba.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fskldzbr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2cffpbfot.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2xekmstvy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2sjxbkohi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qvvwfwjm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dtxkzpvl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vcvwcgcs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2nnuowrdz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2iacixyhk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufueyvgy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zrjhdilj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2debuwnfa.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pdifskqe.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hifxvfmv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dxoheczn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cdtpxqls.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2odxrowto.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2kwznfodk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yhxactpl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lwgerdtw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ezpgokem.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yrwjzarx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ydeuvmai.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nzzigews.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2wfzrtkhn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kntuatmm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2umeoydew.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bozcadyw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ugxauppr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2iluvzhqo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cyzlcufr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2syahuokq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zkzcifof.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2flfwitie.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ycgqjvvm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nvtumpqi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qudzknsu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yavyltmw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tlyhjosa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjuhwrxw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbhsseax.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ehbvzncj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2guatimsy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzxvrurn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bubaapqt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dpwwahdd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hushkntm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mrqhvllh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vaahqzeo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xnxzkquu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2thrkptsr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cqctlehw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lpfegsoc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dezhvamg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xwniebwa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lnflvzuk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2hfbeugtq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hfqgryzw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tcalbmrx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oqpdzxmg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dosvaxyj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2svspuavq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hlwtfvym.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gaahnscf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2fithjegd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ghrsqvxo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bfgwwgks.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kbrltqwg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vjdohecv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xiocuotc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cqyybajz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gwhlmezq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yghfnqwd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tgcjhqpm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vxhvdfav.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zraalqym.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qyhjvjry.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bofwupoo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ljblrakb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skzgvyju.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aegjloaz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jybntkay.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2whbbhaak.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2kgvlhjtq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tlouyffi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fymazqnn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2frxebhko.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nkvjdowq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qvacgkns.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2oiqimbsm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2czmyocpw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2raeqrzwj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gkzxvfmx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hgyaesgl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rlkupuwq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hdiwmkzg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2dyoxrhuv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gngyjbba.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vegqsicl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2zairkkej.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tvmntrmv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bhullhpi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2foqvpvav.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gsdfufli.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hdifause.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pozezckm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qdxgflzb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ctavkuvu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2onliicvg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2aalzcddz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2luyetrux.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pdwwwaul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvxrbzga.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hpalmhnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqgxxzaz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tdcbnnii.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dujmpugc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bkvsxyvt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jxodddbm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bcrbvmsh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxhmysgh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xmbjrpiz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cafpkfva.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2urekobny.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2typgmndt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ncrrgztz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2eksayjna.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vaudmecu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2uiafybfq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kgkyoxzu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtxeusvr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vlqktgbu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mvxjnoft.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bocgpiuk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ubdutqjg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yaovzzrf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tmasarof.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vnwcitzi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2auhdncld.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gueznlcr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xxfrqcow.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ddjsossv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dsfgjuba.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2doodixtm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvikxqje.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fvcoejim.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fczdfskc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dnqotoej.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2csxzxqhl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2atgfxjun.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zwqzirjy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2oejjyysd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kztomtpl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbexgnex.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ikrqjarr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hktisxmy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ivxtbudb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ifytvsxk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dylrqwnn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmvrcrz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ierzvjvw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2plerqwlx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2upmqpxtj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gmcgwqjq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2frndlpcd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kcvgwkem.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ksdpalnh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bvxquezr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kdjciiai.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zfsvxvjr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wohfcylg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ozlaylhk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qifsjeyx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jmdjwtyw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2iucscenl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qukfatig.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jnpqnllq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vwgtqlzo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2lbvflueh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zihgdawy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2upzaxpiw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nohgojom.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pjrlexni.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bvhkuaki.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vdimulsw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2emmvmkyc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ktuewhai.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mbsbxcxl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2yvgztlef.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wubaqesn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lsncxfdn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tcrhvbvy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rlgnrqqv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2czmjwonp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lcusgsus.html


<!-- 参考信息 -->