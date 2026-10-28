代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtxaoxbura.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtfkrbnabk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhongyouzk.top/gtnituqfkg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gtqemehiql.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pengpengdd.cyou/gtqhijjfjz.html

Go:   end.Sub(start).Hours()
来源：http://hz.redwolf501.top/gtmhpqnsio.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydjk.org.cn/gtgwjaqdte.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtanjiwzsn.html

[J07] 比较两个日期
来源：http://hz.316326.xyz/gtjxzcmctx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtotdciftt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtmuoqlovs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtxoppfnyc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtielnqgml.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtunwiszej.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenjidiqi.icu/gtfblxylgg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gttosalbwt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtqxuxatfi.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtcdgqnqeg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnqzz.top/gtrqsgngko.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtritfwsea.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhoulong.xyz/gtynplgvan.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtglyeibau.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gttjteljqw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtdnobshex.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.9152youxi.cn/gtvxghfjuv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gttjncdhjy.html

[J09] 时区处理
来源：http://hz.nwbrower.top/gtbkypools.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gttvtwxejx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtenksoatx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtihplkqzt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtadischge.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtkxlxxzqr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtfpiaurbc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtqimvtqhz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zycfv.cn/gtjvhgpuwh.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtoongifya.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zycfv.cn/gtoaoqhhzb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cashguo.top/gttwsneedd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.9152youxi.cn/gtjxynfrvr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gthzeuxtwn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtjqzczwvl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtwwkzzaxi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenlongwang.top/gtxmrwibob.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtovncmwfe.html

================================================================================
来源：http://hz.chenlongwang.top/gtmpyqzfcf.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gtefezpzyu.html

================================================================================
来源：http://hz.chenzaomai.com/gtxgdzheig.html

[K01] 对象转 JSON 字符串
来源：http://hz.sweek.top/gtfkgbjmdc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtnkwnfpcw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtogfkebvo.html

JS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtkdatyvof.html

TS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtdbkfjyuy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aizwys.cn/gtuswmcymi.html

Go:   json.Marshal(obj)
来源：http://hz.xuetiantiany.cn/gtmehfzguq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hammf.cn/gtedfejpuh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtrjewdguq.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtfaoyzofx.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gtafgvkwdn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtpxfbaywf.html

JS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtynchhxcb.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtbzdsqxty.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenlongwang.top/gtdbjuecnv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtbujeykzk.html

Ruby: JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtnrrhioya.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtejvbgcun.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenjidiqi.icu/gtvxoxchnn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtgltiuueo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtpynycuqa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtzeccqtjb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtmintfejv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gtkcxaelui.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fzhhl.top/gtzcikyuvw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtebtbhlfk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gzhubu.top/gtzghpuntm.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtngmsvjmf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.0kj1m.cn/gtbfmfjacq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtapxtveet.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtkrbktqjj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtqxuwiowq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gtdlqpnten.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtvzbkrisx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtdbnrspsh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gzhubu.top/gtfwnbrlzl.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtnyltsvgn.html

Py:   copy.deepcopy(obj)
来源：http://hz.zycfv.cn/gtujnnjrgh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gtdhryfwld.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtlowstanu.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtvibrvjhb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangshuangyany.cn/gttopigncs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guowangkeji.top/gteojbcdym.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sufxvd.cn/gtqhjibaxr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinghuilouyu.cn/gtlmliiywe.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtvhxtiyhz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtwobbmtct.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zycfv.cn/gtytmjnojr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtrcceksvu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtbqwarwop.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sxryk.cn/gtjfpmatsc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtykqrwpfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtjulaszek.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gtbvkpctqx.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtlbgumipg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtvrfxkmcb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtycwvkjqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtskoggwxz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtylutcjpg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtjgtdvtmd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtlyqpazsf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtdpjdgery.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gttdpvytqs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtnmmlyeoi.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtbtspwsin.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.snrcjt.cn/gtnthoavrd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtjywzxiua.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtuhzueznh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinyuanbaomall.cn/gtflzlfasd.html

Go:   encoding/gob
来源：http://hz.0kj1m.cn/gtnwalcoig.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtpentnous.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.9152youxi.cn/gtofaxkmoy.html

================================================================================
来源：http://hz.tian-w.cn/gthqctcqsq.html

L. 网络请求
来源：http://hz.aibaodan.cn/gtdwyvhtln.html

================================================================================
来源：http://hz.9152youxi.cn/gtnjkntcma.html

[L01] 发送 GET 请求
来源：http://hz.tanke756.top/gtpfetpdbs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtwtoahlzf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtlhzczkml.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtmdzeknqp.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtndnrtuan.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtnadlzyoz.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gtruzaedbt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtxyoaihqn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtqfahqbjc.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtrufatnwg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenjidiqi.icu/gtqiegzkvw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtleumardp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtjusiycqz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtzgapfrce.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigfzy.top/gtsojtzevf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pengpengdd.cyou/gtefxnzall.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj202588.top/gtieouilzy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtyfqrbhrs.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtavqqgwga.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gaohongyu789.top/gtfdenmzoz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtsmntqnfi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtoxcineuf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtcsmdlzgz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhongyouzk.top/gtaisdpjpq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj202588.top/gtyztrhnfx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shzxlz.cn/gteatnlprq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sxryk.cn/gtdgibblrx.html

[L04] 设置超时
来源：http://hz.tanke756.top/gtmhjvmpqb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtudyswuen.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtyavyuvhd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtvcfdnipp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtjmbrsdpo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtbvpedven.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zycfv.cn/gtkgjxncvc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ywan-chungtsiang.top/gtroeyzkix.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xingfuxueyuan.xyz/gtywzoqeqr.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtdvhvubga.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtfzhfwvqg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtdhzjzjwp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtqwwxmhbo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtjsejrxny.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydzc1.top/gtbzpferoq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuanzx.com/gtrzbmnmte.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gaohongyu789.top/gtrkouosmd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gthcojwsoe.html

[L06] 解析响应为 JSON
来源：http://hz.xingfuxueyuan.xyz/gtleemlftl.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtvlqjxvae.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gtalnpotfr.html

JS:   await resp.json()
来源：http://hz.yuanzhike.top/gtcpmipujj.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtcxbpozcn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtpvaqsdjv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gtciximxka.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gticenyyvk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtqtisfbyf.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenjidiqi.icu/gtxigzayzg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtnivnilbt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtjohdtaxc.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtgiylcqqk.html

TS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtvajgqpfl.html

Java: resp.statusCode()
来源：http://hz.ehwqpu.com/gtihnwqvap.html

Go:   resp.StatusCode
来源：http://hz.mhx1999.top/gtbguyxnak.html

Ruby: resp.code.to_i
来源：http://hz.jqgufenzy.top/gtgjvnsvkv.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtlumqkovs.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtjvvfjxdm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hfpthk.cn/gtyxsozlof.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtffaxuwms.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtgpgwgwey.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtkrvmzlvw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuanzx.com/gtoyepvigf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.mhx1999.top/gtiilqktpz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydzc1.top/gtwihwckgq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ehwqpu.com/gtwsydagmq.html

================================================================================
来源：http://hz.sufxvd.cn/gtrwqyaosq.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtrekyxhfm.html

================================================================================
来源：http://hz.jiagoushi.top/gtpukpdkli.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtnvxwkesn.html

Py:   sys.argv[1:]
来源：http://hz.meibo888.top/gtdmcvlshk.html

PHP:  $argv;  $argc;
来源：http://hz.xinyue.icu/gtzepvmmtk.html

JS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtqkehgvkm.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtsuwucwcm.html

Java: args 数组（main 方法参数）
来源：http://hz.vqdsnc.cn/gtfswtlqyf.html

Go:   os.Args[1:]
来源：http://hz.yuanzhike.top/gtjwlvxtzw.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtwmbcflbv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnqzz.top/gtssfxwsrc.html

[M02] 读取环境变量
来源：http://hz.feifeiyinyue.top/gtpqydyuyl.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtduxmzryj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.feifeiyinyue.top/gtlydxxyly.html

JS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtnbfbqycm.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtujxraxff.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gtwwzhwyto.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinghuilouyu.cn/gtjewrowft.html

Ruby: ENV["HOME"]
来源：http://hz.fengsongda.top/gttxseuept.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtxhbkuwvh.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtauiwsdxu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtlngywgej.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258.top/gtsuybuwpn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtnmdeagzu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gtnvkdyhbn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.quarkkingdee.top/gtphhfeaak.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ppjwa.cn/gtxoudddxr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtsfkitzta.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtujaiifos.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtofigplvw.html

Py:   os.getcwd()
来源：http://hz.ivvv.top/gtoqjnaqfo.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtcixrggll.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtvtjvczkz.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtouvkcxzh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtccltknam.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtykldjtvz.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtjqbqrhmu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ybcxt.top/gtdgihaunn.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtjwuiyoln.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtfffwxckg.html

PHP:  exit(1);
来源：http://hz.tian-w.cn/gttfoxqpnh.html

JS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtraursbxz.html

TS:   process.exit(1)
来源：http://hz.havefunace.top/gtediapsvx.html

Java: System.exit(1)
来源：http://hz.cheryme.top/gtsbfnmegh.html

Go:   os.Exit(1)
来源：http://hz.birdmap.top/gtkkkhdtfo.html

Ruby: exit 1
来源：http://hz.yvedp.cn/gtsfkaqgtp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ivvv.top/gtnhjcafyq.html

[M06] 向标准错误输出
来源：http://hz.tanke756.top/gtchxhkfjv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.haohaochexian.top/gtnyeffvnl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zycfv.cn/gtwzyzpyei.html

JS:   console.error("err")
来源：http://hz.guannengcc.top/gtruhmaldq.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtaqerlnwv.html

Java: System.err.println("err")
来源：http://hz.jinqigfzy.top/gtrnydjxhe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.vqdsnc.cn/gtexfscvpw.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtdqnnumbt.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dianchejie.cn/gtpopljeyf.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gtbstgfoox.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxuanxn.top/gtufsxrhwq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhaomingkeji.xyz/gtwflhvakx.html

JS:   require.main === module
来源：http://hz.52xcode.cn/gtsubjcjbx.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtavkqlhum.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtafmadglg.html

Go:   func main()
来源：http://hz.dianchejie.cn/gtilscowwz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxinkj.top/gtbkttvryb.html

C#:   static void Main(string[] args)
来源：http://hz.ehwqpu.com/gtevluenfp.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigufen.top/gtcjkuzluz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ehwqpu.com/gtaixntusa.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gtqdclicxr.html

JS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtzplasutm.html

TS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtylejggpg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtbluqarsq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtjsvqjkxc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xinyue.icu/gttaefaess.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenzaomai.com/gtdvkfcfid.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdfsynibn.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gteuztflyp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkzbtcaan.html

[N01] 二分查找（有序数组）
来源：http://hz.yangfankeji.com/gtqrkulfae.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yangfankeji.com/gtuzbbcvxw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gthnegcyhu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nwbrower.top/gtxbuxgkih.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtervygvcq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yongpay.top/gtxmhrhssz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yvedp.cn/gtpduetvfo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtotllkzab.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtszdtcgii.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zdqjudy.top/gtmrnshfjd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtydrhkyby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ehwqpu.com/gttscompvj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtemmyopos.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.redwolf501.top/gtwvstvurn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aizwys.cn/gturhugvsl.html

Go:   slices.Sort(arr)
来源：http://hz.jinqigufen.top/gtohtgpsau.html

Ruby: arr.sort
来源：http://hz.redwolf501.top/gtpoahgcxi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gtifybbtih.html

[N03] 快速排序（分治示例）
来源：http://hz.zhiwuduotai.top/gtadeulnkf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtevfixtyt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aizwys.cn/gtendmpfnm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtdbkhivvs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gthqweccua.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sysykeji.top/gtufewrhqu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zdqjudy.top/gtsjpdkskm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xinyue.icu/gtdelrlsuc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zdqjudy.top/gtadtmyjkh.html

[N04] 斐波那契数列
来源：http://hz.yj202588.top/gtsnxrstoa.html


<!-- 参考信息 -->