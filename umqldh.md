代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2pgkewrfm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2pnrhgnxe.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2hgnffoto.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2hvtdgczp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2gnrwnkho.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ckprexdk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vjtdhvww.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2doltkwlx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2uueoilgv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2kfzgvfsp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2cvpkyema.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2lwfywsma.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2yywmvkdy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2vjnriuzj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ynytqnkj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lkdymzyk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpjacha.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2jovavmfj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2gwkrfclx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ivowadmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itmugelg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2jrnhspls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svzniizk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2syzfxvcb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2msbvnqhn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2llwydfaz.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sczktvge.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jgtrrfbp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fdunshri.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gunxxghz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2dzhdxzwl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbfwieqx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2uurlnvwo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ftaefcnr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2jnefxtra.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hnuetpiz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ddzckigv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dlwypycm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bnirltiu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzrgfswl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrzvkzky.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ehbejwug.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qckarmix.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tqitbruq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kikqyzgq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2muzhyxlo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zdbxchje.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2leowallo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ycbmzjxy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2oelrrzry.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2uqveucby.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ktughonr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ietekztx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vuolpcug.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bljnckmt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jvvsosuu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2czrbnxeu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hsigeswr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wusjheqg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2urffkdoo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2strynisy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2aqvvqkfu.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pbpxprcx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bpywbscx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zhgpwwkw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2nvdyvvlb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2pmpxlrea.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ncxmmgiw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ojpsagok.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pzthlaqy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2glmqpult.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2esidphpx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ueqduagl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2etwrdqpm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gupczdeo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mggutrqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vsheaefc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hfkepzal.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nvzyxvei.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ftrifwfb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qbhouptx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vduccwqi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cchrjlwd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2lddozcxi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2eajlggdl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wijvvyuw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2rnkyczmh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kptjkxeq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gacpplxv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wtxidesn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pjgwohkc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2sijxwczx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ktoffmul.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vshnglxc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zczxpbga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2osldphzp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2olblwgje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceumzfgd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zkmnwxdp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2hbmdnxtf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lqxcwgto.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2znawcoge.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2utjlunhu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cyhnaqrk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrkmgog.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cdplfqqq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xnlzmbyl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2olanqavw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tacojjel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ijgaqjjd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2argomivg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fwzbtpld.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hbitjpdq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vydnjqwe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2loviwyah.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iolskogw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ujmrqsay.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yamkbrhb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jcheipor.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fmzmawvx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wxifppit.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ydhkvcav.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dxmryeig.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ttzarjgr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2sfthsobg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vxwejqpp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2crqzuceo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rfvbyoaj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xclozyhz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2aiiejlou.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kiqqutoe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2effpqzvn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cwyqcumq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2clsrdtpq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ycqpigdk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kfyodynq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ygiculgq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wvznirvi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jbfdlwws.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2clupfncl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kqgbsfbk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2efibneyg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wetezzlu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rzjeyshy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hynefcuq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qsfallxs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jywhxlvm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ajgrpdkn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bxfvbywl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ssgbyyjb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pbbednoq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xsvonvrx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vhmdcnvb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ccmnipiz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2szgaaxqn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ltveymmg.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xjhhzife.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rfvdmnbd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vzsfffmz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2oubqsrco.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ptgtjsaa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2cxluglcy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kajhchhv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wgozisfw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2afmtctlo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2almgwjyv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nxutiqtq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lfjoheix.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2skudqqux.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rohcydud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xddwavhf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2utjlcyjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gvspvzjn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2cbztgwrm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hapgqtbi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fpxbhusb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2znkzilxn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fbpdibzm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fuvqzrew.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cgtmdtnn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qtejxqxj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ycmxavtw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cfxkvwak.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mlcgbkjg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qphyejom.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2iagdklhr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pxjyakme.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yjrsegnj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2msvgnjxq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2eymisext.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vhqomkbe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tctibrqd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pusnlarz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2oiwsnzac.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mpowzlqn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ypagdmsc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2gztbungr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dxysrgyd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mziwsabm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2smqnazzw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wyewjlhd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2txolxhnx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bxguvbli.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ermpgfgp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iqbddkxi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2eevxinvh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cejjceor.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gqgwvdqj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mbaopugi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2aytlxtcz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sasjjqyu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2adbefdlw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uhmqlzar.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pwkpqjqg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ooqklcoz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjntwwqs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zkcumlqp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2vajkdvnb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2wcfvadld.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvjqxcif.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qxjirner.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tmuyygse.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ytvahcmr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kvauenqn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpuhhvs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xxlcltus.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rjpotycs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2diqetnyz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ebqajuln.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xifievpn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2wwahmsex.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dkduwlei.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vhcxiluc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2qhcxqtuc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wgpggvui.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mdzlyqvy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2einazuwe.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2jbgtfvzx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zwkfqcps.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tynxrgdo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vxzvumnu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2koebxnsv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wxuyryef.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gzekswnz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2lagrliik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgeiolkn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zfpipeql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdiebxxu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2idfcgnqt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cotvyfvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tnomqpjf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ptykugib.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eczeoyzg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcdlfyoz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvowmpc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2vtynqpdi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oamsihov.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ggbonkei.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sgntmahd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xckrvpwj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bwrztoda.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tpfsujeh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2yeoevpms.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2draxcmzh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2exebjycg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2arbwbgwd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xphmjdra.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kawknket.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zfpocwba.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lwrqedro.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qprcrrxr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fjtznzhe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2lqjnxedl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2mrwfqaki.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wubptzfx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kneorpyj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gzfydnsw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zjhnaefz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bgdgxucz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fpaudmir.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2axoglkda.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2yuepvzau.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifernlng.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bktzwrwr.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qjdstjpk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2beusqdiz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2zwyppjic.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2idfpbtrf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmlxzdv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lrultdzi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bgpvbhhx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wjjzksko.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2fxrjsdha.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lpvynadz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fsievjrw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tyylavcv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vxjcnnro.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gvfloghe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2txyznilf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2itabatfa.html


<!-- 参考信息 -->