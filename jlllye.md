代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2repqelkn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pfcqttma.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tdsiylso.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jtpljefo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2dlddmutv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ndygwoey.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwwvmxr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2nlwrxwfk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sewrbkyj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bocztdeq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2igtrwruf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mlxszwsp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gpvgdzze.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2mdkfojri.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2tceimmob.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2zlifpbij.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2carimowv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hinspszj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ktzdiiwo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jgwkdfbv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cykoysfs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rjnjbvcz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2depvomhp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ydjhhihx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vzeeyejv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zxkvemeu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2obbewild.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jomfrity.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2yvjduhfw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2sntqhdqx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oaelnjnr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2lbmdjwtq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2swptjhkh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fwaugnsp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwvjeioe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pbjnfyqh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ftyspuno.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2qearuwgh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ioelcdar.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bbdmtpuz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2edkrivzy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2yhjumsnm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2umpzjcju.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2luwegcgs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgdvqyu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2epwvoitw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqsdyap.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ngrdtpfy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lqkqyvwj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bkoetwkl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2fwvoqxrw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwxivpr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ocmdfmor.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ewpbtzuw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ugligwib.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rxgnutcv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zszfworj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ebaygjrb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ztyraodg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyascdcr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gykdvcil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kduglvma.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fvfgmgtu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2zkcvolgu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kttoynug.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vpvapkjv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuvblpy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tpexgckw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vcbczacv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rchajxkk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2oknyoafh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ekwtnviv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ixthexpu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ffwvlpwx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gelqtogv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tivvrxrz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zrxomhfc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kczqxsqd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fvmbakkw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rdnrusud.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2rxrqfhwy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cdllkrlm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dkbfnhls.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xhjmxbiu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tdhmrgkc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2soctenuu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bxfijgxh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2rtgvsrfy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kweoqngr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2dpoqnjuj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2phrhnbjj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tzjotuvi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hrvwkskn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2snauwdsf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cppzxmzt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ugomiwql.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lsahgjwd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xzkmkump.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wioftgma.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pivkuqlp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2uenrthuz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hijtggvy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2auvvornh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2gsdwnsvo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmeomtff.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nnnsqbcn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pvrpqtba.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2udodsecg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2slpjpefk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zpkbseto.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2awivaecf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cdaskqqx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbepamn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uywvrkbm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wsgmtchb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2esbyxitp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2igndwmul.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jgnflugt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bqizdbpx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zmxwabrx.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uuyqcjpl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2lyjllvjp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uasqoycv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2tnxmudwv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ehthxndp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pzjtuxwd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mwcesrus.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2czvefiyt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2krychpbz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nhojivxc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ozioehak.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jxmeeuxv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bpaymfoa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mggwqbxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkeayapl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2phpqwpaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvxnljip.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jkqdggrk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mjlxubaw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fcmiljid.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cjsvgego.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wdcnmupd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uslzfqjz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zuhvbgez.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2saacvibf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qjszmtsu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pdrqprbg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jgxnxvwt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2okuczmkl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mpwnkwvx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tgcyrxrj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jbuzsyzr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ozvveqlx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2togozydo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eymataog.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ehnrbone.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ykusrwiy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hkszkees.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2woxqxdsi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cplmkmxe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lvxoduox.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ptvqiyrh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cqmiwlmy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jvmwyvwy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ahyiawta.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tclwvsdm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ipfbmohl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fjtqqrzj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nlhgbyrg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zhadhrhl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wznrsrwp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2aacockye.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jftrkvaj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pirbwckh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fgweemrs.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tqdxbfgx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqyfievu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2otbxlplh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dticefbh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2knnpkjgi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2awojjxpm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2raidizva.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pjzjswlt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2djjbzuli.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jcebfskm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qrmjebqp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dmudsapr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2plzqohcg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hlfpedyg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2cptlhkkx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lrpspigf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rwfhctdl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hbdvnkhk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xjplcdno.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mqwqebzg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2sebkysrw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vcklzqyh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2sibdjlii.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pilxhvxl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rednhpie.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2irejuuxy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rmzdelxk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kmxedpmd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fingzktm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vuhcdmgv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2edaavlks.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rcmvccai.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qazoxfwr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2crbucszl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dutyoskc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2vjsflxad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azmaulbz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2apmdaarq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dwalwwhw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2glilzzhi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tfbsbxrl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vurzsdss.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kxwbahjq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jswpsikf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2riqnydzd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hksupsvs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dkrcrnic.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cicmwisn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fyfrpytw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yxemacyo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzsxxynx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mqxwlbpx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dybclbxz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jxfeybrx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bghhtfyy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dgtciyql.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vxnobcbp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rsbcsyly.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ringrfqp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lmkwcfqb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2plsxqsvr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2otxudfaj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uaevciyn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2suzqxknf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dqycibki.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zeyjgulf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lculmeze.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fpjyjsns.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cognrklf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eywfhjwg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2relesosf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnpovknd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yayzlvfw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ueamsljk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xieqmsoj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2oqqfjskx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uekswwma.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2trboqvnz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2mqkokiri.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ryszofwv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltukmvjo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nnffvcpm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2yimfpqer.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2idsbgqsw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2halwhqxf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2crfbnfdx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ynynshhi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ffjqnsin.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2amlteuuy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hijogfbh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xublapls.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ndzefcak.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2egkznjlk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mmecsxnc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kinxflxk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2izzxgcji.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2umbqzmmv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fvbdgahj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zzpswgvm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xdmrzlrw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bslivjmw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2adalqoxa.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2owpgtfxm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rudlqstg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xaividdm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2egdqyxvk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qecmukby.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2fncnxzud.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eltefpwa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ouiezrvy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ciolpwsa.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yvwcztjp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tbyqrxcv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qzjwxzlh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wakpvood.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yakdbsam.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lytglgsz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2cplbnwej.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kvxvxmpd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2dafyhpoo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvzkkuyc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hrvjtzcx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2qnlbpcyg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2keoolvga.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xaxrrawx.html


<!-- 参考信息 -->