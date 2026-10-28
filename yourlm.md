代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtudkatcgn.html

[J04] 时间戳与日期互转
来源：http://hz.hfpthk.cn/gtwxvvsdon.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gtmrevjszj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnxiangtu.top/gttsfvwxyf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shzxlz.cn/gtredalmim.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtgubcxcdj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guowangkeji.top/gtiubwvwti.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtbxslqgql.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nwbrower.top/gtszhllkyy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtbczobqlq.html

[J05] 时间加减（加 7 天）
来源：http://hz.xinyue.icu/gttlqezyld.html

Py:   now + timedelta(days=7)
来源：http://hz.sufxvd.cn/gtrjwhxzzz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cheryme.top/gtydtnmzwv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtiwvfywxg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtvyphhhov.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtoxbfnjpw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.iojbl.cn/gtukkhbvxh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gttttaorky.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtoydjfivg.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtyvyafked.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigfzy.top/gtudeagkvw.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtomnnewnt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtjbumhslf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.smart0.xyz/gtoopnjqht.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gttpfwhfza.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtfoupgbia.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtnewcrdjq.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258.top/gtlhkdelds.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtnczjcuot.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtpzmtadiq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gtfynrxbrh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtctsrnfdp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtvbfgrwtn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtlxdutuft.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yangfankeji.com/gthibdxutu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtanylksnf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtsnmiwlhq.html

[J08] 提取年月日与星期
来源：http://hz.gotoacloud.top/gtblwygooz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sweek.top/gtuasvxpuv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghu66.top/gtqafjldkg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtafwykwwn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtcpdmzkxd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xylfe.cn/gtgalzotem.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cqqwz.cn/gtmazxjzvq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtsivdvixw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gtzwoqcrer.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtatjrdeon.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj20258.top/gtivmksplh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtqrowhkri.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtqvauuoxw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtwrqfcgfp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtkryljbci.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuanzx.com/gtioafbomg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtmruuhyaq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gttnovvswm.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtowjjcdod.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gtgkvooped.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.birdmap.top/gttferbbpw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gthzcnqxyt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hysaishi.cn/gtiujemeox.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtetebbcsu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ehwqpu.com/gtahjureuq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtzorfjhen.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtxrcaouag.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdveoqfep.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtatkrjsbs.html

================================================================================
来源：http://hz.yangfankeji.com/gtgxxfrgfb.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gtnooliuvj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtdgodipla.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtpmkzoeac.html

JS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtmhgybkmo.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtyljbyjkd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtfonwclvy.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gtavwunzeg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jianghu66.top/gtliidbjiq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtzosvpevx.html

[K02] JSON 字符串转对象
来源：http://hz.316326.xyz/gtjksmfmce.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtkxxbluvs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtvhnwzbji.html

JS:   JSON.parse(s)
来源：http://hz.sweek.top/gtynpjfgch.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtblzxalnr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhijiandao.cn/gtamwtptdt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtlmwpotlr.html

Ruby: JSON.parse(s)
来源：http://hz.daria6918.cn/gthfofjhgs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gtlyqiucvt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gttwpsohuy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtupcjaqus.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gttafeaqvw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtdrcrjemy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtgfhlqylv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gtpmjhrtfd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtcqtqthcq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gtwbbienwb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtodwbhqxi.html

[K04] 读取 JSON 文件
来源：http://hz.xuanzx.com/gtuyovellb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtihwnmvvm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ybcxt.top/gttbdwlgzs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtlsozorys.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtywtckwte.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.c1oappe.top/gtxfegrxou.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtbueubepr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtuahgceuv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gtpilnciay.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gtpikhycds.html

Py:   copy.deepcopy(obj)
来源：http://hz.sxryk.cn/gtjuhrrsgr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtipvevhmf.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtjwgvzzqh.html

TS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtxxtnduhi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cqqwz.cn/gthzntklnh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtbdffdpaw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hywenlv.cn/gtzkdiedgu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtaogfzkda.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gteaxhtfqk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtsavhhlie.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtthfzpbuc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtqoyjrsvc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gthnwwnsug.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgfzy.top/gthgwlakeb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydzc1.top/gtlfrtxtlw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gttytkfqoa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gzhubu.top/gtdvfrlkpe.html

[K07] 进制转换
来源：http://hz.0kj1m.cn/gtvuubxmjb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258.top/gtzvaurqmf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtvynpydqj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gttbiovkvb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtfhqlvfib.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtagyapilv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtcauknshg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtnitwujna.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tian-w.cn/gtnioqnoer.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shangyingyoupin.top/gtujwomwvq.html

Py:   pickle.dumps(obj)
来源：http://hz.feifeiyinyue.top/gtfveacvzh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtfdfscwcb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtatoiwfyt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtpflhrgkp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtahjxgcpe.html

Go:   encoding/gob
来源：http://hz.ydzc1.top/gtkxkbedtr.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtkcamtfsh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtmrxxwuvw.html

================================================================================
来源：http://hz.jinqigfzy.top/gtesuuyqms.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtxhlvbchw.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrzswxsrl.html

[L01] 发送 GET 请求
来源：http://hz.zycfv.cn/gtxrtpruoj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuxming.cn/gtwtuhioem.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtblpymqit.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtkzwkdgrf.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtwrlmrjof.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtcofzezla.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtwiatsdku.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gteihumydu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yanxiufei.cn/gtpjreatco.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtvnitnvag.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shzxlz.cn/gtahxhduek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinyuanbaomall.cn/gtdkkiwpni.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtehhitcfv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtaxlnmajl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.smart0.xyz/gtqtntmame.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.9152youxi.cn/gttzivfglj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ppjwa.cn/gttwcxvvcx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtzywcuuaw.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtcummiptw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangshuangyany.cn/gtedtduztr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhaomingkeji.xyz/gtkuvjkach.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtkrludvoq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtdypnnbsk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinghuilouyu.cn/gtvqwpjigs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pycfn.com/gtkmbcacpc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hongshengwenyu.top/gtcpqnlvvj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtlkbzzvvo.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtejutdphp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.meibo888.top/gthtyywpwm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yueranfly.top/gtiiceppyz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtlmbihxfw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtqbvzyfkg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gttivosevd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhaomingkeji.xyz/gtkcfbgmlb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gttmualwwd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ehwqpu.com/gtpycmtsey.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gthayaxckk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtwnjxcaqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtttstgkbh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtvpofvsvm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtgstsdqtf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zdqjudy.top/gtwabrzlhe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guannengcc.top/gtcvlwaiht.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhengqikj.top/gtoikuruki.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtqmczhciv.html

[L06] 解析响应为 JSON
来源：http://hz.nanxuanxn.top/gtjiydkqhe.html

Py:   resp.json()
来源：http://hz.jiagoushi.top/gtmmfrymip.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gtinngzxdc.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtqtdrbtbn.html

TS:   await resp.json()
来源：http://hz.nwbrower.top/gtcwwtwpbk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.feifeiyinyue.top/gtgtwqzcpg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daria6918.cn/gtzqusfwdi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtoljyfmbe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.birdmap.top/gtvcmuaios.html

[L07] 处理 HTTP 状态码
来源：http://hz.aibaodan.cn/gtrerxmddi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gthmpjrzue.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shuidangran.top/gtqsxwrugu.html

JS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtpmkabgzf.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtmngtjszj.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtugvpbpfn.html

Go:   resp.StatusCode
来源：http://hz.yuanzhike.top/gtpiiuqoip.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtwgklrksm.html

C#:   (int)resp.StatusCode
来源：http://hz.316326.xyz/gtwiwgmjbi.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtxcuyvpka.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtwkzfltoh.html

PHP:  curl_multi_init() 系列
来源：http://hz.cqqwz.cn/gtnyejxdot.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtjkzzpksg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gthjbkuzni.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtnlwcelpg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenjidiqi.icu/gteqiuihqa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtjmojgawa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtvwbswwwz.html

================================================================================
来源：http://hz.cdnleiting.top/gtyzmfqsqx.html

M. 命令行 / 进程 / 环境
来源：http://hz.xziqi.cn/gtqeatknwt.html

================================================================================
来源：http://hz.meibo888.top/gtcyrsosud.html

[M01] 读取命令行参数
来源：http://hz.jiagoushi.top/gtqekelcql.html

Py:   sys.argv[1:]
来源：http://hz.smart0.xyz/gtswrvlufz.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtwmqdbdqf.html

JS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtfaywxhzm.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtpafklixx.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258888.top/gtredgdorq.html

Go:   os.Args[1:]
来源：http://hz.cdnleiting.top/gtpyasktsz.html

Ruby: ARGV
来源：http://hz.vqdsnc.cn/gtcjneyzjs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tanke756.top/gthlvizrgs.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangtech.top/gtyozqbkwd.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtmpflvwbu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtblzxluyz.html

JS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtcnfbwqxt.html

TS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtxqnjpiab.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtfwkgxeny.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hysaishi.cn/gtsxncyrhr.html

Ruby: ENV["HOME"]
来源：http://hz.kuanghao11.cn/gtfimadqxk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtfciwyxhf.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtcugkszkc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jlsjyb.cn/gtvinzzhom.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtwlaafyeb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtljxdzwof.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gaohongyu789.top/gtyexitjxh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtwegwnkyw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtrwrrambg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydzc1.top/gttgfmmezm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cashguo.top/gtkybhmraq.html

[M04] 获取当前工作目录
来源：http://hz.xziqi.cn/gtuvugojer.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtidxkdsge.html

PHP:  getcwd();
来源：http://hz.yvedp.cn/gtnocqhyad.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtndjiwopy.html

TS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtldchsyxr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yonumen.top/gtfeilmrta.html

Go:   os.Getwd()
来源：http://hz.0kj1m.cn/gtnypfntpk.html

Ruby: Dir.pwd
来源：http://hz.xylfe.cn/gtuagqqwzv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gteurhyqum.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gtiljqafty.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtiyhfyjrh.html

PHP:  exit(1);
来源：http://hz.jqgfzy.top/gtfixhunrs.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtjpouftfv.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gtraodmuyh.html

Java: System.exit(1)
来源：http://hz.yj20258.top/gtctoxlwon.html

Go:   os.Exit(1)
来源：http://hz.ppjwa.cn/gtqbntsiwa.html

Ruby: exit 1
来源：http://hz.ivvv.top/gtukmzlusk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.aibaodan.cn/gtgjzbuvfz.html

[M06] 向标准错误输出
来源：http://hz.jinqigufen.top/gtbouqwmep.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gttbyrmbbc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cdnleiting.top/gtwuurtzfr.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtjfhezicn.html

TS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtwnznqizg.html

Java: System.err.println("err")
来源：http://hz.cqqwz.cn/gtbttpkbrl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtfwdgsqwp.html

Ruby: warn "err"
来源：http://hz.bjfxy.top/gtuazlcqab.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtbzlpytka.html

[M07] 判断是否为主入口
来源：http://hz.ybcxt.top/gtcqqnodmv.html

Py:   if __name__ == "__main__":
来源：http://hz.52xcode.cn/gtfjvoferp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ydzc1.top/gtaokbjaol.html

JS:   require.main === module
来源：http://hz.52xcode.cn/gtlsrdzukp.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtagcasrbx.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gtktgbyrqo.html

Go:   func main()
来源：http://hz.cqqwz.cn/gtaeazykfy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gogol.net.cn/gtjqlwkqtj.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtbtiztcyy.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxinkj.top/gtqovmdzje.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gtdwzmmrmu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jyoumei.cn/gtjxoafbvu.html

JS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gtsneeifyt.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtsoltaqsu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtuqeevbrg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtharmybza.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhiwuduotai.top/gtsmpzqljo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtozjuzdax.html

================================================================================
来源：http://hz.hnqzz.top/gtyoxdgavg.html

N. 数据结构与算法
来源：http://hz.yvedp.cn/gtmthqdmdb.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtwaekmnsd.html

[N01] 二分查找（有序数组）
来源：http://hz.yuxming.cn/gtmpqeiauo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258888.top/gtfrfldzzd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.andypj.xyz/gtwfoquyqc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtrqddfjig.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtjjftwssc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtfnbmrtov.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtdgtwsszv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258888.top/gtbmjvtkxx.html


<!-- 参考信息 -->