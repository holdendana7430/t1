代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkqyfgjc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2piineopc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2teeffrgj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2qpebmnzl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhdwlolw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2otxtnjhs.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2dmigymee.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2euhtbwiy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ejsnails.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dmnlklpl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2txwuehio.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2scsiejvw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gfxclktp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yutphija.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qrpxpexl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2waohzzom.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ffgkvrcr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2buiunmip.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuaimzr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ofyjqrlv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ufmobbeo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2iphhhgmm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mwkuujoj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nogipcuj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kpdxfxkr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2edtsvwio.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2lqaytgsx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oowzsjlx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gpamaebf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ydkilbxp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2blxlsbfc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kjssfaqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qfaidzxg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cnmscfou.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2owtecvjx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wbujtsih.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aypxbtdy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2npmelrtj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2myabaisa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvuptyi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2bdbtuhwv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzizrpa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vhyropvu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rwkeuats.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ylxqouil.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gtwutsvm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2njmoptas.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ebsylrdh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2qbiawaap.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bdingaqu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2poydktsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nscarnqc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2grjspmoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dofonpij.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2trvqnfjd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2jkwwqzhn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zcitgpqw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vdggyfgs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jemgqiwg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2kfexrgdx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cjzkxoeq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mwoapcpp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fbkcjyza.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pkydavby.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jaeyknjs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2tdlhejro.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zxcpvpbt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aavyfofq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2icfuobaa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2fdzxrqrw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zaoxpoxy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ivrqaznc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2cplymhim.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dnqfxuhz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dxtuyijf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gvtjweiv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nlyftjnl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jtiekfgz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nnzfwiue.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2uwlzqork.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yomqrjyp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dqykdciw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bbdwqxgy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wbmcwqzg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gxgfoyfq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2biuwxjno.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2faevyhqx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ztvievak.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2wklktroz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qhcnlkkd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2topunrcv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tbktisbv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2skkbbskx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pkfscgvr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qqplffvi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hxhreivd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgnnfjsp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ntuqpbpz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlnrfwhj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wkssvlbg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jgrzifyd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2viwcypbs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xohcwwgz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pgappxdn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mackwbcq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wanhknzo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2vadrnqoq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2hspktbyq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2coruwvuh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vnionmcb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bquvtvpt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qtqeemln.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kgjulirv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2puctetvg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tbqbmwdg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jqfrefkg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2stxsipma.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qacaagyp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2sjuyckce.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mbanmkiz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ylbmzfxp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zortflqs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gapeyiix.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gpszvzcu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ixgzeyjl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mxhohred.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufuqnrre.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ggefcvxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjoiqwcb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gfdoxkpe.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rlxicsyr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2uqirhnmr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2osnnjkty.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2saupfnwy.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2felmbmru.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hacrdqnx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fhonhfqd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2segyvjcy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rtvqeaan.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yezzmpbz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mqpsimqv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yzxeyjxt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2milddvrh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vmcigctb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jplxkapx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ayathadc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gmajvgdf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gfhakrza.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tqdeacpt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wwttaydj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sxarnrcd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dxkkffjl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tuirkrup.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lnliljtj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qwrdcbpg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2wcwcmctb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hfvzfhxc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kqslfexh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ixzjfcha.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ryoxtbsb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rccqdtlt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2sflcviqv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rmsvrldc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hmeypxdw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2movucpsn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xqrnttvo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2npfixpia.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mewmupxu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vyvowgmt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dswikopj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2swshslxp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vdyvjypz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nyailmkf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2juxoffvr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dqtdduce.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bwkerfgj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uihjfhzq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hmoqqxmn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vzwjufwp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fdbptivh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ajksfjgj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ntdosbqo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ocschfwe.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uxeoalph.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2damtekti.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mktpiflg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dmocisqq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xkyfvfab.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nqmzahqi.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qagnsyse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tfnhkdzj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zuedcgpj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ziewzzjt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2feedhcub.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xovrlbjk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wkchmjzz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oigsxtwa.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2epwxaldf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kblnyzbv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rikoqwvn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2luiyrind.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgjgvmku.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jzcunawl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crmwwmkb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tkxtjbqb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dxvtwfyy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wpjqtads.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rnxzfbpy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lzqlezyt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2osofwhtz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqjaegdz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hyttrdsc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2itrcerbe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2retutiis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ejicdeec.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rzagtjni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndocasjn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sjhbcuwe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dtiffxnw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2flkknzjg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eujhfnlk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qjzzvebc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rdytirfv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ualixupo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gzuuvlwt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2awftzvmo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fzabhcta.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2lrcwcphy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2dcrldrwj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jlynaegu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2aewkmrsy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2uiruehlx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xycqmprt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgoztfiy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ktdrwvcu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pkynykqv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uepfzdcj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mxfuzkja.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bghcjgon.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dnlihcve.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2sjkwzvzn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oltyuban.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fijctynk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wdirgruh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2epqihzcv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zfivbfiz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dsargqmq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2eiebcots.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ejddnleh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xlajkxqm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wgzpwoca.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2silaufur.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uhorgosv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hkamdgmz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wjezstxf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pobsqfri.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2niexnboq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gcralodz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kglmkgmk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jyifgvtg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2lhhwbbjn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vdcgcwsf.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nbpuxfmi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wnvqdgcu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cgtssvry.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gyylaodg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uqfhorcq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2dbdyjasa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dtnewful.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hdshsunc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2frtevmye.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bcqeeaoe.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gfcveujg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dhljrugc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eilcarnf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kwttgyug.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zbmcwsnd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ttymqtvg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nkuwtonx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2keckxfqr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dtznhrsz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jldjvncs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bzfvqddi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tvcyhtjt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ecimcpbr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2pxpoafrv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xqkvwbve.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lgntfteg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wietsedv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2waljhqnz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lotiqucz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2bhqnmavt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwrtfqp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuojzsnh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zitcbscq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2upnousqw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uciwnxxl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qhodkpel.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sfuqjzht.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sfsedtmh.html


<!-- 参考信息 -->