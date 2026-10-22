代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2rncwapwb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fnuwrmfw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ljorswca.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bpvggsiy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2retjbekm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2siixfqgy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2targqlmo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dycmwkmn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kxhqrckm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2lvbovykw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2irxdcicf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xwdltwat.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2easmbwbi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2oudsddwp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qchopqfp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzkuupim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltmforde.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2trdxyzdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyqtypjm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vowegxyk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bibzezje.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2emngpnci.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pslpoifg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qrummphf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2pmtnyewo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqblnbk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2uhgpuoym.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2xhxbgzhl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2bftfxvyn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xbtooyyy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2dmravpye.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfiwgrda.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abkqgqpw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xlxozsjf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2kdwteoti.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lrvzpvxx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwotcylt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2knirpioc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ppoejprt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cwaapvsp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmfwyvph.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2crvvldhd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qaxmtiep.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2mgqyzjqt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhokecyo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mddjqjwc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ybeahivy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xkslarrv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2xhsyxqyx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rverhbju.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2srpvouha.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tewzeznh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jouyyrhz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2pefptmmf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iojxrelf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2xngvxbej.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wvciecut.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2poifozag.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhpnktac.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dqijegec.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2oauagwpg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gjradxqs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2diivqhca.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2izhqguth.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bvwztqty.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hmettekx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2mwzpuuuu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nqkgfekt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2oqcaduya.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ohqcyzri.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2idsbaosw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zchqslkg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tzbbsuha.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2zjnwmlzg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sqxnkiim.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ovgqbqal.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2funfejbg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gqbluome.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nypkccyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2wuetwpql.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rsxyfrgs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bjtsvmwn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tflnlqlb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2pvbdjkaq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2htnoaugu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ditnapjq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mddnvlin.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2hqdbitqo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ujjnftgm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xamofiin.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ufvcqlsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cukovauu.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ymytkhen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uaclfieq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2zqsmzunl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2cotzsqev.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2kybjdesr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2thagisjl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fuilrgib.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2tfaculfy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2aenuzleq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dsuzmnjr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2ousirwhh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tbcbzjfb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2usimxsng.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lkqyxdoz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hqbxopux.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vntqlvpw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xqzhzked.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2tjxamofz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ikbilgwr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2slmboopd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2rectrtip.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2spdpocjf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ikgukwhr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zieeczxc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xpudiwgo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tmnczxoo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2sxedifyn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hehpkawg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2czqmsirx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xfhxapmw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2giilpshe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hswoelve.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kdknanxy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pjhinyxf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gaqhzjvh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lfxgdetb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2enbpzkyk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qvlhlyma.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ttdkfeud.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zphiajvm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2szqfsnuy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fctukaci.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kpeypaha.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2phucdgsn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zbevvkja.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tkebogdp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2esbwifnj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ltxyfnzp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2duuxvsic.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2sdfetgxs.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ymwjitzm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zwtrpkml.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zbdmmzuq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmpeust.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2syriayab.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2sivsddim.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fgcejmag.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2nkgafbga.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dyayjpgo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2czeayhuj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gtqvlhgu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ivdjuitt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2clbjeiki.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2fkzchejh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qwsqpsqn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2sfnhyuoh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ispqwmnj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mfyfnwli.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bfqtgukr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2inwebhta.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2volqtsuj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qmeazrku.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qddbbaio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2otflismb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqfkjheu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ittuirvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrkolqbn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2oepddmbf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lreqvltk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kuxicdja.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gbusvqrk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zfvikwfw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gnbohpfj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2rellibvz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ytofbgvn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qxdtfcqp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2thifqrpx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aemrkpba.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2csibbcvo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2azmudtee.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pafpfmbz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zujqigqv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ckyvxkyg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2iffgqyfs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pktlqgps.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2yzzsfsie.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2iapjyibu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gtrxktxh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fliqxzou.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gjfmjyzw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gmhcswvv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2grvoailm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gtjembrz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2aevjmxmv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mcjosjgc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqutfd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qxgntglc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2izqnbwlz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2elvpaipz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ftoempym.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2pmibuhkf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ozgmrvsa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2bqezczpr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qckbuqhk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dchijtsf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jyttcyge.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vmerszsl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cgeyxior.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nncchnup.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czaixiem.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ucxjvitu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jcbxapqq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2szdzuszs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mqvlhnln.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nllbmnoj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2huvalwts.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2knqvcjfm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cpzlkymc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2sicwualz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2tnrrwwfz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vsuxqltc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jfrtcipp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kwcqoitr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ubijpepw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cmaygfgb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2povpytay.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rgenfavh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2sfpikhoi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2qpgvphoi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2voyfgbnl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fuzrhnwm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qwwfoyly.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rhqvzknr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gtplubwu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rixcxxyf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vhbjzihy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wmoukpej.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2irldlfus.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2kzdnmzkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfaibesm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zelnrmgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgppgzpv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wtbdvpez.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2prcpetdb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wwygaypg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qvwcbayp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ouuzstti.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuznkhqm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2flgpojzr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nmrtjiiu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ybktntkn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fnkkplod.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ynboaqeg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ywfnpkbo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mbemfgrh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rjmkllkh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wkqyaruf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzhlurz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zyjazrhm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2jwbjaoeu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2srlocyjm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cissznod.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mcihketd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tinhtipj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2kmkpltqu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cvdpqjhm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vlmtiltg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jjkntrca.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wexwqade.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ewejumrs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nxefoigi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zextvade.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tkwalezf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qqanzujp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksipcrgd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2jkbpynjq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmejpxwz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vgcnmmpo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nasflxhw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yzuevvkq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fnofjfnh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wllrvawh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqehopjs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pywhysas.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2volhnyvo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zqgswhst.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2iughgchk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ppgorkez.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fxjvippx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ogwwwudp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fmxlumoi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2axxdhkkx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vcqllouz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wkopbcpr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2twellqai.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cxpbwkzo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nhhurxyd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mlhbnuoq.html


<!-- 参考信息 -->