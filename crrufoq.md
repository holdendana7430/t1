代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gexipxkxi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/getyhgxxo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gnkgpohtw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdrdagjbh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gysychngy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gpspghkdk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gtgumlqqm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gzmozngcr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfezavfdk.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gbxanowcq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guzyrcojg.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gqxplnnzu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gkgpgjutc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gtcskphbg.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gmdfimvfh.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gsgidvxgt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gmzdqaxoz.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsehxqog.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gexooijtg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtajevrjg.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gswsqkilq.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gtsnfjhkg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gmyjxmxbd.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/geasyhfyy.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gumtokpko.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gqprrbqbt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gqfcoxrac.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gefqawhfd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/ggbxetqcs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gyckstpws.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gcvjoiwju.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gefpcekty.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gyyalxqim.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gsgfpgqnf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/glthgcbvy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gmliyywxd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqgvhishc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gtnjosmwa.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gpltzykml.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gnjlolugs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gxfqapxdk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gxwgqfzlx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzznhoezz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gmaxggdpb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gktwynvpg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gotumvwyz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/gjsyxiqde.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gkxztzyro.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gbtpcekjf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/guofkowrz.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gagontoqv.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghcadptpw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/glxhestuz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gjtsptets.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gjltuwhnp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gefqplitl.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gxmkjcrqq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gmbvtmecb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gnzsjuxaw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gswnypjfb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gnywylxqv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gosjvhzkc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/grrnlozhd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gnhvmevjb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gitpidaxh.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gambcpmjw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gwxktefux.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gihzapjpz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gpojzcrws.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/glgsfuhhz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzlyofrkb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gxfgfgstw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gpcsoiarl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gpryfcape.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gapxoeffk.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gszanjnoc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmupiemtf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gdenvalae.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/glytvwwwr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gstcpnhly.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gxhhetfrs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnhtjdprk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gzaautxrq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/geaxblhkv.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/guivpxoll.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjifqljmy.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gmwddsslv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gxhvrlvfd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gsyrzzjlr.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gxrpnyaam.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/grukrcnob.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gygrdhjqm.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gzvkonqus.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/grxzpjhrr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gltkgzimc.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/goclrixgd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gbhzcpyhg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gthlznqqw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gnwikkfeb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gqnoftduc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gijfjeklu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gwfcrjzem.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gusmrqzcl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/ghengvxqa.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gsoaarqau.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gtggbodla.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/ghugkjeny.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gwnazvjjf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gobuccecr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gnewilpze.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gawjqwock.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/geiutrwfy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gpzebnpvy.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/guqvrhpty.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gdqjfvaco.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/girpokefe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gnldnnkik.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gdwllkvfq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gaxjbigik.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gdrmrnfii.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gifrbevlu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/grikhqaoy.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gvnajvjox.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gwxmpxdrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gbghcftsr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gsetpnxjf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/grfoqvhrw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gkantqsit.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gvvobkefg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gpoeegejo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfnldoxmu.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gjveyudth.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gaayyzegc.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gckhibcpt.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gknqyfqyo.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gxcnkmcga.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gjidtiauo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gkouopnjm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gjzewsbqc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/guaujdvqd.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gdynbetvj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gcyiggdyy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gqztbaiuf.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gzfqeusss.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gdcwjqlsg.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gktufijgs.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/griotouju.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gikpomknc.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gfoefuhel.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/grwlxxpsp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/girkuswlb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/ghrqqbtss.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/garuceadc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gdjoculhd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/ghxzqojed.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gvupwjofx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gwiienvkz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/ghufvzhjb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaamnzlzv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gzymojcls.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghmngqsfp.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvcypzpnn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggqqbsyrq.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gmhhtnvzj.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gweytpeex.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gxddkwqxy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gyanpcilb.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gvnfkqvkf.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gfqucnspu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gwpblfcum.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gcwykvqdn.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/girqecghx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gfcdkyogk.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gumcqstin.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gtzncjqrr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqyxzea.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gltaratmm.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/geovzuwyl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gbpqkhhmn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gbdeayjcp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gyoxihymo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gmuhbuuor.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gxfoitfqi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gwztwkipc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gdlvcrhck.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gizvmctmx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gamjnrpck.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/gqcdvxagi.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gamfeuwyc.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gjdnhupzy.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gmgrloans.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gmrtnavll.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gjnczogie.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gdsshyprp.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gznhrndul.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gtdymavdx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gtmdkgltc.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gkofpklgt.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gvzixjltj.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gjnwbmeut.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvijrlxew.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnpflgdgm.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbgfdqdum.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gucirpocs.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gtwmpdcyk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gdfjkccfy.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gsbqoxhiv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/grpxmqkun.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gbmsxrigl.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gtsercdek.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gsnwijygm.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gnecpbxgn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gxfqlvocn.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gnvidpdqw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ghyrxelri.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/ggctspbui.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gftdgxstu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/ggtlupzes.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gzasdyvcn.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gtoriafzl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gktjwueom.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gwaktsttv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gvfghvfdc.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gdddnwdir.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/giubuvxty.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/givhqzgcd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gaerfgcjh.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gbdfpmipi.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grhrvjgbq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gwcwnqrjj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gonplrrgq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/ggfhkryeo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gaomxfxjo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdzwaiuda.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/glfjahwbq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggpvcziur.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/geqpqogrj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gkurijaqe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gxihoqpyl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ginrpouqj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gixuybnjp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gghjebnsn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/givgnhxfd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gjwshazpn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/guelgljdl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gtexqadgp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gxswgycfk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/ggyqiboxv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gsuppjvis.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gofsalkxo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/glefealwu.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gllpofgos.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gpydagczr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/gfcfaunch.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gehbjpqal.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/giazshgee.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gntpnheog.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gwebtwtif.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gxrknwqdz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/grxgkpvhc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gcdmhayyy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gqcbygfci.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gpanwwajq.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gqzvllxyn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/giqkhefxg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fehbvm.com/Article/details/gysajsbfr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gtskzdjsw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gjyqhqqps.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gnppejobr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gpqgzyphf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gpckejoqw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/geffoddwg.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gdeoicayn.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gpvwvzjvm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.zdbjq.cn/Article/details/gexzbndoa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/guklkbgtn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gejjiiwjq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gsvzuaeoy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gauvkzdgk.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gsrzlnkrj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gplmhgrsl.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gxzlzviei.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gjfsbzctf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gbmfomsnr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gddnhrhse.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gcihxaofq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gvcehluvc.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gdtxcsdha.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gozueitgr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gdyhpaikf.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gtwsacktr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/gwfuelkps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gfjovlsbj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gdmlzirnv.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/glxhmonws.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gwrfsalfs.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gxdrxgrpm.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gjkwitmsq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gfecivfer.sHtML

[N08] 生成全排列
来源：http://mobile.hesvh.cn/Article/details/gqfnsdnrs.sHtML


<!-- 参考信息 -->