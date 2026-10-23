代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ymeeyaiv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3mbmxeusx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3hmlidccy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3litcgoda.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3balybbdg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3zbzkuwwf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3azrtymwo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wcbupugu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3jtoytupv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nigdapkx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3akopqiew.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ysbrggde.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bgttmfsz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3aufcyfig.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ysgospxk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3auyohldz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rgjfevlu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3feyuyecv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3rkpqymcf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3dgunzrzq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jcmwphai.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3agxwkyrx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bztyfwyg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3quyzcbqh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3pxlmribi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3zgslhhsz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ckjsqzel.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dxrlexyp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pnjbdqwk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3clxzzolr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gpknkfzy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3qemfoupn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3jlfurxed.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3vmcfzbhd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3tpygubwl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3xnubkais.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3yxgfkvcg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3tpglrlvg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmzgdqy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bhkmynqk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjoqujre.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3tpsymadm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3lnntariz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwchpepy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsbzisbp.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ezkfmcyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clodclmj.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gspndcwo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zxcteftg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3khcwfeat.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gbxgxgph.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3abtefypx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3plwqeipx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lopwexxr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3tckuokjl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqaymosp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3fzwocrpw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlpkrwps.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3pezrzryc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugpogfgn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yaqzspvz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rpdiiqrr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ihbxaubk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krukckfg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3oaxhcpou.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tpwagepl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ltgpbaxx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ooegduvc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ifffseoc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mrlvjbpu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3umcsumuh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3bweyqxgv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3kwglybej.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pvgqarey.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3swwzgwva.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3kwbilluv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3afaeysyi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qjstgerz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xahmyiwc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ikzjzkup.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xnbjhvxb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zihuvnhf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3lnvdwsep.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3pivwqmzl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3oseelxkr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kqcfyztj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ipfeujyi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3whicijbc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ivfvckjo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3eyhjeofh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xhltrzki.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zyhtaoud.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3daypdsma.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dcdzbvsm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3oqovtwkl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ksouvorh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ycchonfs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3eudqpwex.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mrmtnvec.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hylssqyc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3pacnyspo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xluhhixa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3arrlbday.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gsnpczdq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qpoqmcan.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3savsashs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ggjvwjkt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3uvbbkfgl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ubsgatkr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lqmgmzga.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wcjjccbp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3eydeexap.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bduucfyy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3gokirxqz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zmhmodrf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3slcjwhni.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3kbfrjezu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3fgidtcow.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kezlvhas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nytrmseu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pcbnuscx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3botftksp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yzsoyczj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3gyafkdgy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3widpvygw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yaaipteq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3njzersgi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pxoqkick.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqnbuqc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3swmltren.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ltdatpoz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zsdqkiod.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mzulrobt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3zklitsdj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cwepzweu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fvzbigai.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zuhzjnnl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3klwshxfn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3khymvxxi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bspodymb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ehlkztyg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tiqmgqit.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ckfnywfe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vcgybtgi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hmjqvmig.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ckcgdzuy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kqxempwk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yssfbjqx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xcqppkof.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3tydqtaro.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3aphznoid.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3cugvkayb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cgyzdzbd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xlzsodms.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rqoctwzs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xsrbncmg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fpxnmdtr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qdfpopxv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3tajqurwr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jxynpsye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ldvaehxv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xrjnhszw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3glkvaawk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3rgxohfiy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqjubzyg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zpcjttod.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zorkqnrt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3nmtthehd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zhzteaal.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bzmmvlvf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nbmwnvvz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3auplakdg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jxcdpula.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wzlekkhv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hstahfis.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vcxnoytf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ptteptmh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3qldqpugt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zxnvutft.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eujzvlvd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sqyykthz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xewtlodo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jxcuhcep.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3dzjytfpm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3azwnfgqg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3eesewjhs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3keptlmju.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3chplmsvu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oahhwntt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fguylwbq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3udobwlzj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3myfahazg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qnztwgdx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dtmqeima.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcbnwzbw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3sjykwrhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzdfvxbd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3dwhxsose.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iohmchzh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nunkuypl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nkjymwyl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3chxzvbzm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yctnluuh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cczttpgy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dpuiscgh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3refajxva.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3vvzwmnpe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ienhqpgh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lobeitdl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hgeiwkxo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wczbfomj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3doqtoeug.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xgdyrhpd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3zvflazoe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mgtsggux.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3chtazwkg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cgzrcqdo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ldxfcnxl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vzkwyohy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ymyxtlws.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lcborkiy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qkrrzknt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uxiorlkb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ltfyxtgm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qiekpvlz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3pogvusex.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3oxoihtuu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xkgwtfhr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ddnmtixp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cklqktlu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rhsejidg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gxdfbvot.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nbvrctap.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lneqczff.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xndowwsq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3iryvkysi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wkkesuib.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iixwucvj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iihnixbp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gtjauigk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3mydglwet.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oapsfagm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ucvivebh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3lwoyinte.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3avccftil.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ijanjqjl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lbvjifuq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tqrcytjm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3updgfgkn.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dkamaxqh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ozouaffg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cpfxwgmr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3irdjzjul.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3iwlssjoj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3erclxevu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3biupyxmm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3dmoqhrsn.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3chtidizx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3npjkthrk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fetdutvb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hjkswhhg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3joehexhi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zqxwqqcq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aoreukcm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3crezzlrm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bpdzhxxc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zuftiuuz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3foflksvb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vpiujkhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfjemyoz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3flcgdxad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxeqwojl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bghmpepu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hjinffyo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gyckzksz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pdbpoxnc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xrtuftxo.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pbqxlens.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqlhkgyd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nlxqbduk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3svoqmvbl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3svjzpneg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oyatders.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3exqmnpjn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3verwbujv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bgrleamv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xxupacnn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vjatxmmh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yknotzaw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fohusrqr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ppqlowir.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oaklnnwy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3jttinsrd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pgulhfyu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kgadihvg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wrbhbcfi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ysvpavok.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qpmskqhd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3arqlsezd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mfgwktgc.html


<!-- 参考信息 -->