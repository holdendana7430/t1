代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.chenzaomai.com/gtmvoohnja.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cqqwz.cn/gtsskjcpru.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jianghu66.top/gtnojhqokr.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtdtomdmpr.html

TS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtenvgiojs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtjxmvsell.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtvuhyduuy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hnxiangtu.top/gtcnylozqh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.birdmap.top/gtogmfkpfn.html

[J04] 时间戳与日期互转
来源：http://hz.cheryme.top/gtalauwxue.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtfbqythck.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtmvqfmjen.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtlzosexsd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtemrcavsn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gtblqbkjvx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtxneskiyk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gtywtisyfj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtzcqmocdl.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangtech.top/gtvtbjxuyk.html

Py:   now + timedelta(days=7)
来源：http://hz.yongpay.top/gtcyuotrpx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sysykeji.top/gtxrjrhsfm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtasjpezyq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtvdvdqaec.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daria6918.cn/gtkqajhmhm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hammf.cn/gtcknusdxp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gtdmbtuqwl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtdnbdudgi.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtiwyftakb.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtkmzmstza.html

PHP:  $end->diff($start)->days;
来源：http://hz.0kj1m.cn/gtacungmli.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuanzhike.top/gttdcxzxrh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtqxdznnma.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cdnleiting.top/gttfqupgjk.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuxming.cn/gtknsenjkr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtsoekmemp.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtohpcphrm.html

[J07] 比较两个日期
来源：http://hz.dashuyun.cn/gtqapuzqwd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtrbljsxze.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtkthlvunu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gttrdqqvwo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gttmimvusb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangkeji.top/gtvcorsail.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtsjjtcyyn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtkmoqtnlc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtcggwyqjq.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gteilpmrba.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtzeywgnxj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gtfgnhdixz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gtgzzempsr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtrklqvguu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinghuilouyu.cn/gtkefgkzqo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guowangkeji.top/gtjovtooru.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangdashe.top/gtqrikktlx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtlicxqcyi.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gthwoeunls.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtgjpwoqbl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuanzhike.top/gtfxdsywcw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtvocwgled.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtsmyqbume.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinghuilouyu.cn/gthukcmtbe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtstqpyfzh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtdpktwlia.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhaomingkeji.xyz/gtibxsthfy.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgufenzy.top/gtohcupfxz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhoulong.xyz/gtmovgjljd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258.top/gtzxtzvwqm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tanke756.top/gtdephsxvx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.haohaochexian.top/gtipgqcjvm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtrqqgqyer.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtuluaclqr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pycfn.com/gtyqdvlmdo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydjk.org.cn/gtkfqmrnrh.html

================================================================================
来源：http://hz.chenzaomai.com/gtdevobqvv.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtjxfasvmg.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtliynovkm.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtygiqxarl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fengsongda.top/gttrqqaojb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtvryvxvfy.html

JS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtrahumliv.html

TS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtrzdmkffy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhijiandao.cn/gtmdtccezv.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtxtdhvxia.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtlmzowpjv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtcruwahqs.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtlhjulnit.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gthrelfrfc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gtryczghdv.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtktmrrgel.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtfhunieyg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtnzzsczjw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtbwywjvhg.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtvoghgvtt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cashguo.top/gtkdsellcr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtcuwzxtnh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtzhsjdoxy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtwlmmtymg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtgvckypns.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtjjpnuaxe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ppjwa.cn/gtlztothgj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtbvlddwqm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gtrryjrdjg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtynwogojp.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtucsbyqpa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtfnbxncyn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sweek.top/gtkvlxqzkb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtsgadlatp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtiqgojoxv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sweek.top/gtnsdkjwdv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtpuqbhkfd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xinyue.icu/gtidoptnsl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtngdkdxjh.html

[K05] 深拷贝对象
来源：http://hz.feifeiyinyue.top/gtunphsdkm.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gtttugxsgm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtkmocltfn.html

JS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gtttwxupis.html

TS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtugtbkryo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nwbrower.top/gtitopktkr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cheryme.top/gtzkzworft.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtjqkppslt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtbdalxdfe.html

[K06] 解析 URL 查询串
来源：http://hz.chenzaomai.com/gtfckfqtou.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.haohaochexian.top/gtvpsbqgut.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gtdtqqvcgc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtpeaoqlna.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtuumsubfj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinghuilouyu.cn/gtfvyhyvwe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtmquyzodc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtwneoylkk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhixingplan.top/gtgacigqig.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtlzqrdeka.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xinyue.icu/gtikxsbbry.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhaomingkeji.xyz/gterniaflx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gthjwmfbzc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtihumwwko.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtkmecfdcu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daxiang520.top/gtkfrsoyjk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtjxlnrtkg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtpgxwaprb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cashguo.top/gthokeqbyn.html

Py:   pickle.dumps(obj)
来源：http://hz.jiagoushi.top/gtlynjgqsi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cashguo.top/gtbhuulwrx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtomzonblc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gtezrzfagg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.havefunace.top/gtwuafmlbq.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtjrhldhux.html

Ruby: Marshal.dump(obj)
来源：http://hz.pengpengdd.cyou/gtirenwogi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtxvapzats.html

================================================================================
来源：http://hz.mhx1999.top/gtxvsejtgg.html

L. 网络请求
来源：http://hz.smart0.xyz/gteqhdjfcr.html

================================================================================
来源：http://hz.bjfxy.top/gtjgilukah.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtdrxuoefb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtmowwuuil.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtexgunqmr.html

JS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtrkuiiask.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtqesbsdeh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.havefunace.top/gtwfwkqvya.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtfuxdtica.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cqqwz.cn/gtzbhgmvez.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtujfblghq.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtnjmnvcan.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtrpbijycq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtmknwpudv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtlzlffkuy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtfpxxixwu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgfzy.top/gtacrvcvcx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangdashe.top/gtdowabazr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtlozueyxi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtazxirpyv.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtbgpfjhos.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jlsjyb.cn/gtorobohmj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yanxiufei.cn/gtmuznaqqu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtcxwxhwid.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtermkqpju.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtbmwxqqpd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtzuesrjpm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtblndcbyo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydjk.org.cn/gtzyicnekt.html

[L04] 设置超时
来源：http://hz.zhiwuduotai.top/gtfigajdbr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.meibo888.top/gtnwqjehds.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtysgjjfjc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtbqzxjwdh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gteumjsgpw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.mhx1999.top/gtlxfyrzxz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtbqolvgbd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daxiang520.top/gtsvvvollp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dashuyun.cn/gtgjsvfpwa.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtbqrpthig.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258.top/gtqyimrrdc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.9152youxi.cn/gthnswvlfx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtvdqisvcl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtpygfqxkc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangkeji.top/gtqtunoojz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hysaishi.cn/gtuwinclfg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cqqwz.cn/gtkmfltfft.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jianghu66.top/gtgkqisyhv.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtlrjdejzw.html

Py:   resp.json()
来源：http://hz.jinyuanbaomall.cn/gthmsrpqki.html

PHP:  json_decode($body, true);
来源：http://hz.xuanzx.com/gtcedyewir.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gtxdokkewo.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtfoixyxlq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tanke756.top/gtkyzaijnk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gtxukzwyny.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hywenlv.cn/gtyuihthqy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtdwnejgaf.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtatdodgkt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gthokiskub.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gtclsszpum.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gttgcwucox.html

TS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtiikysqgl.html

Java: resp.statusCode()
来源：http://hz.jqgufenzy.top/gtddmkavdv.html

Go:   resp.StatusCode
来源：http://hz.jinqigufen.top/gtwvphtted.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtjtnkbgme.html

C#:   (int)resp.StatusCode
来源：http://hz.kuanghao11.cn/gtyeikxsgn.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gtpkfajatb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtjwvqtcwg.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtyykwgsbl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtjzyayeot.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtimrvpewd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuanzhike.top/gtwzgvqlav.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.haohaochexian.top/gtxbqvtsus.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.havefunace.top/gtezrukjey.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtebxkesgo.html

================================================================================
来源：http://hz.daxiang520.top/gtarivdvev.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtzeqhzlhs.html

================================================================================
来源：http://hz.yj20258.top/gtfqmpmfsj.html

[M01] 读取命令行参数
来源：http://hz.jlsjyb.cn/gtuxsjbsub.html

Py:   sys.argv[1:]
来源：http://hz.ehwqpu.com/gtxybcnbws.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtqauieevq.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gthipkvghu.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gtamwdcgkk.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtphmohyei.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtllqbbsub.html

Ruby: ARGV
来源：http://hz.jinghuilouyu.cn/gthuczyeze.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gogol.net.cn/gtxgprqhjn.html

[M02] 读取环境变量
来源：http://hz.chenzaomai.com/gtrxebwuvl.html

Py:   os.environ.get("HOME")
来源：http://hz.fzhhl.top/gtuehwaqoh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtyyfgxbxz.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtsyycxejj.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtqvkxgctt.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtzhlfswzx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtorkfljzz.html

Ruby: ENV["HOME"]
来源：http://hz.xziqi.cn/gtebsapwrw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtvvotymft.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gttpcsbkjr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.quarkkingdee.top/gtrxevbfxb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.vqdsnc.cn/gtzspwpdib.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtwwyivdxp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtbehjxxaa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj202588.top/gtjxkvyqlv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gogol.net.cn/gtcgdanzwp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pengpengdd.cyou/gtjriyzbpj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtytduvwqw.html

[M04] 获取当前工作目录
来源：http://hz.tanke756.top/gtxupeloze.html

Py:   os.getcwd()
来源：http://hz.316326.xyz/gtdhqugdlh.html

PHP:  getcwd();
来源：http://hz.yj202588.top/gtkdehvrhp.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtajobhjmu.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtngvulgtt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtsaxlvlyh.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gtmymouliv.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtkzwcnzsl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ehwqpu.com/gtcllqxoql.html

[M05] 设置退出码
来源：http://hz.nwbrower.top/gtfuvgixda.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gtzfpxhywq.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtocfhqwag.html

JS:   process.exit(1)
来源：http://hz.nanxinkj.top/gtfnzjglhm.html

TS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtdvantplv.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtgxdbnoku.html

Go:   os.Exit(1)
来源：http://hz.sweek.top/gtbvfmkzxv.html

Ruby: exit 1
来源：http://hz.hammf.cn/gtzfmvkqhd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhoulong.xyz/gtgqwghgpc.html

[M06] 向标准错误输出
来源：http://hz.shzxlz.cn/gtuicrogpt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hywenlv.cn/gtufotziey.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhongyouzk.top/gtufoebeds.html

JS:   console.error("err")
来源：http://hz.zhaomingkeji.xyz/gtumkqjffc.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtetzrknmi.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtilmqbkul.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.bjfxy.top/gteodopaxz.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtrgpihgrz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtzxnnauwv.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtwluucbet.html

Py:   if __name__ == "__main__":
来源：http://hz.zhongyouzk.top/gtnofdcije.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtezyqrrhk.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gturvpjltx.html

TS:   require.main === module
来源：http://hz.fengsongda.top/gttkygffmi.html

Java: public static void main(String[] args)
来源：http://hz.cucudq.cn/gtweokssan.html

Go:   func main()
来源：http://hz.ybcxt.top/gtphxcqhcg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtchravuog.html

C#:   static void Main(string[] args)
来源：http://hz.gotoacloud.top/gtvqibtlow.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtuyiiinvn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gtpzjdepag.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtzfebyylt.html

JS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtgeqjocor.html

TS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtzptgzagk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.52xcode.cn/gteriptnim.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cdnleiting.top/gtctbmdymr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtxixtodsb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtirarpjsh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtbjjjwkdf.html

N. 数据结构与算法
来源：http://hz.chenjidiqi.icu/gtnjvgrdij.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtblzrpfww.html


<!-- 参考信息 -->