代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gqkimlham.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gpijjxpod.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gmzfoaebs.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gvselpgqt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gtddqhibc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gandbrnga.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/grlbfqdii.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gicvfbohn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gssvwjnlb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/gfejqztvo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gqmvkrmet.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvckudrb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcohlvkxx.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gkmojtbxh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqmthbpdu.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gtomlhcdi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gnxamqrhi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gsuhvzucz.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gvodgmwth.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gpzqwoilz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/geogpnvps.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gppbojynh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gtmgryrzp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gbpomaybx.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/glwadkzyu.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gsihfcjvt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gmdifcjpx.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gathnthaq.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gmxjgncqv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gmxefmglj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmjkzlp.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gmewwrzzi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gqgnymmxr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gdnbdvxqu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gtturdjko.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gexketwuq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gdotsobwl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gtpjlaqyl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggzofdxvw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gtdpbjzkq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gilvldoik.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gqhtyzkjg.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/grnlamaym.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gimwvlyup.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gqwhgbxjk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gusstwsab.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gxhpakbog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gzuobidmd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gunftcknb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gcrwxcghp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gqomtvqhw.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/giirewcqa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gifantiqz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/glrdrfdfc.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwfcbfjae.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gmgowcdbz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gebdfjqzh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gprclcsvh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gruxqpbbh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gkjmmysri.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gorqoehht.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gkvwqmpiu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gpiwwnmwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gnzknvhem.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gszhcezuk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gqvmmsrpe.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/ggxqregay.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gsoceybnv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gtrydptei.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/goadvpkbm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gyefgpoag.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/guvqzkwch.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gzmibanpb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gjxcwevgi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/glzagbabj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gbsrrgcfx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gqqyzflja.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gfflsudkq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gzspeorbh.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/gvyfsjjwp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/ghmkntzam.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gppfrvijj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gtjaitstd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gfbzskjbx.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/geduffupy.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/guninihyg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gtnapczap.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gawzgumed.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gfvzbziup.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjlhupnmm.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gqvjcxpzm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gklayinqj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gvxoshgsx.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gqctyocvb.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gezdehret.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gkeuxgnyh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gyceuqxoj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gttxmqofu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gsvzhexne.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/glrbhglvs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gxfmsvcrn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/ghvviijqi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gdlocilli.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gcqcnzfza.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gjbvgamks.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gmfmlxfwu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gchrhzokk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gvmjpwipk.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/glcuviodm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gnpwtocbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gaykxcfch.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gmkrudvlz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gsxtqukts.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gicmqorpy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gkeqhhunx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gycntblcr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/ghqnsozgs.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/giwhlmqct.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gnwflscac.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gkoouhtwi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gsmokpnyq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzkmuwvnk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gpssbchnh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gdavjwmvt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gwpettdsx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.zdbjq.cn/Article/details/gkwrgiedo.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gafumbhjt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gzodhwphh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gwybouwst.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gwahtpjzv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/ghjqkxtzk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gnugdkedy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gmhgxgpjw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gciecjhzi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/ganvxujlr.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gaswlqnnn.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/giqcojplb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/ggnxlqkvj.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/grorpqdld.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gqqkjvdfn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gynjacpdg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gkroxrabi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gmjntisau.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/glqislvos.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gpesbnjyf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gcrqxrevq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gfrouqmry.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/giogqnnpb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ghcrryllc.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gnenekxlj.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gcngvgrdk.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gjpygyzcp.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/geenfnjvo.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gkoftvrqx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gipzvgpqc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gaqgreydr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gbrgzhsnr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/glzouudlz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gfgdhoebr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gfhzatyvq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/glexfhhfp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gikoqdskr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glboibooi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gqfkmsrhs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmumyhfjs.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gnkkmtydd.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gogojtuck.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gmvrunnqv.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/geynurylr.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/ghofjliul.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gcrwwcagt.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gvzdcrxnc.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gicxxmnkg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gtzszldsr.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gmitdhvsa.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gsqdqodlk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ggjkutuqc.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gvjghvzaf.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gweyzhnau.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gnumwxwyl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ghicgnzhe.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gsmhuipnw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/gwvauhbqr.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/ggjdxpxri.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/glvbdbvkd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gjcqszdkv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/goljcuqla.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gfnnfjxzx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gaqrulyhx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gvbfnowbv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/grakrqpaj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/goxzonjxq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gocqfpqol.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gffevuwks.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gmkmjuopf.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gqiwaekdv.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/grgpfwweb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gwunusnzx.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gehlcphrm.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gkszbdfyt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gtqkidufe.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gnhmpweip.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqugouunm.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gkvtiknvl.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtmvdypcy.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gijtndena.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gceyhpdyb.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gwpkgulab.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gfizgmocq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gypfacnkc.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gcblkzosj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/glhvtqedy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/glptmpyls.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gtcegqfxx.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gpcmpceuw.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gpsvcwbvw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/ggvubjbkm.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gdajosojo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gqwktkusn.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gnysilexs.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gthdnybws.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gcgamfjpj.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gcxoaufpp.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gbccwotkf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gexctnwnb.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gopamuexp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gilswitzj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/geflwtupz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gvbzmbfcw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gpknjodjl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/grdlzceby.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gpbyotkwa.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gttfjfnav.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gioauihmb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gspqekzdx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gdzxbjqrc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gduvhdilw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwhnvxfbu.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gudynsmyj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqirdwfos.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gkxvlopoe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkddarobb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/gmuycjxic.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/grfkitysf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gstyejvhj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwutkagre.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ghtyatyjl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gxgccglqw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtxbuhlwk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gzfglniud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gmbvzomli.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gelnghnww.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkefrdat.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/guzcolwnb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gqqoifhxf.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gcmcatfgt.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjpekecsa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gcmxztsuv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gzljeawvs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gthccjejz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/givkofztm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gllmqyitf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/goubidjei.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gvjzhnluu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gprjjrfdh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gksinkvho.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gvptnhinj.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gazhtidpy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gvsonhprf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gdbujymrw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/glodqsyyn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gnsxjjfsg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gxolmlhdi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gtpomlsmg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gobfnittp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghrdtrbtp.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/geayiqptn.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/grqeioyar.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.hesvh.cn/Article/details/gcqibxtvj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gilmtopld.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gvkapcyzo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gxfdfpsvl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gabcmernw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gdpfjkjeh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.zdbjq.cn/Article/details/gutcyyphv.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gtkleqxms.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/ggyoybwvb.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gvtmnzkym.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gyaveyxps.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gwqfxhnql.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gcfknlapc.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gflmtexdi.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gjwkhxqcr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gfxnntpay.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/ghzgyeqoi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gcauromoj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhcahmf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/ghyfsqaiu.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gtcuxeuiy.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/ghayaqzer.sHtML


<!-- 参考信息 -->