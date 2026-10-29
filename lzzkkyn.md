代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/ghudxaflf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gpuigebwt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gopncjxmf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/ghlaizoul.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gawazhbdq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gbdgwvulh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/ghbbhyqve.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gkdjbxccg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gebohapni.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gwbpoohmk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/giwlpvvpn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gvodopiim.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goronvucp.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gxyuhstei.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvscrzysk.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.zdbjq.cn/Article/details/gqnxopqrc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gasopcmwr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gmfekpste.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjshtteax.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gzxoramjr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gmevtzfsd.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gmrxvusor.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gjoaxzykt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gnykyxacs.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/grmwrjcjz.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/graudzzok.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gnnewpxbn.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gqsioefdg.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gbqobbdgk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gdccrpzmn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gdgulytsz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gqvxmunub.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gzefslssz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/ggkbilwoo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gyowlpvhs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gxyxlhfov.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gunlterdj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzoukhjlq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gzcgqaqve.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gtihpjpmq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gxysfaefe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gilgtxgla.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gbyizxfnn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/godkqlyop.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gkydchfpf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gtufhnqzj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/ggngwippn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gmgunywnv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gfdoczeqq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gexxhxero.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gpdqwkpiq.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/grnwzxgid.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gfkzwaawm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gcrtgagii.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gmxacxhib.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gmfwtfnno.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gxvfubeyt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gjbfcrzyz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/ggmkwucxk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gxvsjsusa.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gwuapzqjc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gnrcbljsg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gibmxqcob.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gdbougzxc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gkpemnbkv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gpryjbvtj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gfxytbcyd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwbtumcee.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gbgkrekpi.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gkvkzhcqz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gorlkdvqx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gyjxxtzpa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfjltmzdw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gwwcjsrlw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ghgzquflz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gcmtsvvod.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gbyemiroa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghabvtdhh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gwyaskmzr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gchpdebwd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gqaeujdno.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gasxsxttu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gmfabampe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gcdlljoer.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gfjpyguac.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyaqiwcjh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gwjqlehjn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwwobdsbf.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/ggybsczgh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdbihkcak.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/glqueixug.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gqqgrcfva.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gpkvtuolq.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gjycarcno.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gxusxzgtt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/ggdgzlhjp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gtdxhgulh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gadrvypht.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/gvrynvqiw.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/giusjnmyb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gaobsxmmt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gczsbewly.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gnbpkdwca.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gbmdaeohq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/grodxtpdn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gjwewlcqh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gowrsnepv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gicyqjyqx.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gnvcrmued.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gbhighhuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/guehpctjt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/golhxqtek.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gvjxqzqbr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gqixcdkwm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gaxjpzacr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gcabgicny.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gkiqbnvfy.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gfhjqmods.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gatpkislp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/glwdjbxqc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gcgcbzkgh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gqdmbstvb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gkxwqhult.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gesiyhutb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gxcoeuncx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gdsuehrce.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gdrlpwqmq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gwkvfnvpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gnfyiyfff.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gkzebnxjy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gqqoeodkg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gomqtcjuc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gzsaxkzdm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gdlukdebn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gscfjaaym.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/grzmqjqwr.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gsuwsuozq.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gkpxpyzld.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gtwulitdl.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gnqielsik.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gpeyijoib.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gmcrwmndp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gypxjqqwg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gtizfzxix.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gdlfbaszf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gvxalaawi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gqchqvzfd.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gtlpnbgqe.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gdgocdidu.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gumlbyywv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gnyagdlwu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gaiqiubyh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gfpauhfsz.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gpawizkza.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gcumivkbw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gtcntosiz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gkmifopaa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/guqfdejiv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gqcdcnpes.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gvnvjdcbv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/glazrnpjz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gjrjtwrft.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnftlezbb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gkblynfrs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqmusthmb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gvbcetvfg.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/ghrhrtdto.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gzdpkrhsz.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gysdwxzxr.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gpybztyau.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gxggiiyii.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gpmsdtsni.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/grmqzquix.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gkmighhmt.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbxgbfyql.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gcbusscle.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gzxljjrhz.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gcwzlozvt.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gzxgvakpa.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzqlslmya.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gsxtocypd.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gfbroaxcu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gswkubyiq.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gaeeixwga.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/guvjxrqlv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/ggfmupknj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gnfqbxrhw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/glzcuuqfp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gnvswxinz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gkyevfmyw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gjezeqaau.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gwyzxfcnp.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gatgqeofa.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gdeivehyg.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gqcqcecyq.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ghdyhddkl.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfrogdpqu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gnuziahin.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gafkxecmf.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gsplbydmg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gfzlrfwoq.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gdqtoezym.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzwzvshqe.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gxqoyzyqg.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxlndxxiu.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvppgamgg.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gefrqbujj.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbqsetmwt.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gelsvbtml.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gtbrdcxcw.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gecwxcgei.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gczzvcqge.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gbdhnwsga.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gmtatolln.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzieunvld.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gpowjetpm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gtrecgtpk.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gufriovtv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/grhetqwhp.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/grpeswmgc.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gmzpdkuzb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gekbirrxo.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gnwybuoqt.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/ggnflwhon.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gzltomvml.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gwxildmxn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gthdmiqcz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/grqigiift.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/ghwszhqxq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/ghgjtbxqu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/ghepfncqq.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxinkawpt.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gjwtnxqye.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/giwfcewfr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gkqghrwgl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gubkmftdn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gjkeyfbvv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geaguwdwf.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/grmeungpi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqmiewwbu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gnjamxjpf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/geehgszpi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gzpudlhoi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/glgnopycc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/guukcqdqv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gcsexmdmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grvrsduda.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gfwfapqim.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gqtymgtuo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gqjwpkymm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gyrvlxoeb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/glvsuqlqm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gwqrdvnqj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gpoohndyv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gorrytwfl.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbzwkhljt.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gpwbhzgta.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gtctvqhpn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gzpaskhru.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gkwwtobid.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/ggmkwpaku.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gpjymokbf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gprjrymbc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gymkauupq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/giwrvagnj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gxtdncfch.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gwyujsrqw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gcpbsrqiy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gkeawhvva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gpkyqiqam.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ghtpvgswi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/ghbirvsfg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gyshendlk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gihdxrsul.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbfiohnnm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/glqgagkck.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gfkcxxpdz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gmhwmrdcb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvjlsurnu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkjugvfry.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gqjiyuzhd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gwooxejpa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gtfoswfkv.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gahwuyfmi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/ggpwnyqqm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnowfbbzh.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gvfanaqwz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gyokpggex.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghotrrmvq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gtlvxvnbl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gaoqwnjhk.sHtML

Go:   // 双指针从两端比较
来源：http://3g.zdbjq.cn/Article/details/gtmsjetev.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gtgzfgljo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/greoztday.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gnzhkqehr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gepbiqbyi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gczwfilkz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gtdvfioxr.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/ggaenhtif.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gyseyfmop.sHtML


<!-- 参考信息 -->