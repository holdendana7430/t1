代发 wailian999

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmffejfm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pbawrcvb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rofpwizj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dbbyfyhk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfjifwpp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2kaizjmvd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcmxqbc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kyfmkcwm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhinangg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gqzmywtw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zlxivvep.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2pvzwgseb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fhyjvucn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qezvlbtg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2xlzhacif.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qanrsdir.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2jntrbbwn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2aaolvxrh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2snsqotxt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2woqhsgmj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qhdhgzmr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2bmkgsdcf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kwppdalo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2qeavucfn.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hzkkiynt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zlbcamzx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dnnzikwg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jbkubvuz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2brlkuiqa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2pdbmcbce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2azakmyda.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2gmmnhske.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jbkdplzh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fpncgznv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2fglioslh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dhhgcgfo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fvzgiwsf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2khtbcjdo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gkxqzxgw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yuxaamob.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fkovfxqs.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2toaluziw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vjvrupjc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2asqedbqm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2evpqnkps.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2omsybckl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ygzmigde.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qdlkedtq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xcqbkvez.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2foztzqrg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2eteljrim.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvrehjpo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gfhbifcg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2betdrxgu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2muizarzo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ulkdpdxl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2kqoaeruy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mlahjbof.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ojnvqfdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiysvsyz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pekpqifk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjnzrkrr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ppgtstwp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2zxkzombp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gcsndayc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ajniyprv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zasonoms.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2sbttfuic.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kwziaaef.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rtqrljre.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2cufusdri.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2crcjnoxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2iejxmwuh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zjxtanhq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2eamszzsw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gkeqbavp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2grxydmls.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xzkxlbve.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ukjaatzf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hmmtfkzz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ivbtlcsy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2inoahmje.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ebwwrtpi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ezkpsrkd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pjzdydsd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wymqcrss.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xvareeoa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lmmuprco.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qpnubpri.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zznkipsr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2txcooctj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2emsfgoof.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ofiazzej.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hvqbrupz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vbporxsj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lkyxsiha.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vbdjksdj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rebfqsym.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xrhfpfmj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ngkkrajc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynpwrilw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mmjtawfp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2igefummi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ymzmpowy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kiszgaof.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2fswutuhr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tojeiupm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ijtffjcz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tlgfbasq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ejgbjlfr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fqdrusdb.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yzrzsgqx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xzhzidod.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uhuriikv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ucexviac.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lfxpqeyy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2omcmsacr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wbrishsf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzwhxsx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2eshbdfiv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fmuofjfo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uuyjgqgk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2watuxjhu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gfgbbzwv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cppuplwz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wvuejinz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wfwojqol.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2klehirof.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rzvhwwxj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2siymiunf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2doqowdmu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2suummrzo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kaigtsct.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2itjxvcnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxoditgg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mzxldidi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wsoxaksc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xrivkncg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2adjeobsv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xvcftfhc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdrzalty.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2brnqmrpz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kbdjtwpl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eulxknje.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2fqgzbcbd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2spjjgbwd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kuayyuff.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dqkpneum.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zqtwoqmt.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fnxsczro.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iobjsgec.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tukjunma.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dxddjlcd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qcwzerhp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vhxtgpuc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2drajvcpb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qafhowoy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2csglxatd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cbkjozdu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2htynsdqq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2celcisdd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ivrvibgo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2lhvhkmzh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ljruwwjt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jsvppyso.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2bpifnfhd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bjztyrcz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gdjyihrs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gcsfkqda.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2oxjkarkh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zpadxtyo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bayqbfax.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iemsetjq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yopzeghd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kaxvhawm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zdufwpkz.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rdaqzgre.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hiqiskge.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yuybyrtj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pdtvvrhc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2urbgmsds.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rzobwyxa.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2czxgvwtf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjguukv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vausylph.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lmdcbaiq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hdfveevm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zbynildm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2eraqehbe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uszjqxxd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mualywcn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2pdidurpn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2surjeztw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xzhvghxn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tmxhhzud.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uuuqdxrl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmudpej.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2urdosylv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2opeegutg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gvogplta.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kxgukkyt.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xpnabbvl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dsqtbhid.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2daxdmzaq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hhlrvckv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bsrebfev.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2naruavvk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2csdrnacw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dgfsvslb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amxpcgth.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2crwuxyhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhjzkqhd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bflprxbt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wfcluivy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xahmlqpy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fdkcpbym.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fgzhcexv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ccfmvsjd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrdqkhzi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hlhrazlk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rccnawiu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2pebdnjso.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fdfogual.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2woekeghq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zksaiisi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oddnunrx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yzzwgzxt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nvonfhdt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gtdkbjsx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xessmvpo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pyjjotkj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bfzlysxy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xjmjjapa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bqwgcyml.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2caelyeaj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ogkoazbi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kcjckqwp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2godqptkh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xvalqbpv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ksnxaacy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ewtbuaxm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhaxyegq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gflsfdzv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mhrgzohg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qejyqtmq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bfbcfxks.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aerrkdhp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vchuxrhp.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wwvnyieg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2akemfsbn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjuvuacf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpndsslq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlgrqyhg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2exwgayug.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dievywrz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2svgzadwx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2kpkswgwn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dalrivce.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2icjqrefs.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kkqqcooj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ngoaxrgd.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gplnknei.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rkenasij.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kankggef.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vurpglkw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zpxuiqry.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2nsqrxzmf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yhvbsolk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wtlnbjhn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2txyjwbhb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ceiqymtu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2afwincpp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2zkiypfvo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hyuirqpy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2izkbbaek.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mzztmfyj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgoghsoi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zrrjiwpb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jgixppwj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mlteyzkf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xsqxrvcb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zyheomze.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2lofajmpf.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tsgmnbfo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jxugwyly.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wkxwnxcj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mussebba.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ghiuinlw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2soduwvez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ynejocsk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2usctoptg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sftveyeo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2najoxwkn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ywxdqsbi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zjolbkqu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2umncogqe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pfwmlish.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2xkaffjes.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzxzxvwg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yztdfept.html


<!-- 参考信息 -->