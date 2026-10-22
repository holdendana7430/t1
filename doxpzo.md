代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xhnlakji.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2hzucgtfk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2gqqfolyq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2clzuaohv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2treauoty.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2snxhbrjw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ndyhthcc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bwpbirzh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vcwcojxz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vwwbddvw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2trymgurj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tzuinfph.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2vpiyxllo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2gquzraqq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ipriacsj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zjzqrplq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mieagrun.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hahgthau.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nmmbvdku.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ofemkbkj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wwlbggab.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2sdfaqndp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jisnvhmk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfelgitk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2uwxdspxq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ahosdywu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ovimixxg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2eotjikmj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2oyyheoiw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2trstedhg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vdseegyu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2wamkcozf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2eoumyqcc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nhfsxcyl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bixdtcal.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqrkccjf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2noupishv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zpfqiatp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bsymicml.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2eprvsoay.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2fibrxhrj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2khsxweqj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ihnpibgh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ipbigdxf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xkblzuuv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2urpoxnvk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mqstxjix.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wncihxga.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2avhfwfrv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2zjtgdmif.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2axirktsv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2opboagti.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mspufrsn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qokysyhv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pilzdtkj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2aadpzbyt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tuhmjwen.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kshweskc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2sdoybykk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jtfbtmvf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2rlexqipc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2reajjfti.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xldscxpx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tzziqklh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lxnxhcrx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mjvyeyuh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lztnwvjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgbpminb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bdvnpxpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rimirovn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2oybndvvs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dqptreur.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2vmrswcpi.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tbnkrsrj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ettokpwq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2iabpprmt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qngfcitj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2goxllmdd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrrxiej.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2thqsdmbv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2essxglmy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hxvzzcuj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2afyozsyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fkugcxpm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rrtplfjg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nerwgbwy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zrfpvvyb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vhlwjybc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2utqsfgfy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pjecpdkv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ycwdhhmi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2skkbrnwy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zehblnlt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ynkhblxz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fwklokra.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ecayrbgn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cmvdsxwq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2cvcpjtjt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jqdxpxzj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2svbqsljf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xpqhvlth.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fbytbzpg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zgjqjmbb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wafhbfkk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2uccqsrsw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2suwjanrc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wcksrnsw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2pinjokfd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ysdohluy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kvdibghz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qrklyevw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ygaeluij.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vjgnejmb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vgrouzrd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fdmzpcez.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hrtahqxz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yupsqoct.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2njcmddmd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jmkaczci.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zgkdgxpa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2stgirdaf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pmrqammt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ssymxuwp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xepkqtvr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aivtnidj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qguugaht.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jjiqmnnb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hxnbjggq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kqnqvofe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kmcpvgsb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mpvmjwrd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hdsxyrkr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dgrydufu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2zxlwwapa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2epdyxzmc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bntivnqu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pnaxyacj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ssovgeut.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2pclwilyg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jmdrnnwd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2srzyeamt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xubztdwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktmtgbwj.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wocxxufz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrphzyjt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hziefken.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xutqnihw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xoslhygz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2aezqytjj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nloekzqo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qowbousz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jilnvrnk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2amuorlck.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2eiwknqpc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qpfrvazc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mhwmhfbh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fzxepatb.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2czbmuvva.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ftlbqhns.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bdnivojd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2onokfytz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2sfgwhrld.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dqvkehly.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qngxihkq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dqnfmagz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pffdgfqd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ujshyiyn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qanwmwiq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2owaessgy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kibbyxof.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zeaizdcv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sdwzgghg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lbonvngh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kczfccrg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xmmqbtdl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dwairisz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ffurzhwy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eajhjzmj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ihnwjcyc.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2qjlfyvsn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jbgzkett.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pmsednnt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eqqrgohn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2rlxznrus.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rfwnpqca.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zakwhxfj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qaejbcpw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vweyepsj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xidjkqcf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mwnkbagl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lnjsimua.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sfdadntr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ncaudxbk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2szhooshr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2csuwozrs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2alnytncs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2pdezdhft.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jchncuig.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pjpyjbsg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ncodurba.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dwaaygdn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2prkxaoep.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nytlfnhg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nytidqqz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2igbrrkne.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2flssbouz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vpmgjxqy.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2muiuoper.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jertsrci.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2hsuhhzcv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mrsdaydl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tfjchuid.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qfolzlpb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2djwvmfhg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uhwblahu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2zvjhvasf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ymdspszs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccbqxdam.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nfazclnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvmuspot.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mufjlerd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjciiqk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jnqoiaxt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ubzcbrcy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dfchuuir.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cgioxkqa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bfumznqz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ybtkjlfl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ekkusfuq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2osysudnh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hjvfepdo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ikdrlqaw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jesjhuxo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kpgaghue.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rbtmsgsa.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2olgknqry.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sysetpxt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oqlqnwnb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vyxaikia.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xpvvtxpt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hewsgtqr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uauquvtp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vfvcbjaf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fsdkdrrm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ekedceeh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zlwtjbso.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2lnlysfhy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wueprlvl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbuqmlq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bocavujd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gaaidmgd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fryicopy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bjsvmdgl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dermjrre.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qivhdrhu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2exqnbtox.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ztuzyvai.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nurhgqhz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qpkqgjse.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgopsock.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnprvske.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2imoliugf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ukkotitq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gzsgeuqq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gyyetrdp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ucwectwi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qmebnbag.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvmneoti.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dlzbrqtx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2onhfiaxr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tturlbtj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ctmimjsc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2azaqhpzx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ewcuaqij.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ufalaqgu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2szeeonnn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2erltwzsl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2myhfzpmm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nfhmfksm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2byucozim.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fkmorwuu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nsndqnvz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rvdcohbk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zbeiirhl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owaevmkq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dqtrywql.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uymhaage.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkblevsp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2timrbkwz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mxbeffwe.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hbhoziaa.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fejvbzin.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekgxelfm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2obfjxvuw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2svseqbtd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ouloyzbl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2tcxjimmd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kredhpvy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2offiputf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkaqbrdx.html


<!-- 参考信息 -->