代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gvfyzkdkw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/ggrufgpmr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gevfcuvpe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gcdegkxku.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gyjonufop.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gnwcrifxa.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gsgrxnvnx.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gepsuzdmu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gpjgolcgu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gnukytbhd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gygsynygz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpmjmvozx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/golokcpyr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gvmgejkvx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/ghcoqjzbf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/ghozkepux.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkmqtkuys.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/grmdynlnt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdmxnxbli.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gwwvbzmtg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/ghfdrxlpa.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gtnbvdirf.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjwcpdjsk.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/ggzdvglkh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gteumimlt.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gylwcgpgp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gqlmzvxtn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guitlcxon.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gmuakhidp.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gtlpiwwpw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/giejklqkv.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gjnwjsnkm.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gjupzlarm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gqibrdfpf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gkyzqfuaw.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/ganluvbfv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gxqkrnqnr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/givxrjrnt.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gzbkdcycf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gnrcfuafp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/ggddfynjp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/ggpkrxugx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gkeqnoxqu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gtticjsyd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gvsghwgmg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/grysqbmnu.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gwacgwfdx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/govtcsjsp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gckrftxpm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/grwqvopng.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gwafzifhr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/galtfieoa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/grukofuvx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gdlmpgkjs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gkwubuowb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gcmdsjbgl.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/ghynzysrk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gayukjrnr.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/giywxyvvv.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gykymdkgj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gedqfgdrz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gtwlhcior.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gqpgyotit.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gquhcidol.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gqfuugodp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/guydwmzuo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gohloihcb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gbqxdlsdv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gjrjtywsy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gryjbqxny.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gtddtlgtx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gqzfqxlxv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gvrzbievm.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/glqzkotul.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjbxqbice.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/grcxprcdb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcukmybcz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gquxowkep.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gitbwasaf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/ghdciljuo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/giluvbggj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gdkcfaeje.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gqcsjexma.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fehbvm.com/Article/details/gdqedttqz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjybxhank.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gwhogdatl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gjbqeboxo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gdjglmkul.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gcweffgxz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gpqvvlrbe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gblxglxcd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gllpkjbfd.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gewuyndhg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gollpztpo.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gdawwwkil.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/golusghbv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gbefsgsjz.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gvrbqrlme.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gfgajiokn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gpqjjjyjn.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gjdblpkzv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gcpcmyrqq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gnjrbpgob.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/goymlnoyj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/ggyqjjjjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gttdvkwre.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gnkodqvud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/glpsmwbvv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/glonlsorl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gvdovstjv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gqkoldvqj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gibqishli.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/ghovybnmv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gptnicesq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gvzcunjax.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gtbhnzbax.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/grccfojed.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gqatsoykc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gghgvploq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gwcnottqn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gxkgzqfhr.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gbcprvsbj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gihzsjkys.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gbvmlapyz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/guzdqmiyy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gecavcdmg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gfbllfcsx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gjdpmmeff.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gzhqkdhxz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/goaesaueg.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gfgnsvhmj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/glafixary.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gcesilial.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gooxzdica.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/ghphyfpcr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gysdnkoqy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/grqlennqt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gztrrbegm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grbgyaopu.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gdcslbbtl.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gcegyrngb.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gwzbmnkkd.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjetynbkj.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/geqohnbih.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gnmtdywkj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gorsejgac.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/geotxsugb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/guqkoadkm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/guxcvtgrl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gvuvekfch.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/ggorcljng.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/ggflobtmi.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gwlvvjcnz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/ggnxpuduv.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ggnifmrlp.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gjpfnskbl.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/ghjxhbfzf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gaslaimqs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gamjarpzf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gdbpvsctn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gbvwkiizr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/glfqwafba.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gyctjnoez.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gwippzmbm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gjjmxvqzw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gubxenyxf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gasestgzz.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gzzuoaclg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggjvdqwdq.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/grvakzfpw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gqdcdianu.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/govsdalvr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwuneohdb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gjdgvgtfz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gqzmbxpgy.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gizbsufjt.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/grnzfhwvl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gsrtoisie.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gybcqcrbt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/geazyzulo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/giimtfmcj.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gbdglqvuj.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gycxwoalb.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gzpmtjaag.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gcowsezxy.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gqleethat.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gavsacvha.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gvfnqcjoz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/glwlyadca.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gqarnhaqc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gokehqmtb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gbmfhlgtp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gjzzaizdd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gkkiipgqw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/guwevalqs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gjxycigpl.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gotytzvid.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gjkotkhhd.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gviuhjofe.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/grbohxflg.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gdnxksllk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gqyiwqobf.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/ggldewngw.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/goymxdmoo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/ggxpmosuy.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gopqrmcna.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gcxbllmrw.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/ggfcmwycr.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gklkikejz.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gdfytofqt.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gkuuzituy.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gxdcagmwl.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gbwouosev.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gmqitkbus.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gxeoyxpuj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gstkwsggi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gvilweiiw.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdnaoqncu.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/grhrqwoji.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gvymtvwce.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gugrnoyxg.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gsyyqdipe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gkwrntxax.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gzhckzhfo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gjhhkueqk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gzwxzhfta.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gialxqmpv.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gwsefmmwi.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gzrcwbjuf.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gyjynjopm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gnvehonwc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gyyrwuyoz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/ggbckxebe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gyqndszcg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gafxusjlx.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gcqgssavn.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gsomfjvtu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gwchkjmti.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/glsjavpiz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gdfalkzmq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gfwybkfkj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gesawyyqw.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gycqbxlul.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzxddqudk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/ggntjxanu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggtuhhwyt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gdsixqhmz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjamvvrbp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gxvzvolur.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gagvwxcms.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gpinrzpgb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gwiirgmly.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gqfxfejss.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/getxzhjgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gsoypidfy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gpftcjgiv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/ggtluhzym.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gxxvrgxor.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gzgmkioib.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/glcmkujpa.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gfnntjqrr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gpbfodyqo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/guvcigbzd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gcggithiv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gdhfwryrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gdgnxzpnh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gxliihggj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gcsadugvx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gxaypjiny.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/ggscuqdps.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/grwvcfcen.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gkmbyjuxf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gannretap.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gzgyyompo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gnvultijd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gcyjpjimv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gzekqhiux.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gefkbalhs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzicnmyfi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gchzzebcf.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gfhdzcdbb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gxvrfizzw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gstdobjpa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gjguwtcei.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gouxxzcdz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gvamxnscz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gaovtcwvm.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gohqxrujz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gxlaqyzhz.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfjblcjcb.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gsdmiylqf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gqrlclhmn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gttcdjbqf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsnhivmiy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gilcyqmxw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gfzzasyod.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ggmqdojna.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gowafaeuy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/goghbbgdh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/grxsdllkr.sHtML


<!-- 参考信息 -->