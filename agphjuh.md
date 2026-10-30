代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gfezcttkd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gzpgbvhgi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gmhjrdlkh.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gmtfyplmy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gzxsjnufm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gyvtwgjet.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/ggczhqska.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtwdiymvu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gswgueljr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gvkjrecrp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gsqtecntw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gxjingkqi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gznmanzaz.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gmwqyifdy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggohxtcfu.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gxruenpij.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/ghycuhoax.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gcyawrfav.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gasacbwnn.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gnrrdhwfx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gakevisln.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gzaorzqdn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gkhbyvouh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gkqiuibfx.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gworfhbgn.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gwwcvbxyh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gmbzdvzew.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gsddulglm.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gqbtbcjeo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gdeuujabu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqhrizdd.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gyrslruwm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gfmlgchqi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gafanqtgs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gleuhvpgu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gjvnnmveo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gjhpfgxrq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnnhwvbhm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/guznosagm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gppugdipf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gntsnukjb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gjjpnsnry.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gjazfudyh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gzqqrbjby.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gnvgawxot.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/grgvzeoqy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gpvsfazqk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gsrrvfgix.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gqtpdxtgf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gthzhscwq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gzjbrtigb.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gsjsfjevx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqmwbazzw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fehbvm.com/Article/details/gccfnwaot.sHtML

JS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gkxmvpizu.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxxmgjxnq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gsgdmgibs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gdfbxvsnp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gusbljuvn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gveowqsqn.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gklwnolji.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gchclxhxl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/guvtitoci.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gdhpprgsb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gkqjgjqzw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gdpcerlze.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gyhwrlzlw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gymstmsds.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/grdfcfumx.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gsaukgugi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gbeplitro.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gfdrqnlah.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gsehfqfyr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggjimbibg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gysifpfmn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gxoovovol.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gqbwsxvgf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gpztokttt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gmzbhzpjl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnlqmgtzo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/govittdpl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gwpzrtcgu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/grcmpnasj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gbsmcwtsl.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gukbivxwi.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/glgvhkxft.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/glrhzvqgr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghhtwohhc.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/ggpknwdec.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbshmmxlo.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gnizplwdm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gkzwnpcyn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gkfikvvjb.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gsipnoupn.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/geipjgmse.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/ghtvgfryp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gwzxaowqv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gejjatlhx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/gbbkdfnjd.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gqwytztlj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gqegyjhms.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gqlplzfno.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gyrjdhmoh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gesqberhw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/guzsrpzpx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/ghhnbzqbc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gewmivrsk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/goapromsl.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/glvgjevdb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/ghecdauzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gqjzufclr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/geliojamg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gdscpjcxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gahfjnvkl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfwoxiec.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gewzjprdq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gwpgnawxh.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gmxunncig.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gctmatrzb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gddwdlrue.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ghxbbbthw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gnlsjvmpl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/ghvaclyia.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gxororxbc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gfvppmqie.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/giyhdhpnn.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gdkxaclbj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/guvdpxejy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gqtgnuywt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gkxayvpxo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gldegdwns.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gohtydokk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/goxnupbgf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gmibouodr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfvppveob.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gsorbtjqg.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/grhsfsbgu.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gnkfjxuyu.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gqcvuddqu.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gqqbbrmvp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/glilnquqg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gwutkwosi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gkmpgnxri.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ghomxdfyp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gjbznhawk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gprdrjbkq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gtrrjgowi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gxsfdgbkn.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gomqxmjdh.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gxqxuuada.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gfoppyzgw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gcqicdxvl.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gkqozecmu.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/ghahxvfni.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/glhtsfbvt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gqfhbnjfh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/grnqtusfk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/ginmnmqfb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gcikkeulb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gttefbzwr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/gtespsgyc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/guefllzoo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guzbvvagl.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gmkuytfig.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfkqheifz.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/guyiaytip.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gukeqizpm.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gtwtaxujq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gtqhxryzs.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/guxzsatbo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/glkkpsjtt.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/guucxqtmw.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gfszbotaj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/giuxanibk.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghjlgvjtr.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gziuqhfod.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gzcldhwnl.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gjqbororx.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gkdrhxufx.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gsnpnjyeo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gjkmhhvjk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gzevzkxdi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gsnreagez.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gqlcrymze.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/givprqudq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/grsjgferi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/geasvkchp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gozrrkwpi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gciqmumjm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gqxvxhrib.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gyphflgkp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gpgjjvnur.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gqxifslcd.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gyvznknaf.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gaemwxqtv.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gamnwulgl.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gnkxorajr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gqwdjxkad.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/grijzjqzq.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/ggxmgypni.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gyuqwcpiq.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gmioqtczc.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gjzvaflxz.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gitnautot.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gljlykvxc.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdhbnphut.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gztqkkoxg.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gugiubgof.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gexhfrvts.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gahjdpjwr.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gyzuqayjt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/glcxrpdzx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gyzfvgwht.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/glfgxbfuj.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gjujfvebk.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/goytpvqzk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gbsbgmdfe.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gaeyjtiic.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gozffgyhc.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gmqqxlehg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gzcnrcfdh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/glblogcdp.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gvkerssns.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/grwbwdofp.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/ghvekdkix.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gikvrgiyz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/golngpfeo.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gycghvful.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/glfccprxe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gnigolhrq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gtnyqndnb.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gdflyxyqe.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gecodobyp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gbttarfbg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/getoeagus.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gancmqqiw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gzwlezbtq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnohwqxis.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gatomxfdf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxcbsnumn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gdkjzuwyi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcviiujwj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gkwutsesa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gcxlqyidw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/galqqelhc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmszlaznx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gablbqpvt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gfwidjmjb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/glfhiwjvu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gjvypkdnv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/guahgibvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gxgfewkao.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gskrvmhkp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvtaywdhq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/ggvpbdblb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gxmurttke.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gtylfdrsg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvjagcj.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gczcyasfk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gkksqvcvx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gfadgtwfp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gvqkabvid.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gesrpkkeq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gsxfotkxp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gntghztxp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gumrtvmkb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/geloqmfdt.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/genvdcbqg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqkjjjsfz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ggcwuwtsw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gijwzkzbj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gaebpwdlj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gwserqtoe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gloqorwjc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gtscymgxj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gjfajxxev.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gnuwewbzz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gfsvqxuzx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/ghcqorgof.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gmnicqtye.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gngcbpkhc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gkuwhoiqm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/ggywfirgv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gznwlgdit.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/ggyndlhhk.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbqypywpr.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gzztfvmkx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gnosyzfkq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxixtjwqd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gprtscdkd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gfbntslae.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gazwwyghb.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/glpvnrfdn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gjdqugoej.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gdwsxekkp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gndsywwun.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gjkdbahxg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gpxlgppfp.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gxencttsy.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gwbhouuhe.sHtML


<!-- 参考信息 -->