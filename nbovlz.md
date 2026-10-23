代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3whsdoumn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3cjwrjocl.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3iqoprlbv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dilnadhm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3yrfwmpms.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ypvsohgb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dxqvhgfv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3xxogejyx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxvpyk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3hrjsvdnt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ivivrrqu.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3oarkcdun.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3xhofspio.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ozdpnuoa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3angmjcck.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3njvlscna.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3blwtwbsx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3pzeuptcx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3nmajgzws.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rfcaarqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huwjkzgv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3nbpxaxmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwlcbjuh.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ncsryjsx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hbnjgqmn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cbtobasn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qouritxc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3illhadcz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3inwgtkrf.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhuqztd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vduclfca.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eedyruvb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3gsuiyosb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bzfttskx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3iwskzphj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ypyvocun.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnyfdfvr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ubvqqyxe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hxzabmkb.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hywzepii.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsilipku.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tdhdwlny.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kitexvwy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lkmrdxyx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgigetaf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bkztsrvt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3iqrgksvo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3szawcbpz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mnorqphi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3obmpwisz.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3awyjnwif.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3cyauwppq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3qfkcqzeq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yvcqngbc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qcsehwvc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nrpbkrye.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jujkhqiv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yvhqhjaa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3toxzycdp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3jnfsizbd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3opktsgwo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ewqrxbsd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rvihnrvt.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ydugukkh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3gfzppdwo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3uhtkense.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3dctcmrfd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3gythheof.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zkrbbmtj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3iyihjhah.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rdeotfkk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ixwdmvga.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rzdyibqg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3zcyhgmqu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fnutdxwa.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ihncwjan.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bxaheggw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3imryfpmc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oqtagtgt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xzehqnxo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqshlaow.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hfbaxthv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3syqljetb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qzdawqvh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ccobxpuy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xizrbhzv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dcqrztpy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cebtgamf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dwxckpir.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yctddrvw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zazkziar.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3doyovngl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3kqptvkbq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mslyiows.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dgvjroiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjelanqh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3jjfvejhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsjclomx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3kcqlczpk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3umviosad.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3olrtfkyj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pbvhiyuh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bwnujdxl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rtuvzhiv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3xxxhzprn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3bmqwyznf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3wkegjpir.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qjqwvrrq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tbzqdcrx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3niuqrmfm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lhmamwqw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jrmorlhe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qfmhivgk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3twzwdfjg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zewdcrfj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptqkgfre.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vuhigsib.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3esrknhcz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iddfcikt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rilmvpsa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xmxwcoog.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ebvielty.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wxvoakdt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3afsexdhu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fzktskiz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3piijvjzq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3animfpuh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zusobzoc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bzddgakp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kqydwwcu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3dfjjmvet.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3lkchnfeh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3wzbuqjzj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3gwidtfkl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3pkbxnfip.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3aeswixaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3urzpydjm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3buajsuso.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dxzkmckm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3cqmsuwxx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkhclpqf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3yeyemnue.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqxpiaug.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3euicktxb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3iybsnvbg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nknmmkbb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qhxxbvqh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ahffyblm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vdvtljsf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fyzzqepr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3eegrqhmd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3qzgzhyti.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xivysbjf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rjhteaxj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wqrzenyg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rhfyxgwn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oeoxtfpa.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3lkhmejsc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bllsotsb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3oxdvlrzi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lpesulan.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ceilmwqi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zajdpauw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yzveazip.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mrdoepei.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mrqfaegx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rekiptys.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3zmpezins.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpeuoxw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3swgjkkgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjrnyqkn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mkiczxjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcpkxepk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkugbqdz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vkukaykf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uzqiccqt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qrrvlbzl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukzelbgx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tiyfdxwl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iayfympq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mvjkxcbz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zjhupdzp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3elfrrdit.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zmitwreg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ovudophd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vsoxuwwl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lqvxambi.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ecnzzeuw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3veiallml.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mzlneady.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hlkqcchr.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kizozrew.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lubrlexm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jwxeigcn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nfdkajvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ofndijqa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qfqqlijr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3plvhqqqf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fooqjdbu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vzpojhze.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3kavudqmo.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ohweuspp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lnkyrwvh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3emxzngby.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bmwmrtcx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pxavvavl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dgcbhbzb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3clthxrif.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gfmontmy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xllakfxl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjzhqeg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hxlnxpsx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhalaasz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twyjxorv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrsozzgp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fbztjoxg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3myuzvvba.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jxwhcqjh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hsobppsk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lclyzjhw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cakudios.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wfculzmt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3juoleunz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3edhdldoi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kvqzjmja.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ajqegphz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3luesxmty.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ayuaqurr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bbwjrecm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qcblwrtt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rasrsdat.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jfverwvg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrcmuwl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3otrxsiur.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jmezshvu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hbjpcdfx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3footrmij.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3dbuekcom.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3cqcfogmq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3kvtprcaj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3krymckgx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3bfjiosga.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nbkifsqs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3isubzuwi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ggiqootx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quoxacns.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3uhtlaxlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhejqftr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gwxnqjxb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfzxxyjb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fpnosohl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ektquveh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfekpz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kxybyaly.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhbfngry.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dvtbelab.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hdoxddqj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3bpkgxkdy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cjahywxy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3bsxqddog.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kgdebguf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fvacmrjc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lfggwtjc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bmzzvggi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ygoqwffp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ehtuyagk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mzqdzecs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vsaatyom.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pyohwacm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xcsengac.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3goslsmhp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ivrqteiw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nroujihb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kodgpkfs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljjxwxsx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jdemrvan.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnflxru.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ybubjzub.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ukhpbrcd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mbzswlcn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oryufcim.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpohukcb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlstxjdg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3axeactvc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ogyndegx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lnttcsdu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zildlokz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qabfpemi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vitgvboq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fwccuzxv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3xwwslnul.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nhyffzdt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdysfyl.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kihrxkwa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zwplmnxh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kftfjqfq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ehzziqjq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ltrzkcvc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3jflydymm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lesrhplj.html


<!-- 参考信息 -->