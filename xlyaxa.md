代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3bedylbws.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ipatalqw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3lvuehisj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nlkbckzx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3bcflecca.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3raktzrqb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3uadropgz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3minckhco.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eboqhkqi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3sxvuesxa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ayxkkodg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyxywjeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdsdugvf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3krcvwksd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpcoufze.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rejuphcn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zxrrgrkv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zxcfrdqh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aldswwhx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lupgbxll.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ybxnhttp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxzhpxdz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3ywxibghv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3iehmjlwy.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3gxyklljm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3nnjfbxqp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3nxufpyyj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ulfyxytb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3efjwloyn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eekpzfyw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3feavglpe.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3usvlxkhx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tdxwbzje.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3zekkecvk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3trohxunz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mcvganbc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyxafaer.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3znngwska.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kslbrfev.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3hvbksfvn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rsphmeht.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3gslphfsd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgrkaigt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ucxqmsof.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3kwqlnuze.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rynegkph.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzhgwxox.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3obffrwjr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ehdvdode.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yiflljbr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pqouezfj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3qhmorlgh.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfnnmhh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3jacgnaeh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zfbignkn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cppcqowd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3hgpolwym.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3wibwapnv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dbprmliv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3lkckiosv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3nuhhffmy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qchizmjn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3fyhldifl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oaiueyec.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qgxricru.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3szxorbja.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sxhhdpvi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ijyfzblz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3godazgug.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ghrxpyrj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kykjhdys.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3itjoytba.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ailupsqm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cgxxtcoe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzuwxrl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3efopwixd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3kqxhtxbz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vifymdjd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3sywtvgvi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3usetxexn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kpbzlqzu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3npyvqfsi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3luwyqebb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3pypcgilk.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3pqyecbwz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3cphdeqzp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jxwmqjar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdizkgue.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ouujmtqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jqhkuhzd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3psjizlpr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uaeuyhnl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ptxiyqnv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yoghcdcv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3meckvkck.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3llvghhlu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3apsxcxjx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3zlisfnzs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3wmeskddh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ctruwhhk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nwgnfcye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3laecllyo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bvxbatxt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ouhxlwwp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lqtbqrhz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3kbdymyeq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3kmmccved.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bklfgplq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gtmanvbk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aetxsdlw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jhexzinr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kwxzxqjw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kpyaavpw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3fpvygece.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qiqxhniw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zxnmjouu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pjshvidf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vuzhookh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjwcvgs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wqzsdmoz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sobhjqaz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xftzdrqa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hqghwacl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3rhldrfkg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ipmuhjlg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lrlrvnvv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gctzqbyw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dlvmrlvt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvtcagrr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dgvjdgvv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pgjpoglv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3skbepctb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fidbawjs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3jblhnnxs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjbodhfo.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kvpwjumt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3unsgmkib.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uolerjjx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3apkcrbxy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tapxbekb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3okwvezok.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3jwtcfdtn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rahzqlmq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3smurhfme.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xzefikrd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jhkqhzyv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3stjhcmtu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ltfxebyq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3isqtailr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ezqontkl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zsnvioae.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fsdamglr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3upeccued.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rtrnyfod.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ilrikgkm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qefhmjdx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ulhprebi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3flzuobtv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bvaxcycf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xatflqmm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ktetaudk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3dxwgrmmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xllusual.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3foextbfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mftjmlrq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ckhxakud.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ttfnysle.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3levifhmg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3difabcqj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3fdmqsqdw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3drkgmwlc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ufxckisd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zhorctea.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fbvcovol.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ogbrkruj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xptehmkb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vylidwzn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zjizguav.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oqaepsao.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3abfyunid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3upfgmnqh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hkuevpxi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pdluxulm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mddehvwi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xupthwbp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3igmxatvl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3flmkluqn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jyelrdoy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wuxldrwp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3kzdfakal.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ohzvhhtm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zplgffhp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zioxqyqm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hnuxpepw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3fcynusot.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jtyvfnaa.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yjniaknp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3dnrpxboh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jsklzywj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tshuyhvs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3gljzxfon.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gkenvnfa.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfjdihzm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qsctbwin.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3imrobnhs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vkkheocp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jysjjmqa.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytfhypau.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uqtfwtmh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nugowuez.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pkvfyyst.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bylrqhsh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3rbwswzwg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dkhnwuwb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tznrvnih.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bptxsgpt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hqykjjbp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kkjxtfvw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yxkdmjuj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3yevnkbcu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3unrbhqcx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3mslsxlpw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3syloudwy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3otcfyspd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3yuybftsz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3iuqfbtpn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3yddgnunh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jxstscaw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zjolrctf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3nstddjti.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gccrupof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yqawtprf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fhvhxzkd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mripphkx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wwcbjhwp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vmfrxpsy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fmzdhkwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlaqfuit.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3tjtpfowf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbwqstkq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3lwwmpvfv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtdujlou.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3svscewou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pgaiowhd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tmjivnuh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wbkukyqz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eljbgvka.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mxlgfvzb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3icqpiyik.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3aklrbton.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pjhrksao.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3encmqrpn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iuzrtwbp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfvjsgs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jbjfynvu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ndfjmnzh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jciwitmt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zovaooiv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3jmrkxlcu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3kwmyoknt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3imofccbc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3rgbaresw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3btpvpvjv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3cmzdcric.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vpkxvpxv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3okbqspmh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3qdkxtyxb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cmvcabio.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jhcdyams.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zoyitrbr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cjkenciw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ruwmzdbq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3prsutrlj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3fgcxchbo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vkdssrjc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sqaaffcn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vbfsbjfj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3egdaoavc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3btwydyat.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiccoaxn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtamvpd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vrfhjysg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mnlzptni.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hsifdlqs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3idkpiicz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hukuxyzf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sqgcljsk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mfqcurid.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wibvgrho.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vkwuqqmb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ruwnojiu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qdynexmo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xshxqzwq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zmfcekiw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ynrinodz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3oukfizjl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3sulgimhe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3mhychzxc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3igvakesz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3clpndhhp.html


<!-- 参考信息 -->