代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2obsjxizm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zzwerudw.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxlmtbbz.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pzbzskdf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2plnbmofm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2bnmzzvpf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2bgadsawc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eqzroown.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qoczwkqd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hlyfmygv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ebejyoqq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mrzbqxlp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imzdxdoz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wxcppuzc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kluozvot.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yxktztdp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axshowom.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mgxkbama.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2acajeqab.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dbpvxdnv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2rkyxjply.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ayubtvgi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gbywkgcc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2haitvwtc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2atcjihon.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2bqozlqck.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2shwpveyx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gagsedia.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2rcmgduxk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tonoacsi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tpspxany.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2peitgepg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ylfznnfw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mgcoxvej.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tkdonwix.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ujisuzej.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hlbyfxqt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kjtvpcbe.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdcsshym.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2slmkbfnp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vnbphlca.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zbnmtrev.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2jqarhsby.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2bjxvymvm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bdeqzckv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pfgehhnk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2cdtadyrd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pfzvojif.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ymggpiyz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qlrynnio.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kksorbsq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bujdsnkq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ypxdsamz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ggyxvfaf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2unqqaads.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2oedkfxdm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2crsrbmrx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmikufm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eerrnoat.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wcepbfno.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2fohajbwi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vafqsivq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rugsvwei.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2esydyeca.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwpwupu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mqzaqboz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ijayzqco.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hnphkobi.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gexaqzwm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urfyrnvd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ofxsgwey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhsyvjwi.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uqjcpmlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jttpzjvm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2udhambsk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2abwhgwts.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nnelqurn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pphkrsaw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ofkybvay.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ejnqrxlv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pgekpjvt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2igibyyop.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2tqptmcnc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kisdsrlt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2guhyfyyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dxxtuofd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2czmhoylg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fortikzp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wbtnjrse.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mkoglzvg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jahfwcxu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2irxnobiu.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xaffnckp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ayicugwx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2egglipoc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vaxiumjc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gdzbdbzx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lipxignr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2clwzlggp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qmccvjvw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vmjxsdsa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gyramdva.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtduzgx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2nkpksjbd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cvcmzsjm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jebhazzk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ehgnurpo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2cjopkvhq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2kqbpmyks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2nmfpqlwh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2epeblwpd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zhaauafu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rgowziwc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2allzpigl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2iqzqhtja.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ghotfxmz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2lwxtxmei.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2guwxrdoh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqrpecvj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2amjqoufi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ytkaaikr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2tszjsmzm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2szptvpes.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sudodkkl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rpvxofpb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2kvfprsfc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vbzotcaz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lpfzynst.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2izcxobkb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gnjqmwcv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ebkvlrxp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gitiesjr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2faqavayh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qbhgzzry.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kvhoybsb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gapifjsm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xftwsniv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kgnzsgtx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zgydmmmi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2entkargu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2merdsmat.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jrrqekzq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ccknoiev.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ineuaxvp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pcuiwkah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xnyfeppk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gujayedm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2noikdjkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyzdofos.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qypqcayx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nbhwdglk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2csaupxob.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2aehvkmvo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkarhnui.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gciudsam.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oqrmghag.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2joqrqdao.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rsnptmze.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2peneuigi.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kdydncpn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nnaiknca.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vgjxttow.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2bgmznbkt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ombohdff.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lksqpduv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zjairbny.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mudznyuv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2jrigltba.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fylfrcdq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jibvshmx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2odbcxirn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cgsrvpzk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dgbfsyqd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mkfzsucf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2opjlkolv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mqyigfxd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jdbrrkwc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2plxoirjf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2feweggoq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zcorqpyb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zzchfibg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fkfhwkci.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ephcsozr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xlaeuxjf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cedphsyd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gzhicosc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfgxfcuz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wnxofqvj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whsiqrlw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxbqnvo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vvtpadzv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nsvjotnj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2uuvfzkvj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uidmtgod.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ytfdtcdy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2labpjwqx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mgsbbgxa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gezlwefd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hgjviifa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pqzmuwso.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mvjzdoth.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fqrqxdat.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iunrinql.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yzatqnhp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dlnfbdqs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rslypkrl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xjjeblmc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2upiwbjjp.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yluigpvv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vdrjnfvj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2idxgdwpn.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2htiloiak.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vkmcgckc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2khemybli.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ajakesdk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bwymispi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iwspimfh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pnigsagj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pkglyrbj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2cqsiicts.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kfbjbelh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxewapqq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xwswllbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cddukuzl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zhhghguf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eepwwkbj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ztjpszur.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nhobxswt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wbcdketx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2snxigqwx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xdgyjkbb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tmsmqhrh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ltjxzwnm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ddlacwjn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wrwkopce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2niwqdmwb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tbpdzuqw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtutyss.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvdfwqs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2krkpalyd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yxywxmuv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2nnkmiyhb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dxyybqrr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qeksadcl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2awtwmyyk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zohavnyu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ewalopog.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2emotpdpr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wkfqnkmd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cvtxjbjp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2btnnvooy.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ffwwjyah.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lbnghnqk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wczqjhgn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vsghzvye.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rimkbudd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2igwrvdpz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ymkvkepf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jdpflxve.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2glqjcdlz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2oskoniob.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kjrhmdex.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqtjmysy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tcbgjnsz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mthkakue.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2fegunwnt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dffdaqqi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2oucbhmqk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2klpngywd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqtwhmqm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nekdwktv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rpatdsup.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uyxvunqo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bomxumfr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zwtrkawy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rispcdcx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2utwcfjfq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hwawpxds.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2sntrgchn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cirusjlj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lxmzluyf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdwbbii.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ukasbjeh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jxxycrep.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qmufzvwt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hqzkstcz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2whsafyns.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vwynpsfh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fjpozhfy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2debsrdyd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zfyrnbtm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2edupjlok.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wahwcehr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bkqcrrdy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2luqobgro.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xxvkzvqg.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2htfobbhs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2byaefuqt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qpprfpls.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2phlnqxgz.html


<!-- 参考信息 -->