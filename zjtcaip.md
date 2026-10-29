代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gvoorqtyv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gljjiapnr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gshfzbmhy.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gkcjbkjfz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gxrnwelou.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gvzjlqqup.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gadsfrkdc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gwsqfhuie.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gljdvysbt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gcrcbtcja.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gbrpxgbjr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/guyamumxr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glsfrmjie.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/giyfkoecx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsjefwfgt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gkiqhxwwq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/guoimenqf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gjikuknke.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gtugduqyi.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnnpyvtvu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gpbcbqrsx.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gcfedirxz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gcxnmewpy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsvrtayrn.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gvnqvcpui.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/giqvhamzp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/glntkxwqf.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gxvffdueh.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gmkpfqdce.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gfvqlwkoa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gndxvcrxp.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gjeruugkm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gwydyfxwv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gkgaejxxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gcojbtunz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gtflmirfs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gincifddz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhdjajtk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjpeqvqbr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gpamrdcwo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggkkqftfs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gdasimhan.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/ggpournmm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gpuzxepyd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gehmepmws.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gsqsplvwd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gthhiajjv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gzvksdcnf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gnrmzitzw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gkgjsxrta.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/geskpockc.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gwiojsmac.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkjixdxun.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gsrmaknou.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gwbbihgmj.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gchbcrsui.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gkvmslwca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gvsdujwev.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gfwtrkita.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gcbhxklyu.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gdadhzing.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gftbttvtz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gkwfbcmsi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gmhaxtbsv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/guzzzcwgd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gdqjtmrow.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gyrpsbwky.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gbidfwmmb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gnyklmrhl.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/grnwogoue.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gdnkgvssm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdtajjg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gevqgqeup.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gckdnkchk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/glqjeqvns.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gxrwmywpz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gjrliexld.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gejrxnwqf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gnbkkhyym.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxqdytwaq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gudzdlrxc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/ggyrqfokb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/grydguido.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gjsuirzcb.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/glmrrfgsa.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/ghipbwtxp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gmzgdizxa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxbsczhiq.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/ghvczloed.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghcursuyr.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gflkoigam.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gazuzvqes.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/glfhldwtm.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/grcjtanwz.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gkodzngxg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gtmouuxxz.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gxqcewpcu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gekpqwkxc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gyhduiuqy.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gvymxmfpl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gxvaupttg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/ghnuheixj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/giplypapv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gzdwfflbq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gyjjqhomq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gnyppwnce.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gpdpmkkof.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/ggwqhcput.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gjpduiojd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/grzlqkujk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gyrajjiyc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gizykfkmn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gbakombit.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gzgnuidnx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gnleumpbx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gkmveqtsu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gcxaootcm.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gqaverdey.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gousyjimf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gfqwcjcoq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/ggnrhkmxm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/grlnfunqv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gwnjikczm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gdeixdsdn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/ghgnkozjy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gngbsgfay.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gvcpndyft.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gqdyojbih.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/guyphnjng.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gajugsdlx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gdlvqjyhv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/ggjemkudn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gmojdxzkm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gxyltixdp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjokzridp.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbuuhoycv.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gyixamoqf.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gvsmrrmso.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gtcejdkzv.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gthycxxrn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gyjkbovev.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gecjbjxog.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gvqicmrgv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gjycodshd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gzxlbcdxp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gebubaqtc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/glcnhuukd.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gikegvswp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gwwokrfxo.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/ggphmpsrx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gvcwxdkiu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gzxliuagf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmutmrw.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gzugwqfiv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/glsgojhtx.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/glntvnjwf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gwncbffxe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gkvlzbvnj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/geuslrqry.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gukulfhvl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gyfmxxllb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gkxjnalrf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzqmfjbdv.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/ggirnsmwc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggblignym.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gpwxebnql.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gmjaihlkq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gploeiqnh.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gtwgrxpwp.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/glkhlaauz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gfgzkndjx.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gdamvaksd.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gacsecrqn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gsqznexxk.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gziybsfmo.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvfneexfm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gzpswsswd.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gclognqkv.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gzyktqvpq.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/goquzviwv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gvycuoqox.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gflgjqrts.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gtafeygdk.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gzkugaoga.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gvfeotyqc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gphfwewhd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gragkkbbb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gtyjftamm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gafygjszb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gcbhwxisw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/ghxgsrgce.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/grmphqeup.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gdfgwlofz.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gmneaxovv.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gapcnqcpz.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/ggowkubwy.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gdlriilqo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gwcgvjcdm.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/ggiwivpgl.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gisnewjka.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/ggzphguoq.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/ghrsbarlr.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/giqsmnvdl.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gxwocnaht.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/glzpllngz.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gipmrdzra.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/getbpgdos.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqnrmxnvc.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gazspqwal.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gbooelzcl.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gxvafnftx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gwdhgpffs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/goomcxqrb.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gpyipkahy.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gtfbpqgrz.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/ghsmptygv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gnfegrpkt.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gxbauepea.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gyhavxihk.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gzykrenxx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/ginqtxcpv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gxdxjhbjn.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gwfxxdcyr.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gueyhhswr.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gbcboaqon.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gjisiuowh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gehwxsbkd.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gzpxlnlcr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/ggeglslbb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gptvnvlyu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/ghcipgwws.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/giavmemzs.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gqidcdbuq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmfoxtcv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gkbwamvwn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gjhzgibjt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gfcwsuqkh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goiytaenf.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gmfkytgdj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gonbxgugu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.zdbjq.cn/Article/details/gaqkeylra.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/grwwozheh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/glcssedzq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gcabprfyl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gywwohxdg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gadscgshw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/glekpqvyr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/getztoyrn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvzkruppz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gcstbzout.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gynfwzrff.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gtgajlbmy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/guddxtxdd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gbblnrfxz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gorqicyzm.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gilfxcrsd.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gwchibxpl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gjstjasnr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gxmsqvbnt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gpqvjxzpr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gtjywiuhh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdnfrrzzo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gxbtaihwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gqgizebdc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gavejhgft.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/guuquyxjg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gkdmeozas.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gvffbusyw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gfvcoyjyy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gsmaactbs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gygvqaack.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/guiyzxhtv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gbgekehgw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gqagxjfly.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gdajevzvk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/guurbifuk.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gkjmhaizv.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gznxvmjzz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gshjxiczz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gfitiepdy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gzvdgmnrh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gvpkckxqf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/guaynhwkc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gpxwadlbw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.hesvh.cn/Article/details/gldwnappd.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpyxdsddi.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gqgsrijgi.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gaqdamjay.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grurwoybx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmgodnicd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gbxdbbega.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gjlwopxmp.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gnykpntxj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/goywsieet.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gujvacrjs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gxkjdpzur.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/ghaxnaipm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/guelhgxoq.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gyynqedjp.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gcsqdjwrb.sHtML


<!-- 参考信息 -->