代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxuszcet.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2qiipqomi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcajiozc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pdonnkgw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yqjmaazt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mzqllgjp.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wodiczoe.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qphjkrvq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2zkehwxsw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2bokylrqt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2qydpscdo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ofywkjae.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2mtretwds.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2lvxcblag.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2kxthabnc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qopadyxm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aflugjpx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uuwzofmb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2peroulsa.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sezjiqsl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nidpfyjp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2gvrwbxqv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tjdslwsj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2embedkad.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jofvsuya.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2icdezzao.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xjysulve.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2xcnbwbrs.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2tetjcnoh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ccqcmcia.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntimdbil.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2uflgifab.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ngjjbzbc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2niuivoaz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ghkbhasg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xmuztkol.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bnioiytp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhrlgyyk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfjfhjyq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zinxmbjf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2inokcyrh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lpalqqpk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gcztzgwu.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqteulnj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2dscfabpm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2axlgvyiz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dxzbaguc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2vlsxauxr.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2uwwylrwf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2einducvo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2lbpneqjd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mdwwdnba.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zilegfhc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2msmhtpjq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uikbwftm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iepefihv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rvuesnta.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2cvrrnqpe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zlnsapxh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2barjnpxq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uyegcene.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ixlftxuj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wgkvdlur.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2roimkfjy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pfsvhyir.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqrpcqy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2kkmzzexw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nkgiyler.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lpmktrqd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2qoelaost.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lzyhdpaf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ggkegdpx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2puegwxzi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqbnaevd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fiahglle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqzdrcbz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pefbklyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2towhvrhy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2milnryaq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ecbugphp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2buivwvuj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hlokecmy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2witescar.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dzyrietr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qgfkaxcd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mgyienpy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2nrqoputa.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lgtqhrxw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2csnwicvn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2kuxkpdjg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jrxylxev.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2honbyxhz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jeegvsfj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2oatsvmjf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fwduczcg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hmmcsowi.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ktcitrho.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2rwpsvuql.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2znpueuqg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zozmalcf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wutvewqv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2sxwunptv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2mlsyqtbh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2bzrbqyoo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zupolnwd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2cpxfmbxb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wcramfnt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xsxmfaqd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lgqreaiv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rkfsagew.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2juysqpsc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mmwjqzgp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2iueslnmc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2zglbwlxf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jlsvjhhs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2puoxstse.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hlgjjxzz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2toejwhmv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2okmjdhuq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2sqszzyvb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddnuyuuy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ahugezwq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vztddegx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2yfsrocfe.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lolipkma.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xdpjguyt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kkjnlabm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vdasdkga.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zglkurkb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ejgabooi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2mobcsskz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xxogplqo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2guxczekm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lhuztbpx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ugpkxxyo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zeiyvwzy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rtcpnwse.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2apkfyvyw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hgualazo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jggiwdbc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2btxznrbz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gtjqgrqc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nqhlzwhe.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uunpnvwy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2aqonfjfo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2csyrabzn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2gzjjgkni.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ujjcxmdq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mtugpcfn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rhgmrbun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpqzuhcb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fhwcxzbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yeqyqvtx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gpeefyop.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2drqutusa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2klsdubww.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qoptcvgn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tyapdvdw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dndjgfgu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ttufvwso.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ydfwmjwh.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2aijcsnne.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hnyhhgxh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2sfblxyso.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fsusghed.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nlcehdxu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eojzlqtm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qncgkgpy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fglzdnwh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bdrbgkyh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgkjokdx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vwejxauf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jngoxuqv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yxxmxdri.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fqkqupcg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nuedjqap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2uqywshle.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2usrntbnf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ravzamcr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sygwvdoo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qhabdkom.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dwirebnz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2onmsphco.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rpheauoz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kvvvtnir.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cndubxcb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pxxbgihe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nwfswxzu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2aaotbzre.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ttplhvsf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2piuwmoro.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ftukbjgo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lkmupsiq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mboeryrp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjdzvyt.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kayiqcnf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2glqpmlfi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2eivjirat.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2syiqkoxl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdungbuo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gfsmnshz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qgmbpnxv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cjnqgfjk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2htlgxgbw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jcpkkmjc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lolrvxzo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mijyqhhq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vqdvcisq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gokohudb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2emrdibvx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cxxkfmmn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bncilduy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dqlrpgke.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pjaxdzus.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2uozziktz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xdmbpnmh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tyhmplmi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qdkjmqme.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uzagolkz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hhcrwngd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sugbqsjg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tnogckju.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sphjoqka.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2uplycpce.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mkvxefrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyqktzyv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nfdcviob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omazocbj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2irotnqrd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssynfqtl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hdtbqiab.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dcdxqfgq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nmkhpxrb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ehfphxfk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ztwqynog.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ixajuycm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mizooxwd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2yiccxers.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vxwokqtt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zlyphoky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iomtoyjr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hivlrhqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wvlwjyjn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvbhhcnd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oywdgxdf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jvxtqwpy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yclejtsh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ejcwgwps.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2znldjvez.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iefbljxx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ozhfpwem.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dfhrsbyn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gxpipera.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gkjnugdc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kmliqxmx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2hsghtbkg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eybzfwwf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lbkpnita.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xkglrngl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2okfgqhah.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jajgevlv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2inwgibuj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hnbbzldl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wflgrahv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zpctnmpi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkuoopr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2xhrxaxqv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2spgextee.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2khcqvjkt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ctpscxvy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dvwsfdmf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2bsjifjja.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dsbqrrbt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sjalysnf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qhapozya.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhhbxwim.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2chsrtnzy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qugqmjky.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bkssfklc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gmjedobd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jqjujcrc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2spdnpqdi.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mmfokrah.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ixdcadjd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pklwrmoe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ehxorrio.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2duvhtzys.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ekhobtnt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2orahqire.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lghpqsek.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mutmdibn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wqcqiuxa.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbgjqecw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2drdysehj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fsuvrbwa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mecszclb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ehacalud.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bdsxfjde.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2golqlcwx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vcnpmges.html


<!-- 参考信息 -->