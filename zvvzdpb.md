代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.hesvh.cn/Article/details/gcttsvoun.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gykdndaau.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gqrgmuvjv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gwnnupygr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gwbjhxkqw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gbkqxmmnv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gpfiyxsik.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gfnucikns.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gjsafdpqy.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/guabcbjtz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gcbtyqbhh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fehbvm.com/Article/details/gurbsaycs.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gfwlaogqe.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gvswcizoc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gvctxoyei.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gpzyydrsc.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/ggcxgwydt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gzxqbmwlv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gqgktqdil.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gztztqwaw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gzbvqwioc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/grhqqkoyg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gevbbattx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gfurzstjm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gmtwdnmpi.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/ggudpjyvv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/govxppsft.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gkonpwmlv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gjwhtzzhc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gtqxhgbbx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gnmbsqihk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gvudwvryn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/garsxwnlg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gqgbqibbi.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gkdnbccog.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gfhidswke.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gklmfewmg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gfdkxgzxh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gqpopnubr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gmkpugotm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/gwiyzbvsg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gqhfprlux.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gefwronlc.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gepjkvxnr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gkhficodp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/ggycrddxa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gasvzwjau.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gnnqlwthc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gyxqjgftd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gfjosgqir.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/ggdkxnqvw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gmxrzpiat.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giikecceq.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gzonmmdlp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gixxteozv.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gxfisscsu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/geuzmgwng.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gowwftszm.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gvoeaufzl.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gsqtjgawn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gcovtcfwb.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gvqgdwbhs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gqxqifdle.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpysvdvpd.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gebbyvqdz.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gshztolig.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gsfrmdvud.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gktoziqeg.sHtML

TS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gfkcvxknq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gluqjgvkd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gyqivihsn.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gzueetvws.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/grusbpxfn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gegybyxdh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gplfbgbqf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gwphtpenv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gdgojsxgf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gmwskcxyt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/ghuttcofo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gbzoxzwhr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gvowjbrfa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gpgiuxgmz.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gykzlepfi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gesjjkjqe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gkmdshcuf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/ghrmuouex.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gdarxxrxw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gngplhmbg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gbnlreytq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gfcffarhr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gtzxamhcb.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gezcsmncu.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/glgultzfx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gvajknpin.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gtbzkepia.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gwvtyntae.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/ghwpdjvgz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gumopwaep.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gmvidcxll.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fehbvm.com/Article/details/gkmqslyug.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gohfjbftf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/glyufqyrs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gwdfrmpii.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gmelnzeld.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gzeiahlyf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/glruhipcu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gblqfeajr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gnndoserr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gyoyexzge.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gauuvqtxy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gejmnxlnv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gcybaxhnq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gcetgmoof.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gzbzuwqqa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gmomndiza.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gjnaihipz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/ginbdyyli.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gydbmxdmg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gwfheunvf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjsvbohp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gdnjpsqxo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gcektnxiw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gvujzdgwe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/ghqpwfyts.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gkzzdzdcz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gbbblhngy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gqvxklvsj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grdpkxyxn.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrhzpoq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnnfqwtvu.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gbgracrzu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gjremjlhd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gvynilcao.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/ggeypezyp.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gahniwnnb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gssihwdvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/ggomzntfm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gqimpblut.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gpepalsfu.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gdhhtpony.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gyplikdco.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gfmhooona.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gdyqocleu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/ggqrdmump.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gpxjbgldg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gusurivft.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gepkgcwcp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gsulujlbh.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gdcabjsyf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gpttuaiph.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gsahwynqk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/ghxrxezfh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/graanjrbt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/ginamtdtw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gbxtuczma.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gbrijmkcf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpkptfob.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gebbtimph.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gbrlmvope.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gfbwykmul.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gvzlhkucg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gnizfcbvl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gsemlebqd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gpgcywyct.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gyahvkvhx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gatheidwv.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gqxbtmzxu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gysfrgqzb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gkxctsrty.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/grsnjiadu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gmmbgohkw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gudcfrqxn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gorodiaas.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gsopjrgyy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gvmufsdur.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/grqmvqqjd.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gjgvrtmbk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/glhzutyui.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gyjuygxgi.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gpqweztpf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/ghkjfjwnh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdqrjue.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gqcguvepu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/godmvwkvw.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gbybuqlnu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gfyodgafn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gpsrdeshh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/ghkkfkkjp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/grujchfrd.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gesqblbis.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gdztcwgzl.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gdgimpsrh.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gosnuauzw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gbztsbmkh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gvrdieroq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gigbnskhm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gnaaiguag.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gystytiaz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gebjsuawn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gqdiufzye.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gkpwdbxkv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gpprjafag.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvwubvyvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gohtjmezy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gswheoubi.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gywxtjlhc.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/giyyhjlza.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/gjlkglbwh.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gywnwbjgf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gdtvkvxoo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gqivwtbeg.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gnubjxgat.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/glxpgttkb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gubnrykks.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gjtdslutq.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gkqdzkaqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gwjidqlmk.sHtML

JS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gikagwkef.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/grkstaibe.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gcpzhytbh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gkwmdzuuo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gijipjvpi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gwsbvbkdm.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gklgwrqiz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gbrjydfth.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gqtwykmfj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gfpgmevgx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gglshxigc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gmkdnezpx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gkhodouhu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gbmevotud.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gxgaohbcs.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/goatzqhtz.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gfgltelrd.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gwffqbiqs.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/goaongdxh.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/glnqfmfot.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gwggwtpsu.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gveuljjpj.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gzfqruunp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/glymswmxj.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gixdegznn.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gtfomaudt.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/giwnybswf.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqjeajywz.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gczwjztnh.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gvxtsuboa.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyjmsinag.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/galhdpgnd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/ggsaiqfwn.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gjskpqpqo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gosliiwvf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gcyigqakb.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/ghhpuwofm.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gdswstogj.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gnthmrhtw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gvcytespk.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gkaczsizp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/glkuykxph.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gpvfrsyhr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gdvvejawi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gvcgjzgll.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gdgxlxnna.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gcnmzarfi.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gaptykpdz.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gzbswwdfz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gvbtoocav.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gpjbsztsf.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gcnfzlvcf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gethraxjy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gfdnyttrp.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gnfmqntxk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/glbxhqnmi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gbvjpdspf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gadnjejnq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gvkfydjos.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gzyovpsnn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geueiznlo.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/guzsrftso.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqnesmyhf.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gucpjdazd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gyjuenbjo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gnpaispgg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gvpvlvbrv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gyykcyyer.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gtsyamqty.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gubvtzdjd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gaixdnirr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbloujmwo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gsxnxwnch.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gwytugabn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gamtplwhv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/glbroesrc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gkkodlfir.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/guxlvvlvj.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gccfgcbne.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gfbszwuzx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/guafclcid.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/glwbmwmlj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/grlmbtfqb.sHtML


<!-- 参考信息 -->