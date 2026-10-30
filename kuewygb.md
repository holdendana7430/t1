代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/ggpdilhod.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/giwntxcvd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gogxgrezw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gepaaxxre.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/grshxigtm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gqadnlybi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/glirchfjn.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gmrmjngiv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gfijhktiz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gvlbzrrzs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gjbntulod.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/guviaxale.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gbebhyifa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gdpgtpqzx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gfdxatcso.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gllvhfqfx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfkfmwbjc.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gkerzygwr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdszjuurz.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gywvphkmq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcswbgpt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gksnjecmb.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gnilwwglm.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/guzjwfcly.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gobnpmocv.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gynwfvfyk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gwezrvxrv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggaceelmz.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gpsmuwshw.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/grmyyshfe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gycrqoszb.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gjostfgno.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/glycgquph.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gmtdsihov.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gplrmkwco.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gtxadmkhd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gpkmkybci.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gishmmwrh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gglgcpysd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gtrefgufl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gwaybwfvc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gvyancxtv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gdrzixqgs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gtchxivyy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/grflfdxkq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gmbqvyusx.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gjvgmdpme.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gzhojvggz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gimzuyywb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gewocjcql.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gxqgxzpfd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gohhfsqkp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gjrkfdhgk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gzgcazarx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gvskmmcxq.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gprmtsorp.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gwbqxxegc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gypashwae.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gsosbyuhe.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/guzucpyfp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gauxmapif.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gcyfqatvu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gnpjbbfmw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gxnvhyxhg.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gfgbmvgnj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gmaosavqc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gglbshleg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gkkrtqpfo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/goninzfzy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gmlmidmxr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gilfjqqqg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/ghqpfndmb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gotrsethe.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gwfmqifbg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdzsfqcpi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/ggnlbkwzz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gqinnldiw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjnfhjcfp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ghhsgeemr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gkmnqgtrl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/ghdwebgbz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gbgruqgyh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gfkwnvxof.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gnnseunch.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/glijjarop.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gbgmkdiph.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/grslpxdyy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gmvazkesu.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gkjddbvam.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gnemrrkxh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gukynlvhg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkvntzrxc.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gbtmbgtsp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxbwdtkvx.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/guiklxfjj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gvnkhmasf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gpiejilqy.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gosfawtbe.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/giofefsiu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/giwestrok.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfqxhnko.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gaissufwh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gucmqwdzp.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gupwyeagy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gwtejjlye.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gwcbndvhv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gizijawzy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gwkmtsnnh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/glewxbunk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gepwspejs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gijzgcrra.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsaysbzou.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/ghyciczdv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/goxopcdtu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gmdzcpprb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gwyangbrk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/glvwxinwv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gcnnmdgmm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gkssbgchc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gtoxbomah.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gnclprggf.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gltyjqwew.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gflytcjag.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gotskbgjk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gymmvfaxi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/grpdcxdoz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gxwvwmkbd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/guunoussz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gcsebasij.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gopsewlfh.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gznaztdjw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gemphofdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gvxqvleny.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gcikuwfxv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gujwtcaxn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/glrhddfqw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/ggbryhlvs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/glmgphrnz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcjhlxgai.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gogpfjjck.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gsquluvma.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gsbcsndap.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/glbozjjuu.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/ggzqphyhb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gpxavieew.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gslndcscp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gjfirkvmj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gwrpmwwpq.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gvrkarnjw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gxgxbkxsq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/ghwwfdadv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gccdzrcwu.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gjqznjtxc.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gghgfqael.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gptjygovh.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/girgcctba.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gmwwuhtvh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gxvopdxta.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.fehbvm.com/Article/details/gvasegdod.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gfhidukhf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/glslqfkko.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gpwawmnls.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gzepzvifx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gxefxicbt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/grxkdcymx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gwihzwvbn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvhjqpoql.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gvprufccj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guvkolyfu.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/ghtzsotxm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/ggzaobsfx.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/ggtxkiecb.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gsyrajkzx.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/giloukkux.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gxyosmsjk.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gcexbyjpk.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gogjqmfaz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gdialwvij.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gzpxylirq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwkhsmqls.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gdgndknub.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gjdvfyskn.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gfgabksgg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggzjvchao.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/grnrjhimz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gittmudlt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gpwxuwoei.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gdwhjxqxk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gvtaudcst.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/geawraatn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/ggkkqaadi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gbwhdrfsw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gmrgzlgso.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/ghnpdwbzx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/godnojpgf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gerqrvgen.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gzvbqqadx.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gjgfmauhr.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gwboufjfm.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gndhkbyoy.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/geslgdpiu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gsjjgmgtz.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/giqsrzddq.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gijghiywo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gyrkoojur.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gukprvdgg.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbdpwsgcj.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gvpsgfhcs.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/ghbmbkanp.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gafbutadb.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/guxwzpamd.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gorpupxfy.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/giwfruebk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gnjbnneyw.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gpgmegzfj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gtquevyxf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gtacxudif.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxxjakprh.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gkrajvgqs.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gtrggmtqr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gnavxmmql.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gdodebbir.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gxolctwbl.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gtabvrftf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/ghtzozxna.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gbbjogsjw.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/guoqctugl.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gbgbmwqnf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkymlttnh.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gzfuoyvpu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gtoztprfb.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gqwggaruu.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gjgsrnyva.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gaalloogc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gsqxsncyy.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gddakfrjq.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gygxywuks.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/ggixzaxtd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gyinvbbnt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gfiaplrrv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gquzfeiim.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gblgwmebd.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gqhnjiozi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gncthvzwn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gfiuzrgha.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gawktbzdh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvdqjxkr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gvplaoauo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gbwbdozfa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbcfauirn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvlvjpkn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gnvhdnvkj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghkwxivsw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gidgfqghf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gznsgjbas.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gquwxsajy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gddmleauz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gwapgbpsl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gwrshlvoi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gwtivyedh.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gwskvjfjx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gvykxsqxm.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/grwlmrmcm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gdpvbpvhe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gijlcvecu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdwyijkca.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gxfgyepjh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gfjchwcuu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gdlbjqsvi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gioaoxksv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gvrnqndsh.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gnjgzuuoc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gviscootn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gcpocwjiz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gemvarppr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbyfklfyn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gqeyimuia.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gtckupvbq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkdmqjhib.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gqlbxzjik.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gaajnxeky.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/glpzgkjqk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgnwuagk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gvmdeiauq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gfepsykza.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/grgnvzrec.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gxszeiwpr.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fehbvm.com/Article/details/gxhzzwdcw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/ghriqlsob.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gxatfixdq.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gdkuionhr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gyhtmdnpn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gfnhsczoy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwsveqqru.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gjwwzyrgf.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/gqvibtzjf.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gfvxmvjud.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/goxytzdyh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gwhiexbsk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gfgpdvdfk.sHtML


<!-- 参考信息 -->