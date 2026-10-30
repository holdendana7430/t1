代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gykyeufjs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gqmzvgdqk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/gzaffgdng.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gbbaaijwu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gyskwazsw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gfjitipoc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gstkhqxyl.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gzqebyduq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gvjuyfble.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gcnpoelqn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gmvqnvocr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.hesvh.cn/Article/details/gappeldca.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gcarsvqvk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gfcaxsnff.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzyvvvxb.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gtburfnki.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gaxgeevsy.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/giekxnjbj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gapxhyqug.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/gxscomcpb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/geykftnms.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gathvmwxm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/geummnpnz.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/ghkvofwvg.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/glegjohmd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gmfaczhmc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/glvjaeebz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/ghzoshzmy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gnkbqpent.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gxrkicyhr.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/genclswtl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gswqhxfnu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gkallsejo.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gfxkomopl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gjntosfcp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gpfmwekzg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gowlegkyl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gurwxqtcl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/glnouleok.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gdzuvbtni.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/guxkcwntl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/ghhhpwtbi.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gytokeoof.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/geyvewmuh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gartwrhid.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gdljfpvse.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/ghfbdzqxe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gskgaptkp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gnjuhomwd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/ggrduetgq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gkutkebaj.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fehbvm.com/Article/details/gksbhgrts.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gdszufoen.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/ggvfsxvbr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gqranqeta.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gekmlgcjf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gljucvlof.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gwamoehdo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gcqenltvf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gtsoaumzh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghahnmpdl.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gdpowpcds.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmtrhdkkl.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/goxotsyad.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gyowiczzh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gavggwkzw.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gzfsaenbe.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkfarizzs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/ghwydrkyv.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gcvdxpqyr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gyfvvdvcf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxolezosf.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gfaxsmenu.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gjtimqaln.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gtszquwxg.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gklgquyhg.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gxtvqxdmx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gumnoomkx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gvvwttkfu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghfryxrbp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gfsrffcjo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/grkvuvjmp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gucfeuize.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmpxmmeqt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gnzgprpes.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/giyqgddno.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gippbqbos.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gmifdawjw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkiqhypyr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gdwjvigqu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gkukxpleq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/giifcqhey.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gupqwkzie.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gtjjhbmcg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/givqkmbvh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.fehbvm.com/Article/details/gzgsywlqx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gllzmdlsk.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gbkjhwyfp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gwfpyxbhl.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gytnpdevp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/glcklbsoj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gqniakfuc.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gpaqkagjf.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzwvutuoe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gtunniawb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gqxhxyjyo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gvnzhgbpj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gkbmmjhxe.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.zdbjq.cn/Article/details/guyqbwxty.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gtgygjfkm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gmiqigyse.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gbjpdxuzf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gxmkpivwy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gxzxhpjih.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gofktenmx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/getvfoenq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/giaxzwtbf.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gjgqskyzw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/givbhfqwc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gklsxkugk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gnfmbqcpu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/giiimqiqh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gbxhoamzc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gnrfsyekz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gmjzzqfko.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gwzoygcfn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gvnqzlurx.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/ghrokthuh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gzkeladrf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gguohgwlk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gfdotdgxs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gkxwdrcbx.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/grzxlbrvv.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gnnobqpos.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/grmjkgylj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggdfqiyok.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gslxpamyq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gttnroopd.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gixdrlxoj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/grdooytgz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gmvucdmkv.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gxstgbijv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzchlwrb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gtrflnqoc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gmnchqgye.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gjzgytpyj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gapdcekfi.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gmdgrenwy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gfqislxup.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gcxtyiivr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gbddzewnm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gptpsizll.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gtyepjqyd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gauqebnae.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/ghwxzgmqs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/goznjmdzk.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/ggqozavnp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gexhflvyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gjtumnook.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/ghmhkyyiu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/glamdmpjr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gqdkycpzk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gndjnfyju.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/glzxevnlh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gekhajjfm.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gbmhprege.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/geecgsizg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gkevyagtr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gfanswexo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gbzmmykbc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/ggxvrntax.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gaqfyqnsk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/giotlarxk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/geduztict.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gggfqugst.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gprmzprtb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gnoanfqfx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gaowxtokc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxdtujxcu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gvgxqowhy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gwbfqziol.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/girgbmjdi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/ggmvuihvt.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gdtrkgcea.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gjrfsjcix.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gygpimcig.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gpheysrtm.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gwifvfklt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gxxtpylxb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/garcclztl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gdstkkmlu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gvlqtdgwj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gqdtqxind.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gwceygkla.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/glxnaprbf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gxgwezowg.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gqprhjcfi.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gsmxkwrff.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/geioattsd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/geogfmwss.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gexlsdyaw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gklnhuwxy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gixujeuuw.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gqctcmipj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gsohlugya.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gpvfpaqvs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gizyjxhyg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gbefnqadd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gctmbvfrx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gbelavbiy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpkirmida.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gfpridhnr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gskfkdfil.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gpennhbfj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/ggvdzsllx.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/glzguiuon.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gwdswhbuw.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gywyuzjgx.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gvuaidvqn.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gyvpsbxvc.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gsmsunayo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/glvcrkkmt.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gvrnlierh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghdqcosnp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gaqmranwe.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gdmgavykl.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gqhntmzzt.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/geffynucr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gltcmapja.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gyypfunpe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfxzorwdg.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gmzpalgwg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gezryklhy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gpjlguejg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gjbxctsil.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gidtlsgiz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gqzjrchzz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gbywberzi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/ghcwjwvby.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/goqngxbys.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gpgdizkqq.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gygteqpax.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gcxrtfswg.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gscohsdrk.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gdhszncvz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gtflfgqpk.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gvcnhfkph.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gtezqjgfw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/glvzuyach.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gbpattwyk.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdxmngtlv.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gsxbalama.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsccsbydt.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/getwqlesy.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gnutdxlli.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gupgdixie.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkmzruriz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gkufgjhpp.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/geezlzxev.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gvjhwadio.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gvbsxfbvx.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gqexfvhgd.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gczglopfk.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gbwmjebtv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvsdvned.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/grdrlwpwb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gscafxkxy.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gqyrqovqq.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gabrpgjri.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gzfztmuqo.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/ghgqnumjk.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gulihsoay.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gtahcxiff.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gqdxhugmh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gycyzcsvo.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gvlqrywmq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gkclbtnwm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gybkqpmgu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gxpbspxec.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gqdurlvsr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gqhchtjpu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gkzygpfxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/ghiiptjbb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gxmonzioq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gdaegybii.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsenokibn.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/geuziehgi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnrivhejl.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gyfjbklmr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/grvmihblw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gokfagksw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/grhblfkru.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gdinuifyk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gznuqjpjp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gysqzfvhr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gvgvqmfrg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gaadfttxw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gvyhutjom.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gtugunsna.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gsgtkpjku.sHtML


<!-- 参考信息 -->