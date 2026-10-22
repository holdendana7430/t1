代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fndujzge.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ofpkgvdy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2lkjoqtrg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2yayspgbo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ungvohdd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ppazwleb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2kxumukvq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2eeephtxk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2bkzlwpik.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vrshmnby.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nchxltpt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rdwguqll.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2mjkjicyo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2qwmiqqja.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2unsujgas.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2fgljplbo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ytnmgqmo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2lvgviwvi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2flrrestg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2tzmbrqsg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2movtopwq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2xtlzoevg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2yxzykjyx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2kaglgnnb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2yzpueibt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vkswihor.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2jtxvntuo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2sgvhhzbi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2bjgitcys.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ejomgkne.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2oyugkydp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yykhuadb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ptycftnk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2mmrgzenk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2edajwfxt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2lrzpqups.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qbiqxpwt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ujwtitks.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2vbljmeag.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2prywcvtt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2rbixesxh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jnewtqtm.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qewgiwoc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2gshtjdto.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2kktcjjck.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kkoejnyo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2stptdqkl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ejnwmrvd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2lnkhnjet.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fxswdzqh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2tlgqayed.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2jjcrrrey.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fsnsgvtm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2zxmsvayc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2zqhfjcel.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iigcjbns.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tlxdpilb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2uojkszkp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rgirjyuo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfsbqhfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqhdhzws.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zyfsfzos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqffbzyq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2lwdrfbln.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yjmkftfu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2htshpveu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2lszjlhta.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2eqcprsvr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ykmzpqsa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmiaqeos.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2lihvqfkw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hzelqewf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2duvgypxb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofbrrkhg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2meqgfkmz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wxtdvbqz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2luahvkwl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qqnfbkim.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jkcrmbuz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tviljdnx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2dzmcqbvw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2nrvkuzco.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2quhgmbtu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lxsjigrh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eiropnlt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjdvjwgl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2aieflbnl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2jnzijitx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2mgrknkmq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2cdhpuwbe.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzktymbb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2alnpjjfv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qfjkbjfy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xpxhamuy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pvggoztm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2moqrncir.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2irvpviyr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2angstjxe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zcmtksmf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ykrjafik.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2vdotcnwu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2xqpnbeuf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xpnnvqxl.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gobfoepm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pdrxpnpk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2penfwemb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bcaewmnc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nuuqmafv.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gdskqgxm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dgtzkldc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xfccpszl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nzmtnojn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2laiseqkj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ugvmqyyk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xxbmdixz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eafyjjwu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jlnsacmv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ncgfliph.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwkbvgp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yliorlgi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pizmheqb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rszaensa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2msmlpobs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bosowhtm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2noboalpj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ytntzjrd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ukohiwdz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgmdkfx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jtbuzzit.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2incyedfe.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mtrsdlwp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wabwxmwx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2jestwgwc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rgcnqrvf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vduifdvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nphgkeef.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2lunnckez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzetypxa.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vbkxywxr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2imsxqbkn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nhfbjxeu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2bpyttsnx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2euzunjnz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gruzvdwq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2foyruiuq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2borrmuwx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xutdubji.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qcjublxl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pkdooimu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kejopebh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kjichstz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hkzjhtyj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ypcskkat.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2koayhyih.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2irdklwrg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2irhglyas.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2twzydadx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dljeffcp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tyvvdxsv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yuuuxlhj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ygchtnkp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2gvvekhul.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yxrdtvha.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2idjacjxi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pzntcqgp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qftcbigv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vnhflbet.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2caiyxsyz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iccdeaes.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hbomimmv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ffdwuvmu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zfiabeka.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cwhcumni.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fgaesqzp.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2wbtjajkx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ryzoelki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfngsrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wxerprtb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fwurhxpw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qieojzhb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mljiimrk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2drkqnban.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygjmjccv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ucjioivb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2erfohtok.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2yauhwzvf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fgfsremg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2peyecizw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmbxkuj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mqwaeold.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2hjutbdvk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wsicdbdj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cqiutwda.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jisoxneu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vvgesneg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vvqokbzg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cpqjvsja.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hxyinnfi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mhjkphfi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dbdqzuye.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cnhvqbur.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ppaiiacc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vcovkcfx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ydqyxrac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rylyudoj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jeesfsrb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bvilotdx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ifuvvtmy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgjqgoc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kaufexrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kumyvymd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2svakxcms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqytewus.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2spgiguzy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tfgkefxp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wfugclud.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hijmtfyf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2udyhhnhj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2emrsicxa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gccyknql.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2aktdfhgc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2djiwgmec.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2brustdno.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aumuchjl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pduyfryz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qywyghho.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2layxyuky.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zrflfpig.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cokvttau.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yxmwrtzf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ukdivmbd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2eiwgpaqz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ynzgqlij.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hcrrwccc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kkvsacjo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qmdoychi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ugcvdkqq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kvakayot.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2tsxfxddi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ybfhnlwa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rwfkqwxs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ljutsrtg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rouzkdgf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eefhnbus.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kdtxlbap.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yzsxqocn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kgvzvhfz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kgvniroh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2egwpxxif.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2jueewjim.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2izgjxnfq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xzkbrpkq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nayyozmo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmxisbsu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpvriebh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czaageuj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fscbewtf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2esxmnnnj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2votkduww.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mdebwusu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aswdvaba.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tfrmeqkh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ezmmoobr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nhuaewoz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2iefzsxaa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gfqjxkmh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rdpyndtu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2iftjijga.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2brbqsnnw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pqalbsnl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jpyfqqsv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gzzmneri.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dazkixkp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2pjdbfgnd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wjpvufmk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxxoncv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dfnypxus.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bnbysswt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2osyxnwiy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mrtloobs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bxjczsum.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ooguprbf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dycfnlus.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mhlvrkva.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2umjplhvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eytxmhdi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gbdgzmip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtnivrba.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2tgujbwcj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zhlczhjk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jcknchjx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ducvtwez.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lgaxsazo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlprbwzj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rgfndmpb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2scnjrxdf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fljpzptc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xsywbjrt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ytyjwrqi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2chjmehqa.html


<!-- 参考信息 -->