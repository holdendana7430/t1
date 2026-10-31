代发 wailian999

J. 日期与时间
来源：http://kw.haigaiapp.cn

================================================================================
来源：http://dg.hnjuh.cn

[J01] 获取当前时间
来源：http://zs.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://th.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zb.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://yu.hahajie.cn

TS:   new Date();  Date.now()
来源：http://jy.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rn.muxihuayi.cn

Go:   time.Now()
来源：http://bk.hahajie.cn

Ruby: Time.now
来源：http://ea.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bv.huanxung.cn

[J02] 格式化输出
来源：http://mb.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cg.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jc.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uf.bjjhwx.cn

TS:   d.toISOString()
来源：http://ax.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sj.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fm.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qi.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lt.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://qq.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eu.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ef.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://ur.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://gy.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xm.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fq.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://bc.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zm.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://ds.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ei.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ly.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wx.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xx.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ir.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wm.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rq.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bm.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://zb.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://vo.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://av.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ou.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fh.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://zu.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://be.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://df.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ll.chemitech.net.cn

[J06] 计算两时间之差
来源：http://df.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://me.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://cy.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bh.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mv.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jp.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://bc.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://rx.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://ws.lnxyls.cn

[J07] 比较两个日期
来源：http://qc.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://mq.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xg.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ue.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hx.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nu.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kt.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zx.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://ma.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://za.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mq.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ik.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ig.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fv.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fi.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bq.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ls.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wj.huixinmuqiang.cn

[J09] 时区处理
来源：http://xb.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ho.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hd.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rb.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wo.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ds.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ko.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kn.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://af.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://nf.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vm.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rp.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iz.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kt.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mg.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nb.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vw.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ph.gzmigu.cn

================================================================================
来源：http://zh.szxytkj.cn

K. JSON 与序列化
来源：http://yc.yuntaijiaju.cn

================================================================================
来源：http://xw.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://ip.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qo.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uv.521024.cn

JS:   JSON.stringify(obj)
来源：http://as.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://zq.huixinmuqiang.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vg.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://yn.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tg.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zh.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://dg.bookmarksfly.cn

Py:   json.loads(s)
来源：http://ho.wgjwhj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xw.shtwfgs.cn

JS:   JSON.parse(s)
来源：http://fi.asd995.cn

TS:   JSON.parse(s)
来源：http://xw.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://an.yuexingan06.cn

Go:   json.Unmarshal(data, &v)
来源：http://sx.shtwfgs.cn

Ruby: JSON.parse(s)
来源：http://df.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ar.lnxyls.cn

[K03] JSON 美化输出（带缩进）
来源：http://bu.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ed.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fo.shxzukj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ow.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hf.colortex.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://my.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qq.shxzskj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tl.szxytkj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cf.shxzukj.cn

[K04] 读取 JSON 文件
来源：http://dh.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tu.nicolike.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nm.huanxung.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dd.colortex.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zc.jctech888.com.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iq.hahajie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nb.muxihuayi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://we.chemitech.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mg.yuntaijiaju.cn

[K05] 深拷贝对象
来源：http://ed.newstarts.cn

Py:   copy.deepcopy(obj)
来源：http://of.9csxet.cn

PHP:  unserialize(serialize($obj));
来源：http://uy.gzmigu.cn

JS:   structuredClone(obj)
来源：http://il.hnjuh.cn

TS:   structuredClone(obj)
来源：http://fi.szxytkj.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vf.colortex.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dr.huixinmuqiang.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://na.chemitech.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nf.9csxet.cn

[K06] 解析 URL 查询串
来源：http://hz.9csxet.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bv.shxzskj.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dr.asd995.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zy.szxytkj.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cf.lnxyls.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ip.yuexingan06.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vh.nszjky.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vv.shxzskj.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rc.nicolike.cn

[K07] 进制转换
来源：http://vt.chemitech.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cf.nszjky.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mh.hnjuh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ri.muxihuayi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wh.shtwfgs.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mh.yuexingan06.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ek.hnjuh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wt.9csxet.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ib.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://tz.huanxung.cn

Py:   pickle.dumps(obj)
来源：http://sr.jianghongdianzi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fe.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://vz.bookmarksfly.cn

TS:   v8.serialize(obj)        // Node
来源：http://eq.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rx.haigaiapp.cn

Go:   encoding/gob
来源：http://pl.huanxung.cn

Ruby: Marshal.dump(obj)
来源：http://mn.bjjhwx.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ou.haigaiapp.cn

================================================================================
来源：http://nv.nicolike.cn

L. 网络请求
来源：http://kj.szsharing.cn

================================================================================
来源：http://nx.521024.cn

[L01] 发送 GET 请求
来源：http://dz.huanxung.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tz.panjiajie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fc.521024.cn

JS:   await fetch(url)
来源：http://ns.bookmarksfly.cn

TS:   await fetch(url)
来源：http://qm.szxytkj.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hk.bjjhwx.cn

Go:   resp, err := http.Get(url)
来源：http://al.shxzukj.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fj.wgjwhj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://je.bookmarksfly.cn

[L02] 发送 POST JSON
来源：http://xm.szxytkj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dh.asd995.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ny.jctech888.com.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ds.521024.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mb.huixiangedu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jf.colortex.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pz.hahajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rw.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rz.nszjky.cn

[L03] 设置自定义请求头
来源：http://ox.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wg.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gv.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ho.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wy.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ji.9csxet.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tz.yuntaijiaju.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kb.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hd.yuntaijiaju.cn

[L04] 设置超时
来源：http://gk.shxzskj.cn

Py:   requests.get(url, timeout=5)
来源：http://kv.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xh.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oa.hahajie.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ak.bjjhwx.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mh.yuntaijiaju.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hs.szsharing.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wv.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eu.shxzukj.cn

[L05] 上传文件（multipart）
来源：http://nt.asd995.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pm.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cz.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ei.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://po.nicolike.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ig.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ft.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://or.nszjky.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qq.hnjuh.cn

[L06] 解析响应为 JSON
来源：http://hd.nicolike.cn

Py:   resp.json()
来源：http://kk.521024.cn

PHP:  json_decode($body, true);
来源：http://qg.hnjuh.cn

JS:   await resp.json()
来源：http://dp.shxzskj.cn

TS:   await resp.json()
来源：http://km.shtwfgs.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uj.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ke.asd995.cn

Ruby: JSON.parse(resp.body)
来源：http://ql.chemitech.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zf.9csxet.cn

[L07] 处理 HTTP 状态码
来源：http://ob.bookmarksfly.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pb.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://om.521024.cn

JS:   resp.ok;  resp.status
来源：http://oa.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://lt.bookmarksfly.cn

Java: resp.statusCode()
来源：http://vg.jctech888.com.cn

Go:   resp.StatusCode
来源：http://ik.huixiangedu.cn

Ruby: resp.code.to_i
来源：http://qb.chemitech.net.cn

C#:   (int)resp.StatusCode
来源：http://fc.521024.cn

[L08] 并发请求多个地址
来源：http://js.wgjwhj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cb.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://yz.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fl.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hu.hahajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zg.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gv.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vy.gzmigu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nm.chemitech.net.cn

================================================================================
来源：http://ty.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://ky.shxzukj.cn

================================================================================
来源：http://pj.shxzskj.cn

[M01] 读取命令行参数
来源：http://gc.nszjky.cn

Py:   sys.argv[1:]
来源：http://ua.huanxung.cn

PHP:  $argv;  $argc;
来源：http://bf.nszjky.cn

JS:   process.argv.slice(2)
来源：http://am.szxytkj.cn

TS:   process.argv.slice(2)
来源：http://qq.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://zg.yuexingan06.cn

Go:   os.Args[1:]
来源：http://io.jianghongdianzi.cn

Ruby: ARGV
来源：http://vc.chemitech.net.cn

C#:   args 数组（Main 方法参数）
来源：http://jp.szxytkj.cn

[M02] 读取环境变量
来源：http://vo.colortex.cn

Py:   os.environ.get("HOME")
来源：http://di.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pb.lnxyls.cn

JS:   process.env.HOME
来源：http://vx.nszjky.cn

TS:   process.env.HOME
来源：http://ow.9csxet.cn

Java: System.getenv("HOME")
来源：http://xv.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gx.newstarts.cn

Ruby: ENV["HOME"]
来源：http://ex.gzmigu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ji.nszjky.cn

[M03] 执行外部命令
来源：http://gl.szsharing.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://we.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yu.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qt.bookmarksfly.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://os.shxzukj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eg.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xm.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hp.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://xs.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://jf.huixiangedu.cn

Py:   os.getcwd()
来源：http://th.szxytkj.cn

PHP:  getcwd();
来源：http://vp.bookmarksfly.cn

JS:   process.cwd()
来源：http://vo.huanxung.cn

TS:   process.cwd()
来源：http://sl.szsharing.cn

Java: Path.of("").toAbsolutePath()
来源：http://db.chemitech.net.cn

Go:   os.Getwd()
来源：http://ny.jctech888.com.cn

Ruby: Dir.pwd
来源：http://au.huanxung.cn

C#:   Directory.GetCurrentDirectory()
来源：http://le.hnjuh.cn

[M05] 设置退出码
来源：http://gm.shtwfgs.cn

Py:   sys.exit(1)
来源：http://gm.521024.cn

PHP:  exit(1);
来源：http://tj.bookmarksfly.cn

JS:   process.exit(1)
来源：http://td.9csxet.cn

TS:   process.exit(1)
来源：http://qr.huixinmuqiang.cn

Java: System.exit(1)
来源：http://pj.bookmarksfly.cn

Go:   os.Exit(1)
来源：http://bl.haigaiapp.cn

Ruby: exit 1
来源：http://sf.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dt.muxihuayi.cn

[M06] 向标准错误输出
来源：http://gm.nicolike.cn

Py:   print("err", file=sys.stderr)
来源：http://xa.muxihuayi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bw.hahajie.cn

JS:   console.error("err")
来源：http://so.521024.cn

TS:   console.error("err")
来源：http://vk.nicolike.cn

Java: System.err.println("err")
来源：http://mt.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qc.yuexingan06.cn

Ruby: warn "err"
来源：http://uz.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://op.521024.cn

[M07] 判断是否为主入口
来源：http://qb.hnjuh.cn


<!-- 参考信息 -->