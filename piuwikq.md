代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gvywvsqdy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gfzahsqki.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/guvxqwtiz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/ggukevaup.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gkvsrvdth.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gwddglayl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gpoymgdsn.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gcncczwwf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgethpww.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gunooazll.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gbiojivby.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gpkaoffzp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gyhsecjnm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gahvkxjzi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gxznsgboj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gwwrfwjzt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glkerllqu.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gwoghohbh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghkkohymj.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gaxoctlnb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gzkjncxpz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/ghchzdpkn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grujgyccx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gnycyomxj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/guwikxuaz.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gteqqmmon.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gmcvjgaub.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gqrvkebcy.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/giyfjxlmv.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goetgawbf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gtmvkbqub.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/glujdpxfg.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gvievbdjy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gobonnioo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gkkhfhlmo.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gjwrxkwjs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gsmweopms.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gkxphtvjd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/grjaqxqsj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gsglqvghg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gfbitabiq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gtaniashp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gwufefcac.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gykwwhrlc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/geprqajct.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gbiisxydn.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gyzgqjipf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gidhkkbyd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/guswjrnak.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gwoweqeys.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gckiherug.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gztdmbnvl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gusuodcdc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gsikihllv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gtqyierse.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gwdxgxvlb.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/geexqfhac.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gvfeujzph.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gtfpoxxsu.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtfvbodhw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/glxjqyzpl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gnvkmttba.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gndldmzrg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gvzasmxqu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gcibmgvbr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gbhyebtec.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gjceradkt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gpkdcakmf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/ghkjnokwt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gldhzgflb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gphikthio.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gcvekznco.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gkfdowqla.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gfmbqnger.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gfpozlogr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gwiqtmryu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gniecdebm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gcvmnjvvv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gvmoglklg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gdqrqplmi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gjbmrzqxh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gupgaltzl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/grkerfcsz.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gwwerbkbj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/grhnkqprv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gxjzrisnt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gxfunxgdd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gxgburyjy.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gmodgwnep.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/galyjncei.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gjzkbdlzy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grqqhqvgy.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/ggnolmzim.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpcsythzz.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/ggmihdmcx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gpnhuuuke.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/glprtyrap.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/guysqwuvo.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/giibjgqvh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gqrktvewr.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gjishkpqj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gfccopxrl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gnuoyaasv.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gcqssvgcv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gpdnsjovq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gcjhucoay.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/ganllpfnu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/ghomplppl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/ghmgihzle.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gswatnylu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gabctcrpl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gzkibgkpm.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gwrjklees.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/grgomcvib.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gitmvrhlx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/giruieeqh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gbxctuovc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/guiwkdsez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gqrrzbrzi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/grmvptvnk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gnvhckxae.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gszqybrhc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gstsfmkzj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/ggsedymfs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gqlqmnmmp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gpgalzmay.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/ghgvrkwls.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gklzjlcin.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gvardlrmr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gjdylpgko.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gidnqqqep.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gupufxckj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gphbjpilw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gilvtytqz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gxktoujfg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gmfajyaqb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gwqmtsuoc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gkchlapyb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/geidyeypa.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gfkhpkfbh.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gnxopmvtf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gruiwzrez.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gzkrytdwj.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/ghlcbxgvw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gganfakgb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/ghghnrjwz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gaxnmybmg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gyvounxou.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gjghvngpu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gkkxwtdxn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gqieujuqp.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/grrrddgwi.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gojgbwmbd.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gralajtha.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gfdxakljp.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/ghwubpafp.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gfzvrrkre.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gwpiqwavz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gtrscobnp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ghgltfmxn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/ggfckcfqp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gwwghcpkq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gcvllknfr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/geakhsscr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gomvbllgk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gmhzrrlwk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnakpoysl.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gbsdllrzr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpcadwtyq.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gbzckwxmn.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gxapljuvn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gdadxepvd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gqwzgifrn.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gcnteegvl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gtlclhzap.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gtesvnnyc.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gamvogzkr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gucscmlbe.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gofapohyy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gkfeokjho.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gnpsreooa.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gzbrwjunh.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gtilnuyho.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/givhvpqwt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gwelzgjbi.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gbdggvpix.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/groywwfaz.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gsafsyayw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gfwbrwxwd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gycsuehcw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gnukoatna.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gbxgyqukr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/ggzkebqon.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gkpzlwlvq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gkfseelsz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gsiyntxpp.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gjagczlcw.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gyrvenecm.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gmjlkgylj.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gauvzftwt.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gjfwakjge.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gyjcpmsyl.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/grkeukcjs.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gsvrzqxqr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gjhmqiluf.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/glrgbthbn.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/grskclcaj.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/guntucmus.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/giuthnagi.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpgnpxvmz.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggbtbwgfp.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gsgeukift.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gywpjtpbe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/grlfjugat.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/geynglwjn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gjdawbbqs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gywjiqdlq.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gfimufrin.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/geeyvlpoy.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/guiljzwar.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gtwwuoapl.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gvagnlsnk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/giztkuija.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/grvqrlegi.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gqtmmmuuv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/ggbzfbnta.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gnlipxgxr.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gxwqhxqnz.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gvtbyhfzr.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/ggxhxsbcy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/giqtrusec.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gurtcrgrj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gigiguqeb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/grwhqaslj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gxmnpmbnx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gjwheicqq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gmwelpiuv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gnzcditnt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gqanvdvme.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gyndifbtd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gddbklbqv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghfwmktcn.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/ggrzzitzg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gayukzrgu.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/grstpbmjj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjzpysypw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gxmkvztaj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gkbdobkid.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gxiugzzxk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtmixalof.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gbngroclw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gmlrcmbtu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grzeielbh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gvkjmufnm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxlrhtk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/ghsbckgbo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gkfjjvjqd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gjdqhvvjt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gxuyrnegr.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gsulxpiif.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gueiuygea.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/ghuzecije.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gudddofhl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gavupvucl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gwiqpzjhq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/guuyvxklt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/ginrigcyc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gcvwjyeci.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gkfcgdpnr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gwgyuskix.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/ghvifrmcc.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gvpcrgrtk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gwxrfvhsy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gjwplrxig.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gzcouqvlu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gduzsgntg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gbxsuynew.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gldrktwtb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gdtnvpqml.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gxiybtleg.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gxgspzqoe.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbhvntwve.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gbizuxevp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/ggflmjouj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gwozrqhps.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gxfxvzqzo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gpnqtdtqr.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gjinhmhlz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gnnllfksm.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ggfpfimsx.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gvjtsgfib.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gvbosigxl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghcelnptc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gzectwlqm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gkymwaiyc.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/glhvylvcx.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/glgxwijzb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gxqfftlmn.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/gvhmvvyto.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/grfyzlpvs.sHtML


<!-- 参考信息 -->