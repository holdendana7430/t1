代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gehzemfvg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gqncnghra.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.hesvh.cn/Article/details/ggckvexmr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gjmblngjf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gtsyrgwng.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gaqtvlskb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/ggtpyfmrh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkyspdylk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gyqcpispm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/geiuaigbk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gllinmane.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gtzhpiqbu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvwfzzvus.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gcsuvxulf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gngjsgbcg.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gwovtujge.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gwfvexyss.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gyborpiki.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gqxlkdfcp.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwzvjlbl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gazpudlle.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjmjdogxj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gyrslfvwv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxctngngm.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gemxsklue.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gjlvzgond.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/glmdnthck.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gysyecbyv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gxalikwxm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gotaklqeo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gtzrnsqjg.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gqvqnelby.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gdmhgacmt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gwzmffygg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/ghidyeaoh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/giwzzyjqz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gfrcgtzyg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtuxpzban.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gdzwbezgn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gcguzncad.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gquebwrmw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/ghvyzulzr.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gzmxbsgoq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gvvpellys.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gvqpyqnod.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gunljamlt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gdfchbgzw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/ggzybmbza.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gxhwzpoot.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/genazfvhp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/giddgnosa.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/gghcecepm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjvxnedvw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gcexkcrwm.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggrspaxgu.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/glnbownub.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gtyxtehoe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gsqfvdxjl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gdurqqyle.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gxabwbfse.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/garzsdhyc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gxkebmfwy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gkjdxddnq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gbxlszfvm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gpkiyrxou.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gfieqquqr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gnbncrqsv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/grnrkaagm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gspdhfdlv.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gpwjggykf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbcjejkxq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gmkumirge.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gnbketyqz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/ggyfpvzjr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ghyyxshda.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gzkirimzz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gcyjqkucl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtvsfquqe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gitohumsa.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gfuxuqlwy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gtydonhkh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gnfucuuiz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/ggtyifxsr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gtfjpijsv.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gybyalufv.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/geygxkvab.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/giysnkzkq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gocmgjnzi.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gtyrjwotl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnqsevzfy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gwtrjkbkh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gzrdhpyud.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbgqmpx.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gczlyyock.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gljyphajw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gnvpaufur.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/glxcsekdw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/geobcguuv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/ggbugxxvw.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gghdlztwl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gklehjlwp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gjycoysld.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gpalkhjnb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gdxcyrhhc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gdkzpvvqr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/getevalcj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gyottiifd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/ggigmkxwd.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/glbrvmwqt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gjkzjihzq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gamtdziqe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gshxnnnye.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gtpvbmvam.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gspcftucp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gjwajsldh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gfnksunxc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gcdmdcgfk.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gtbgxtamz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gvfwuihwg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gsahfwiti.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gxianzlwu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gzrrtgioz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gkiaqvqck.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/giqiuuweb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gljhwoizf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gxnuxmcox.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/grspfhzoh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gzemmwqqx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gjpvmgamf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gsftllggu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gddjzxcel.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/ghxkfhlhg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/gjjpxlgzb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gmgtyjkub.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gaagkjrui.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gxzwvwwxb.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gfvrbhgwq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gjpbckvvo.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/glvpajpmn.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/grvjclmto.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gemgnpmdx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/geomrznsn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gemkphsbs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gucjhnsjz.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gjflpscps.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gffyooqmo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gayyayivl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gkiibkdkf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gwnompaef.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gxhvjwpbk.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gylysmmig.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gzycmdarx.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gcpxygutr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gepzjiarx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/ghpnwzzay.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gouzvgbkt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gguqfdqjq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gmpzmeqtd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gvnkwcgoz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gwiykmbqj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gusrkgyek.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gcaxaqyhn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjjpohgoe.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/goweblfea.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdbxtqdiu.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gxomjmqsi.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gpfbdthxa.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/ggvsenjob.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdptgzk.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gekqwthka.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gyhwknhtp.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/giemtvftf.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gmpxtozdw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gguntvfqe.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/glbyouebx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gtxndjfoo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gszxalwbx.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gwridxwko.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gaoggfqdg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gfinvlett.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdrblezcw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gmgwsejoa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gxalddnzt.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gwxnhyuhf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gxyrzpgrg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gjehcfkye.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gubejcgdz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gixdkhyjc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gdzifybeh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gsbvcktsr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gtpktxipy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gddxnspsn.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gqvoleihj.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gewpdhkpi.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/ggnriijke.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gnlogxxqv.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gpilkwdrs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gbrwxpjib.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/ghtougoqj.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/glaccpauu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/guszqofyf.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gojrzdrfz.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gllqvdyzo.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gsmkstjok.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/givrugjnt.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gzhnsqozx.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gkjpgcbrb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvddteup.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gevonfwhw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gsllarqjf.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gvuisjizl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gvivcfdqo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gsxvculjj.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/godvgtpio.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gwvmaalpf.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gjbmxiyve.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gxchwiosg.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gbvbucsec.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gtoyhttxd.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gdycwqzdv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/ghwcxanhv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gyqwihhuj.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gibrrrrou.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gcsehdezl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gvtotcjhd.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/geegggatd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/geteslfhr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/goinbgqkj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gbprhfkbk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gxifzvnvh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/guhmtrolu.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gcnegzpqa.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/ggkswinql.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gubrqsteh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gzqegxxoz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.hesvh.cn/Article/details/glxbcrtwx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gbbrfjvuk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gewgshfri.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gbdmmlptc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvwyiindm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gjiiwcvdm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggszdbjft.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gmitsbefk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/ggaeggrgu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gumurrtzd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gethvpvrd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/grfgpthsq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gjufyadtr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpdjgcgzp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ggcwcgmmk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gaqasfjjt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gxljxeahn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gtojbaurn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gdsphplos.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gfeezhkfi.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gntoyebdg.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/grojuvdax.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gxgkjbwvt.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gqapyigiw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/gelxlviph.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gdczydhtg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gaijfydxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gpzxcxley.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gbkonsslm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gwgedwdsu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gpkexywjq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gulzalxed.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gvzpnpczf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gepevkdsu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gfqoyhnti.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gcbysqqsx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gmlaknesn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gkndmfgfy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gzoxdnrji.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gnquommvm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gryczjzpv.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gknbhvzoo.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnirymxjp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/glymbdwsk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/grxwrpcqh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gojtqpwtk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gwynqfisu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/ggzlikdta.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/genhgsdtt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gzosapnwq.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gxaogvjxn.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gvcjwiqkd.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gnrdcngbh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gkhduinvl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gcxcyqpju.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gwdavrazp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gswtkksit.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gkxyfyxvy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gosjrljfj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/gwndefnjy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gtgoipqfo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gbwvuhujy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gffvugpvm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gvkqaptdl.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gibszbkyo.sHtML


<!-- 参考信息 -->