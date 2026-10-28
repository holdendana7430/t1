代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtswvzccaq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtkwzzjhcl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtvnwpzmwt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gtbohwlxln.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtxxyrkohu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtjzdcqlvq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shuidangran.top/gtgrdldxbw.html

[J06] 计算两时间之差
来源：http://hz.316326.xyz/gtvioykqho.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgufenzy.top/gtcwbrqcul.html

PHP:  $end->diff($start)->days;
来源：http://hz.hfpthk.cn/gthgrkmfcz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtpnphexhj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtyhwvmbbt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangtech.top/gtzxwjievk.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtutmtvzna.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gthzpkxdsw.html

C#:   (end - start).TotalSeconds
来源：http://hz.birdmap.top/gtybzpujen.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gtwwwjycvi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtqpcivwyh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sufxvd.cn/gtkkumwgcx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtxsgsyynt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtejewovsk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gttanhxbwi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenzaomai.com/gtsgmxtaqr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtishljisg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtilpdutmi.html

[J08] 提取年月日与星期
来源：http://hz.gzhubu.top/gtdvosbngo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xingfuxueyuan.xyz/gtnppbjqvl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.smart0.xyz/gtdgpndijh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gttnvzansp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtgiihqurm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xziqi.cn/gthckghqqu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtrxqbaylt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gtehqtqavy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydzc1.top/gtmuicbhhp.html

[J09] 时区处理
来源：http://hz.aizwys.cn/gtocwzjzzw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gaohongyu789.top/gtibrtfqbl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtuddayqot.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtdvraccne.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtulebguwg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtwtglckvy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gtipuflkbf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhiwuduotai.top/gtuqzwancx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hongshengwenyu.top/gthjjzdayi.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtbfktgslf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gtfzdooimt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gtdavtratx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.quarkkingdee.top/gtevqzzvea.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtxtlqwjsk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuanzx.com/gtbcenfvcs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtaxadxlqs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.havefunace.top/gthewuuaeq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jlsjyb.cn/gtqsacrrft.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgvncalzq.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gtqtlxwqql.html

================================================================================
来源：http://hz.9152youxi.cn/gtkkyegayl.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtgnistcuz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtefmacyto.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtqqqailvh.html

JS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtnddzzjme.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtcodjehjx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gtegxkbgsh.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtutsckcoy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ehwqpu.com/gtecnamsfh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ywan-chungtsiang.top/gtpnoqized.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtcpbydflw.html

Py:   json.loads(s)
来源：http://hz.andypj.xyz/gturcpiezk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenzaomai.com/gttivflhpq.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtrgzygmqv.html

TS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtyqjraula.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtpufjesue.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtspmylqpe.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gtkkmxvfqa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtddlwpjwr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhaomingkeji.xyz/gtgfbzuvvr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtjrazujfx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtcpsyriuh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtdiktqugd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtjzucoqtu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtaawmihgp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtjukpopiv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xziqi.cn/gtkamlzqyy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shangyingyoupin.top/gtjdrqdxhp.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtzqrhybzb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gtoxozrweq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.andypj.xyz/gttjqdtbwo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtacutfzhy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtfhzpwfuy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtbotfwwaq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtwagjbxie.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtoumpeqmd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtitddanmq.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtxdldrkty.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gthltfzfhb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtuvvyiitg.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtfgexwcct.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtrakkxwxx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinyuanbaomall.cn/gtmjaflcwd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtxdqodbln.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtwqojyuqd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.andypj.xyz/gtzkpmgumb.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gtrikqyutn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtpvyjrdqh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtsizkjnsf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtuphvjcdk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtzjzuuzco.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xinyue.icu/gtnnmtgipy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenzaomai.com/gtvyuwrphm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtctppnddr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yvedp.cn/gthmutpfva.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtvanomqpr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.meibo888.top/gtxgbahnef.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtostfqkce.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtdlieavkt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtmyswmvky.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtqltyvczp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jianghu66.top/gthgdbxnrf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.iojbl.cn/gtmalddclw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sweek.top/gtelcdstxi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtkbeersnb.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtjdltmned.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gthuoyigcs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtrkytqxhz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtfhdbivxl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pengpengdd.cyou/gtcwcukmhv.html

Go:   encoding/gob
来源：http://hz.jyoumei.cn/gthvxbnafk.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtdqlrswcm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zdqjudy.top/gtzxohpmlw.html

================================================================================
来源：http://hz.daxiang520.top/gtxoieqbzd.html

L. 网络请求
来源：http://hz.hysaishi.cn/gtvkqepmnf.html

================================================================================
来源：http://hz.zhoulong.xyz/gttgxxmsaa.html

[L01] 发送 GET 请求
来源：http://hz.jinqigfzy.top/gtbycehtek.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhoulong.xyz/gtnpexckrd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sweek.top/gtmpbvdfnq.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gttvacmknm.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtcacamuaq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gtvrdnhpqd.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhijiandao.cn/gtedxpyssy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gttelzfsik.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtbxqzmeot.html

[L02] 发送 POST JSON
来源：http://hz.dashuyun.cn/gtrzcxtmyq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtrntxvamj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cucudq.cn/gtzkssnvod.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtiltqbwdy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtyfxraqlx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.mhx1999.top/gtvzyywqgo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnqzz.top/gtglzarqzc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtlmceflhy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtmmsnjyhg.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtgsjadjvk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gtfucbrfbp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtretjnnug.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtayqtjktt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtrqzmyrtu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yangfankeji.com/gttgshgzdj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtgycvkueu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtmyuovxvj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtzixjfubb.html

[L04] 设置超时
来源：http://hz.mhx1999.top/gtjjymrmae.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtkvvyhkrc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cqqwz.cn/gtowbsrjzh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtxkwovmpo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtjbamjuxq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gtskaerqpo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtarazfkky.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pycfn.com/gtimnzkuxf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtajtbxzcu.html

[L05] 上传文件（multipart）
来源：http://hz.ivvv.top/gtjsiydntj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gtrgbqkhxa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dashuyun.cn/gtgzvcgilc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtyjzvhjba.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtdzxgrcvf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhiwuduotai.top/gtjllzmydg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gtlxoibtoe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangkeji.top/gtmeylkzlf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtfvhnpuhl.html

[L06] 解析响应为 JSON
来源：http://hz.jlsjyb.cn/gtmsnblkcd.html

Py:   resp.json()
来源：http://hz.gzhubu.top/gttrxwqlya.html

PHP:  json_decode($body, true);
来源：http://hz.jyoumei.cn/gtqgpgeajl.html

JS:   await resp.json()
来源：http://hz.zhengqikj.top/gtheuheruy.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtopzoxbjz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuanzx.com/gtdekywwmr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtkvkckxkw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuanzhike.top/gtoakpjneq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sxryk.cn/gtitlwnkee.html

[L07] 处理 HTTP 状态码
来源：http://hz.haohaochexian.top/gtpltonnzv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gtqefbelsl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtodnbngwd.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtfvpwjvry.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtghfhzxnc.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtnbxeykna.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtfoodpsid.html

Ruby: resp.code.to_i
来源：http://hz.meibo888.top/gtcsthmhzg.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtaqyfgvib.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtuwcgizrp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtylcjcayt.html

PHP:  curl_multi_init() 系列
来源：http://hz.ivvv.top/gtfbcuobga.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtxluwbhsr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtkezsbjpn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhengqikj.top/gtukprjuth.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinghuilouyu.cn/gtljrlwowf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenzaomai.com/gtkrkgoszb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sweek.top/gthovlkvuz.html

================================================================================
来源：http://hz.yonumen.top/gtveuagbsk.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gtdgvxzobf.html

================================================================================
来源：http://hz.yueranfly.top/gtnajyzzuk.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtgytczapv.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gtxsqbirng.html

PHP:  $argv;  $argc;
来源：http://hz.cdnleiting.top/gtosyaotwa.html

JS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtbbhocjzc.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtcqsqctgi.html

Java: args 数组（main 方法参数）
来源：http://hz.nwbrower.top/gtgoedqwwe.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtndyxgvwi.html

Ruby: ARGV
来源：http://hz.0kj1m.cn/gtosqnfvwv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guannengcc.top/gtbupglbyl.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtpbrlucvc.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtvxfwbydw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtmgigxxbc.html

JS:   process.env.HOME
来源：http://hz.xinyue.icu/gtchphskzl.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtrmjlhokk.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtvpnzwdqa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtoisvhcut.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtcxyigehs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guowangkeji.top/gtpoybjoyd.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtotngirks.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtjcszshwg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtifvrpzmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtidqdnmpl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtciibzyfb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnqzz.top/gtxkjmrwda.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gzhubu.top/gtjadvhicj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtckrkzxra.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhongyouzk.top/gtydeknbfq.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtjhqezcca.html

Py:   os.getcwd()
来源：http://hz.yueranfly.top/gtqftbjjiy.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gtnblsbujt.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtydanrdky.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gthltwxoax.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtbbsoldcl.html

Go:   os.Getwd()
来源：http://hz.tianlin.xyz/gtotwqrlgo.html

Ruby: Dir.pwd
来源：http://hz.fengsongda.top/gtpnaiutpz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtzmnzgmrs.html

[M05] 设置退出码
来源：http://hz.daria6918.cn/gtbmndlfpy.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gtrkbzznix.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtfqlcrhyl.html

JS:   process.exit(1)
来源：http://hz.redwolf501.top/gtvuxpemgu.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtvakjwrnd.html

Java: System.exit(1)
来源：http://hz.havefunace.top/gtgxknkknc.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtddjcugpz.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtgodewcur.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuanzhike.top/gtlujylhem.html

[M06] 向标准错误输出
来源：http://hz.yanxiufei.cn/gtmdtqtaux.html

Py:   print("err", file=sys.stderr)
来源：http://hz.pengpengdd.cyou/gtbieuezjc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtjimyjddt.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gtjujyxkcg.html

TS:   console.error("err")
来源：http://hz.hnqzz.top/gtxvaoqakl.html

Java: System.err.println("err")
来源：http://hz.zycfv.cn/gtqyspotxr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cqqwz.cn/gtlmidptdc.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtgbebypfa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gtmrbycvjt.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gthpiyhknh.html

Py:   if __name__ == "__main__":
来源：http://hz.zycfv.cn/gtceqiiuxg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtfuiaqsaa.html

JS:   require.main === module
来源：http://hz.hammf.cn/gthmjiiahz.html

TS:   require.main === module
来源：http://hz.yuxming.cn/gtjohjbzsk.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtfticmuxc.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtgipsvyib.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.mhx1999.top/gtpjumfayj.html

C#:   static void Main(string[] args)
来源：http://hz.jianghu66.top/gtocynaixs.html

[M08] 获取系统与运行时信息
来源：http://hz.xziqi.cn/gtlbdwludr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtltfbcaqj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pengpengdd.cyou/gteqerhdad.html

JS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gthvexkfnd.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtxumstelt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pycfn.com/gtokdsrodu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhaomingkeji.xyz/gtrrvmgynh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydjk.org.cn/gtyfbnvbgv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hammf.cn/gtikhedjmp.html

================================================================================
来源：http://hz.quarkkingdee.top/gtzlyhsipf.html

N. 数据结构与算法
来源：http://hz.xuanzx.com/gtajzdmwgp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzaztfayo.html

[N01] 二分查找（有序数组）
来源：http://hz.daria6918.cn/gtrdedwczm.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fengsongda.top/gtjigoynbg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhixingplan.top/gtinhzrrhh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtwuuybrms.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtlemptoze.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtscerynhf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.smart0.xyz/gtspipcjby.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtbrvywacs.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gzhubu.top/gttukovcup.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.mhx1999.top/gtdgusenxl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtcusbjelq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhiwuduotai.top/gtlvtchkhn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtcpdvfnmu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtgwcjoftm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.cqqwz.cn/gtpnmcwwlt.html

Go:   slices.Sort(arr)
来源：http://hz.feifeiyinyue.top/gtabuxfekh.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtqpkzlbte.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jlsjyb.cn/gtxmpjsofe.html

[N03] 快速排序（分治示例）
来源：http://hz.xylfe.cn/gtlbwyosyd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtljbaurfl.html


<!-- 参考信息 -->