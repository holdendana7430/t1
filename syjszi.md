代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2qddenkzg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lytlxbib.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2drueqzsz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mfokywpp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ndnwmcrt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2tgjfirwu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2mvasgkoc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2hynhijyh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2tqbcnseg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2fxkozjvq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2aghurcik.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2tjxubult.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mppgzesz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2cgrzcply.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2fgusfxlr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2hyfbxdnv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rbyhswuj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xomkzfad.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fxtgotuo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2awgjqhwj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2mwvifefa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2glizccol.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tocqvbrs.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2rahjujmx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2dalkddkq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vckookpo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2gaixaoco.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqoqvwpy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gweapjjn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jfkhpbuy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vfrwageg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ztgitbzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giohzlsi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2xqtkzrqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvguefmx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikawreya.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tbfdsojd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vopuaqhp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cyhdphsv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bcwlovca.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2wclxqgda.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjcpxkit.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2jduizizj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2gghzgcsl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2joiazdhh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2weeegykt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2xgcubxfm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lzustobc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2moszeqwj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xhokzteg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2eeybvzhx.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbplmkwd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2etwdoqcj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ikxhinpb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jgqsyxfc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pmgncwug.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tohcptcj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2jkwehyqi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbhyvksn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wxegvrse.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2weuuswme.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2wvgtkhkj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2vaskcnta.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2qtkmifoe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bmxkhppz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ldsmbels.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2habuqnkx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yernllel.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mpusjdip.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ydzjfgtd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nwstpzal.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2dumxvuxu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tgftvqiy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2mklhlxqd.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vfapxjgz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kucfontv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2zytcpong.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2irzoivhe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jndukmns.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2vazatkil.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qvnejedl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kxoqhqra.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nqrrwuay.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ycftbfmu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eypiztmy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2odfzltnh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qhcqzaia.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2iwhoprit.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fkrcvqfe.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pnonkxdy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2flvzkitm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2oydfxcpz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vccznrwn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tvlnfyvx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uqowcpem.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2vxolxszb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mbqismdi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jzbolshp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pfpcckrd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwdpyzx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ttwgrqdt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2utospawh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xzkuymqe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ksqcmhzi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2itlzysmg.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mbjqpcra.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wkbjuodm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tvjkvucr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zqofaalm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruyhrwml.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2khhjxcfj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2abeaamdi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dwaimzlm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sebeuyqw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2paehhaxn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2sanxybtv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dqzynabn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wdujvzog.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2sgkzuheh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2petthhgb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mvmcxwks.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2oxvagqgd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2waaenbxt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pthrqxod.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qwbqqjew.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ivlgnfpe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2tkrtwace.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lsovajgp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ruwnqngf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zycvmmzm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hfmhblno.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jfsutcrk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zkusjuaj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jjsuvegf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nvgoyfzh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2utdepguv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2nzyaserz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gefbrgxz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dwleqzzh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2pllnsqcp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rddplidk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pavczshj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ckmcogwk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jqgbarvv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2lgyeowik.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2usfjauwq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gqurapcq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2vnceybzo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2nzsbluyy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ymnsljao.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wxhokkqo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hzbzopzk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdfatihv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2tpjodbfu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bbsluxcn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hbwfoovn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2odyjzoyo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wwkxtwjd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wwkbgfza.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2psnnmufs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xbhaejxb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ycfoxkxt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xkajrspi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2inlrmsvm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pdrkojmn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jcjlzqce.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2biryumna.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uvrqivxq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wggcthsx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bfljcgdc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2coucwrvp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gcaeoxec.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sfeeddfg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2akgplear.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ujvfbhsx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2pjzdsszb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dpisfbqk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pcdzqhfa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rluigneq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rwebtxtd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ppvlopud.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nknmhgkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hafnxppq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ebplohxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcmnnfyo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xexwnkem.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lcyrbefx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qlhvjxpk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2smzpfqmz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zqjwtrkn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bdduxjrq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wfnyvcop.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vyupgwzm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2krmwqrdj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2upkvjvmw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dckfwqnk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2heddubgs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ahppereq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ejbegpta.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ceyatjyx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2laajcdhs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ehlyjbje.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gijwqebp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ytdkralc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tqqicavu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bkxhtmgi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ldpwmpbk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tjyormpv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lualwzlh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hbodwvlx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jgdxzkjn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2baojzkru.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lsesggsw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gyccuilv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2hqespqub.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2okykolgt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ortvukql.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2fuquezdi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2isxnoigs.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zarxkjqp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2nrzjmabg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2adcncleo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gtzkszkw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wwaaywkx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xglxzrat.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dpepegso.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhugxqlw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jarpysma.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hocnopio.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qudtetny.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2btffmfjc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfougvuk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bskzvkks.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fwzflido.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cqndqser.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fmyhwvaa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wbjvrlcu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xofbfwbn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kfeznzga.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2wtoeylco.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wjfyohuc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fqenjxpw.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xmusdtfv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rkfptvjn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2acdhxivv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2peusmyoi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nvamcgmj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2exexfxxp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2smysdvyv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pwsfyrid.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gozbpruv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2axivtybh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qbololyz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2iifpciwa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bavsxnbm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bkvcnbgz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wsenmgye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bdofxqew.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2skqkslfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xykulxid.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2kwelvtzn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qzwgbdve.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dqokrscc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hohrosla.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jhlgiccx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uedbuhsb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cqxdbmmb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mjraxlzn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjpjsice.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xqbtkyoe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ibvkumhv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sroswdrf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dlmecaai.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jvasuday.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dqypigxt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2apuuzinp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mbpgbblp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gqfgbrqq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nbulqelh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2wwskctky.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2owgbbssr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2syewovth.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jbbgapwx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mfaoszcf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2anhxylgy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vdotklkj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bqhnryns.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2drtdkmlp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaomtqib.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcbfpbar.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wrbgcprz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sajzhrco.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sepkrmwb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mpcphikl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrqzawf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yllpoory.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wcmfmwxt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpxcpxff.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ucsucvsb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tivqjgor.html


<!-- 参考信息 -->