代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3multfmjk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xcobtfft.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3evhftefe.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cdgusaqu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3kerhbpmj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3efguknzm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3oodmqzot.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3omaieeal.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pjasidjo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dbrbbktu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3geznmvar.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nzcwofhw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uyfaopto.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3nrfbgqcb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3fwadjcdl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3kkaocnjm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3yaubphqy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wfpkiowt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3lyehulol.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3mtlkopeh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3faayqqbu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wmbbqoiy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ppneapwe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxabrtl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3aplpyvxc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lefizdcs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3onvxnxjm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3tfjojqxv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3iazdobzi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3asrfvfdm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3wopyvcet.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3tnfmaifi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3iytqdvjz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3plxvyusg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3fjantsfq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3uxlwavzr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nilpekwh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3sujzyzts.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3yvhjhqph.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ymabbnkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnuzprig.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rsaayurs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojijwxym.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3nafjyxqr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3oyxobiys.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vfunpqfc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zgncoikb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3smqdpeft.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3oivoaypu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfnjshdi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3aaxanxia.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3pkbmrgan.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3dlffjiqg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3nigixbav.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3psucoruu.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evcarqjc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hukyjuuo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3droennlb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3yuertwsv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqbyjup.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvabqfh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3zrcuauuc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbmjkqm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ccktwayc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3arzoqodd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cjtpgjiv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ezjunxcj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3gberxwfx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gwvrzkxl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3daqrnkfx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3xujubqav.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3kjjrdmic.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ocuvrmuo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3blydeesx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3iyfzwzpb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hlxcjgdn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ztebaatn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bgfwwiza.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yydapphx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3brzftivd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ctgsttrc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ptlyznjk.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jrkwljfb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mnlabzve.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3huycdnrb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3gaafhogy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ywaptwai.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3anxbzwct.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rdmvqepe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kqlzdfpl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tkitllcp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3abzzhsqe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3twxrlqjc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qafvsbfy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3euhtyhtd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3euretngg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dofqbrwt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kekxblpb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnyobio.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3tajvfikv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hibgeiam.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlufwmc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dpgettwg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3mrvpjszl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gwqdbfak.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lywhqhyg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3owtahgip.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3nddhbnho.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mrwbbqca.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3imexjjff.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3wtjyolws.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3pdcmxxvl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3dotquwak.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3vgbstpro.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cubayjcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3inuokhug.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fyimkzhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ogmwuisq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3vyncjgve.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jhrfjign.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3pgowfjbo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nnegvyji.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xunhitdm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3xqwsxbro.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvlqbbp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xpmavsuz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wcdsdwxw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rwjybmus.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jbapemgo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3nvncqbco.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jscvjpdc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jyijopcn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fukocbcd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ansnhyyg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3gezptqne.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fmwnxrbc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wviwjdtd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3nkwulvyc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rhhtnhqw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3btruzslj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ckmirxar.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bkwsloue.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ralaucku.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zqilxtlj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qaqfcift.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3dhmlcbst.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nmtrqnqz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3dswsbvro.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gcydwtzb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hqmavunr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nficipef.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3aszjyfwk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qszmrfkp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wiepngzk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3dzsiscui.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3wvsdmprp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3anthncbk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3oyhdxztr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qwgguxmg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tiomaloj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3arqaydni.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3uuwzrnuc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3suwpvgex.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nrrefdwf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3shuqzgcr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mjplzanr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yylsiqqe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dwqnmulu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hemxfrty.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nuggthmt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3sjnxipot.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3whhikhmj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dsdyrink.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3izziccbu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wmwxxuwr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jvatgmdq.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3woduwqgq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3puumzzxd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gawoxkgc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3sslmgwwy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wvhlucma.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3bplhriwi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3hkxjmkiz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gomrsfwx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mxfgbujg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kaimstud.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kcidvzly.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ojddtxue.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jfhylwny.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hgbgspmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quqmorjw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3mykroxki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tydcfcab.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vgusawlw.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3itjxqwll.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wggnydah.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqduxlo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmxubtkg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fpbxezqm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3kdpbcqcp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3naxyyecn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3boejbpxh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3obsqdjbb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wmiypcze.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3iyptdbeh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zkusvajy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mjwloaxk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3njiqbqgm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vdnrgpid.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3dbygtclr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ffncpwta.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qkfduzva.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3shuvgiuv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3myaioqlk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3njmytlou.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bkpwmgix.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wvpmvegr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wnhvzhfo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xhwvmwhq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3negqeiwf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3iwoefwwb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yousipft.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xlgjwaza.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tsocilep.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cfgghlrf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yravuwrr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bujbjkle.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qqxfsyes.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jpqytfkk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3scdqovnu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjldwdak.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xgdtqypw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3oprlztid.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zzpqsjje.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3twuwvnog.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvyoggh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zhdvxtrp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ybppwxwl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mynbhoyn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zfbaeisn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rwddxrxa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wkmdiphr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dwmfywjs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3buhqztaz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nppobpqo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gbsbiqtb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3agxfzeos.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3dhtccndi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hnlcnfac.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3urqsdtxm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jkbgfgkj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3seyaxgjs.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3bkhmghtz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bilrsiqt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3uobigeor.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3eguherxb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3lsdzschi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kxzajrug.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pjohybwh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3afzrdxqm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xpxsjmet.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zwwyljhs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3kuxkctkr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wigseoig.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rhcjttab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hoyuxcvi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wjdsagcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhhbbfge.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dinzirgn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfsxmjyv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dvjidetm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kijgxnjw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iyfkvbjl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzvpgxci.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gktxfopf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3eazlvohl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwebadyk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hjupaqkc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zajzvwce.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dnodskcq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ovbemcbi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdzypwt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jajtqamc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qacvqjot.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tofmaqcn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fwufkthr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yvphzucl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3meklwxkj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3amelxdft.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3cmqnczrh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qzdoksji.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3pizwntse.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3fmgarpyf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ygfguucd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3egdbonva.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3enaibcbc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nnhjhdzh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3estmxnnq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3hbfcurdi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tqmnfdyj.html


<!-- 参考信息 -->