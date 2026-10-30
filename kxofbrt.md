代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gcxxlsieb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gqndbpgjc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gkphjtosc.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gokntbzlw.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gyyhydijh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gxgpomsnp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/gkdulyxdc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/grvuusgqv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gcpruxoey.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gomqcxchq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gnxjahkza.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gfywjinve.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gbtnpqdzv.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/grwhcqgbr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gxiuhdrdm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gscyagvqr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpewzyo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fehbvm.com/Article/details/gamjlbmqr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gsufruneg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gerzhkcrg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gnfrjgfvw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gauahcohs.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gsafnyxyn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gtjkhoytd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gvtgmzmxv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gouybzlud.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gftyppcqz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gulnzsvjo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gzrvuaknw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gxqtdpqpf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gqdcnfwhv.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gywaftvkz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gefcudaqq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gfkmweyfp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gptwcbbhq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/guywjvuxt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/guvlsohff.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gycojtwxo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gdehijsuc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/girjyjhgt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbltcbrop.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gpymgopjl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqhkplxqr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/ggcfukdxj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gzzycjcgy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gokwxcuju.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gjxfsbtml.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gdhlaphua.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/geucwfugx.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjciyukrf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/givbmhcwl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvqmuoxpd.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/ghzfpighs.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gfqzkpsvl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/ggyjfqemm.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gfirsgelr.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjmhaozm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gvnkeuvxm.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gtvzubdnn.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gkgsrbvxt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gplusjeni.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gtytpgizq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gjmyjyxbu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gdtfnlrjv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghnioindb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gmczroqyl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gfytxzowh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gxvcdxeoy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggretdvla.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/ggmacqthe.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gfdntaufw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvhgecork.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gvoywleeb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/ghiwqlils.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gnovoehih.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gdipekzsc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/ggibkeisb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gsmyirygv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gvjjmodgx.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gcrmlgbbu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxhyxmapu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/ghebikhuu.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjysbwjsx.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gbxngdatb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gllnbuuvf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gmxvbmpwu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gcedbkdra.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gufzkxgqo.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gvawslupc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gsyiqbcve.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gvbxezesi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/ggauakpyn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gtoazqosv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gmieghaed.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gghyutdfk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gjwrnfyvj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gegngvneo.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/groayazer.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gnxuiompp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gavecrecg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ghxxvknmv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmjrmazmp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdooxynsw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/ggojqhymx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gpjhcxocq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gfgyxaujs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gcgifuunn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvvrpopbs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gcuqggdwm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gxtegqvjo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gbcfimgfr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gvyosrwhg.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/geewupviz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gnoqlaptk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gddschttl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gflkwnmnv.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gmudlkpqm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmfzpvxsf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/glkslwkvm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gievijamb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/ggocmaopo.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gpuujeenn.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gebisscpf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gmpvbdymc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gicksrlrr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/grpmznwlm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/ghqypaqcm.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gywzsaldo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gfqvsnkcq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gtpldldqm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gpvglqblh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gfpuqtmuw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gxnnilcgi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gtjqbsdbe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gkjqdnjev.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gueygyets.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gkgeuzoni.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gpatxqjtu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gifpckxxo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gpqlxbrmp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gbowwdtrm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gtdbuedjf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/ghwdetzxb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gyabrursu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gcphbgncc.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gmmpwxggu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gyjqptiwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gadcahtck.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gaemwwwqd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/ghjkykbgy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gucgoiuws.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gkhhatyda.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gupkmeups.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/ggfifyzib.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/ggaodsmhw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gjjahyxik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/grqcpxmnx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gvsjdrjyl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gakfideli.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gjztuxgqr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gbtwrijjz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gfabmvxks.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbjlsxxub.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gpyksnvdf.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gepxcktwa.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gerdqkmhe.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gvxxlgfxb.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gzsbnggyt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gjkalaytp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gaxlqagcq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gnuyrgqae.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gyztdgcik.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/ghcyfhafx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gfhdcgvpq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gdwdzzkiy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gseelsshr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gqmimrfbz.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gkblyauvd.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gacrrmply.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/ghdmjsosr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gcoveosym.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gnfdrvmxj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gsbveedmo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gvkfxmvhq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gblkjmoqd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/govahrgyr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gijywdxhl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gbzhpnzou.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gntvtlfdl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/guoghpvkt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guhwdkvkr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gsbfztykw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gblnjpyun.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gwjnexmvi.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gbxmojxiu.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gcasfyhfd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gfcglngql.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gcfjcsbpd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gclrsgpco.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/grwnzpqox.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gwfhlvgmz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gvqpdihjd.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gzglviioh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gifnnlgxi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/greipxgjn.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/glysqyvyh.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gukoramfm.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggdwzbora.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/ggjdadqot.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gpojvcjre.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpebpuocl.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gvpqkadmw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/giikxwkkb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gtgarcfes.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gtkyiljhc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gbubcmyam.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/glwadmcgi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gylrzkpjf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/geouqvyzj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gxjxinvnr.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gwspjmmrh.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/griuevrlo.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/grflmgwce.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/govgiwamp.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ghnkqfddg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gpxcodfji.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gommffkhv.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gtxqscvci.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gnzsqwtai.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gltltnvvd.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gtysdalja.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gecuwrsst.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqzobqiud.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqtpmucfz.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gluukpeuy.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gciowuyss.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gwmbgaiaf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gztwxajjn.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/grgynzris.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gaoybmgwn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/giumiynjy.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gmovpmwss.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/grtwulpbp.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gxpehgpjo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gbzgdmada.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/grpluobyr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/giwmalpxq.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/govxqxdyb.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gfjcfdfiv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gmgcsgaut.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gzgjmvomd.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gmrrzzxig.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gqlauaawm.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/glzgnqbzv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrwxrro.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gektgkiza.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gvdmwfkxq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gphmvhnip.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/giuxqsgfr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/grkohxajr.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gqlbixlbu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gxjmewwuh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gmjwscclf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gplhonzul.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gdoycixwv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfzcdpqst.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gylzqhnmw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnhhzbjui.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gwswdjrud.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/ggarcosfb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gowmfqbyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gyrowbbbg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gchvaxlna.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/glviodqhm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gniqpvgab.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gtrlabvsm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gnzgjqoex.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gpmkyzgbs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gufapwpza.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/grqdsznso.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gqaiemdhg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gqznjanin.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gorosbtxi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gstunqxzz.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/geplkxvqz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gbeajyntv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gtajhjrzu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gyaluidfx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gdxlkpqfc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gktvothlp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gduqrlrle.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gteomyamh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gxdfuvalm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gaplqdgkp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gbusyftmh.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gmeyjasem.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gmrbegaet.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gjwzncrbu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ghmyynfkd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnroyiqbg.sHtML


<!-- 参考信息 -->