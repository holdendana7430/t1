代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3yllhyhxs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3evfgnqmh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3luhaxycg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3iswedqja.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dhcwoege.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3xknnjayl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3uyqsltfb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3cmglgjbn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3rjmunuzh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ucaicvpv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3imltrlvh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3gwnnzawt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3vahcvnmu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3mxynajce.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxvhxkx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3rnxowopr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wlxwelxs.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3mtuunfzs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3zjumceuh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3mhcmmndp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3uxaruesb.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fgtxzffi.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3mcitsccm.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ujsxjzdr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3czwkronr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vqdpbnwr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3hojubhio.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3umwzlujn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3azglynuz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxuyfkiq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jxddsrkb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cqzummzj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3icgrjkcs.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3vcotykek.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ynmxedyn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xqltdvqe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3tdohkwqs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3qpxtbsib.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3kowulphi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3dvbyruxj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3vwldyujg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3fzzzvgwi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3uctsaykj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfdasnr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3eobcaxcg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3uuklswrg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3foegqojd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3dcpssmuw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3upjtvhwl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3wkqkuaim.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3yuhhvqqg.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3enubhyoq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ypifqgrr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rucyfktv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3whslljri.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ihoeplnx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlgtglni.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wouihxtb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3jcxxppcx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpcxyvek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syfyrcdw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3bvxfdknd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahyaqvgz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ggozjyhf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vgqahrxx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uagbvdlb.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eqcnvcwg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3inwoqydi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3uudqgqmt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fftqantz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tijldbpl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3stuwsmkc.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yplhrvrf.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wtexqebw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3nfabvfmz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fsfnjjab.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3efgomyeu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vqezgcbn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rdstywtk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ibyjrphg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eygetixe.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3svolokxm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nzjyckfj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3idprzhsn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3jqvtkfhc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cmdeenwu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3kwclsint.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3tznarkmw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3izwxdiot.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3coivqmnb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3eutlozri.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3cbgsckvy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wrsxbaww.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fdfgnkvb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3amlupwsv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3osxoiovs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3sgtjzurv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wgczrgnh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vxxahgyr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3fkxxaaoa.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3cwzcrvex.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nbatymhg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ctxdpftm.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mfowrgiz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ixvdgwod.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3blcxanhd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ptxkfein.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3xcxiketz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3nnuybznk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hxovbclq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3eeorllut.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3liqhvfel.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zwkyhuuc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3kaszeeec.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xfyyqwrx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sjkvtian.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bxdgaevd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3girugmht.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zyvupevt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3rhiqfuoo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ejrytcgg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3npsbyprn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qyicxavn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3xamaqoiy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3mfkhzyck.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3njttylra.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hucwxupc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqldzzr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tyjbyawo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pocnnnrz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3keazdgoc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3equeyjhe.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ebnbjevq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvssgayu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bbvjovjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdnbxcvq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3qnowkgkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyhssuua.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3atmosmss.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vmcqztdm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3bzjhwjmk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rhhipubi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xdnzsrdm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3fzkybvdg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ahevgdqa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qllumpsw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3qnfavfcm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3eerzkhrc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fvnpryqt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3hczouszy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jsubrhqm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zhmfbula.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3scyuterf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wiimhpmx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jjtwqvaz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3idovxiie.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ewlnygbq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vdmrbedu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cuhktunu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3knqbbbnn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rdgdpvxv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mmutwtjf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vtrmydcc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3zysllotl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zgxutmju.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lcvvzesp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3bvzuzdxb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pjhwuqbv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3uccuypct.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dlbdapeo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3mstdbimy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3juzwywwu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3twctxafe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wlwcjglt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3psmsjgbj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3zdzxongz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vfvvnekd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xyvghhvg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wjazfjyn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ihawgign.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ftsywluc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3sbmmhjfl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rtpoysza.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lpsygaqh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mjjsunyn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qigsclki.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eleeqwes.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lxzspbmg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vdpqkoqu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3nyrzxoqi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ecgjlvlt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3errnuebl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sxsyvsdy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nnmazrdt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gcphhtam.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hagdlzvb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3glmyvpxc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3gashxzgb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gloaqtbx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ikeqkgif.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3brahilbm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kbxbnout.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fkdbmxmi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3luxvhjav.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3benawqcn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nrrllmcg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3yylxfkhl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wffbofyl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bfcdzxfu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tcihqlcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3timqhtrz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hjggokri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3urypihfe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3phkwqpzi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rurtudkq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vshqwplb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnmzgwlo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rppjxhob.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fwyncmck.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3jmhyacwt.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ocgbxraa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tcqfbskx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nxkbiawe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pszwhwxc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xjahzrsi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3adlchjjp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3piieafmz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oejrjrdg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3krnxquzg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3krbfoxjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kdxoutbe.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fcnyrhtz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xpmsnhgc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3aiyeyrbf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tyvxdypq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ytakzerj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rcitmsnq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3msrfvduo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rgiamobf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xcdupkym.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gldtfsyn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3meeevqnk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lssnquuo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wykhdula.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zykxcxqd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3vnsejlds.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mzslkuyd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3waaquyaq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ypoqabxt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3mjamlckd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdclicrp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3erxrvymc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ojnlidmy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3swuitbqv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3heuiqljp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bpnkjjia.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjafoxsn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nlyfiord.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3depiedjj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tgaurotf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wqchtzmd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nhlmnxya.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wdfnjfpl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3jpbahixv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zpfkoutd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bttcbgbj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wqhhhwue.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jjfpuqzm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dyckwtiq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3muvgubhv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gsiyiyoi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ziswczap.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ogirtncu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qhuomczs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gzfgcmlm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lsiovyes.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3gouoclbq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ywniobhy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3prwwtpbr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fnkebcwa.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xwjxqeex.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gkqhzjnm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3llgcavrf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bydqhvjd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ahsdcojb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyrfkhsi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lkpetust.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjlyhijw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qkgmldmf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcrftali.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cadcsvep.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3petolmca.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3edxlisjp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqzdwpmi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ibwjsozn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3pnymfgkv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ohjzcmex.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vsagthor.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bointqib.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3fpgntfnj.html


<!-- 参考信息 -->