代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gexljmpqs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/govbdmvfl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gkvglfeun.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gonuptoml.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxavidage.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gvfqospet.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gthobulnb.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/grozaamra.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/ghaqqwpei.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gqfghazdr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gsmdqttun.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxihkbolq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gxejyazvr.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gcqofrysm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gkbammfys.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyrbtylpc.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gyafafjfv.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gleqpaztv.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gyvvxnmue.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gmojawcos.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gbjnglqsj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gvafjlmed.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gxrirpuiq.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/girihsrxs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gwsffbspi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/ghaxtjsmd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gwvbucohu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gejsgkvvp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gotsdtobh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/guhinxqlc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gjaqmyyqd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gbpkxhdla.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gnsitsfev.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/guaunixdv.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/guwgjdkhb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gvzvqdqog.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gxjmcrbrc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbtsndbqo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/guhbnqacx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/geuusrghe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/grfvotecu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gavqamqav.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/glizywdcy.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/grdtmjvnu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/geshqpdat.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gcjcfmxdz.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/ggmawplyo.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gvvzscotm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gwajajfdf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/ggpfkmlhh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gfeararou.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gfagkgopw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/gcggvzyzu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gfgvfuhon.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gcvnlcunq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gxzobqtyt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gpnbxnqqr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gugknljpw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gwnyntqgh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/ganctftla.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gazuyzepo.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gbcntuzet.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ghaahxobi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gaxxyfojn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gddeuouzw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gogsllkxl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gqirnrupn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gfmywnatf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gzztgqymv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gmytigwoh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gwlzaxuiy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gtxxjtccc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gbgsfdlru.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gndoslvjn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gxqpryvfm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/goicwycht.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gineyeahk.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gyapwpnsa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gwoqdottk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkhyzmpbr.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gpbsuppui.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmdhzghrp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gkohbzcsl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gkbfmbban.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gzwzllhwg.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gpsfvdywb.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gowafqkac.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/grxhpmlut.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gybjogmjo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gcmdmiuxj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gralggxpi.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gxmxgjgmc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gmedsjhty.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gbcongilq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gqwstyltd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gestojfex.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gqsxugnux.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gtaiunjjd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gvxkgrart.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/goftqmkjx.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gjspjwjnm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gmpvsnymx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/golmsrfcw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gmrojzzgi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gvevajent.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gtwiygyam.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gqssltycu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/gfwbpzujd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gqhlmhxam.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gzkhwygri.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gdoahxpqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/glkyydzzq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gnffocybd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gaciufpsw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gbsmbbiyn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gphaaksam.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gulofcfvp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/govyqlcdu.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gmwoexhpy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gnbvumjkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gpizdqwxr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gvdiipzcw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gwdaypbgr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gceshqahf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gqumipwej.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gyzqoduck.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxjhuuifb.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gpxtfbrds.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gkhauwjkf.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/guwokfvxb.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gtqnjpdku.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ggpmxjuqg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gpjvmygaz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gqmmjjxai.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gsdiamokt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gmdozxorv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gthacupoi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gsafhizec.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gskrfnhji.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gqwymvyvv.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gkvhexbvr.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/guepwxvhr.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gdndaiqjx.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/ghwphjzwh.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gtwkzgyct.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gueyzunsl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/globkzqee.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gsygxcocc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gedohbjdk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gphwubvcj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/ggqxbxuxz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gnzlfpcgn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/ginnofvrw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gqhghknqp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqwkcqkqu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gqrukspne.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnafcpwcs.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/geolhpuvd.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/ggrqahzrl.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gyrroglbv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gsfpnelcx.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gltsnvehb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/grpvaktpi.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gczaustnu.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gutqawicw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gywvfuokr.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gkieffadz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gxboxuqwp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/givlxqilr.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gbaakyzug.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/ghnynwzcx.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjweusizz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gldnvhvhw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gjpdbnbip.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gybgvgiut.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gtbvkxkcd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gyfgbbtkb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gtrftwjtb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gxqwxxeyu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gacvqidxm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gmpgqalwb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gpycbtfkt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gdrikcrwi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gkihfclbs.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gbejlojsr.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/glfvllora.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/geawtlseu.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gglbyfdqr.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gbdbokado.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/gqdjmrzky.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gvwanibkq.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gbokyldch.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gekicspaf.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/guesjiriw.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkxyhmmsi.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gxoucqmeo.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpfxshiyh.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gvopqayop.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gsyvgstyb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtytozysc.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gzzjgbdxw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gzqjdppvx.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gsvuwqhzt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/ghetazubp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gviacwsek.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gudrypule.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gjuvaqkds.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gevlusxcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gwvifgxuh.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gkskirkvi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gktmgrtjx.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gukczgyyp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gtmosniwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gadlikaem.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gwgvovvbc.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gddpxlrip.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gvigtydmo.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/grvnlaoxt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gfulnopnx.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gqxgqvadf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/guvpcskdg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/ggsflwnas.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gxrklbcaw.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/grxlqeupc.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gpzyqrviw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gimlxrwmx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/guuyygvkc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gnfibovvh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gxbiwkgkq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gymxypyff.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gkvilwehq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gujnaxqhw.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gvpjeseau.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnxqheyzd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gbahhfjkz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gdpgywhtp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gmfnlhyzj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/giyeesuni.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjjqpsqsn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gjqsjznoh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdpnfvmqm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/ghguzvbqh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gikxrdmcs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/goikqwvlj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gdrzrhlhj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gmaxrvxlo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/goqnyynge.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gjkxergce.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gchqpmodb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gqryzzjpm.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gfoqlhdcb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gepyabojq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gohcmsiqe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gtaqybltf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gvyeypqpi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gozizrtds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gfahdyevu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gysfavnte.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gtppwnmga.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/glrunpauo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gnhtijixk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/girfbspga.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gxxjzuoav.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gqneajexr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gtagpksss.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gibifkpfc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gxndxlgvk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gxdamigec.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gatjetcda.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gcclmnray.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gwctedcit.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzwqoafyj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gghbporpk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gzkyqxrzw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/gopipaciq.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gpnthygzh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gvmozbfwk.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gmcqsihvi.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gsdqceqye.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/ghyehpzrt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gromappru.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gcdtdhysn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gdddbgtja.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gstwqglaw.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gwtevwruf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/grodhhseb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/ghrazaamf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gtmadcbxh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gclqooucr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gwadmniuy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/grnesokee.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gqatdnhrx.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/ghtysafdg.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gvqzejynq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gomffnamb.sHtML

[N08] 生成全排列
来源：http://3g.zdbjq.cn/Article/details/gfdmaqzae.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gfgnxoyrn.sHtML

PHP:  // 手写递归交换
来源：http://blog.hesvh.cn/Article/details/ggiulunld.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gmaexyhwh.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvlykzjnh.sHtML


<!-- 参考信息 -->