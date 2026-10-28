代发 wailian999

J. 日期与时间
来源：http://hz.zhongyouzk.top/gthnllxmdz.html

================================================================================
来源：http://hz.svipenyu.cn/gttixxritt.html

[J01] 获取当前时间
来源：http://hz.52xcode.cn/gtkcjtvgzf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydzc1.top/gtjxtdotuj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtfmfvdsdw.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtokmsztlt.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtylselzkm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.svipenyu.cn/gtuphaippt.html

Go:   time.Now()
来源：http://hz.c1oappe.top/gtzliigvno.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtnjvonidy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtihebzkbi.html

[J02] 格式化输出
来源：http://hz.xuetiantiany.cn/gtxrahoxzs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gthoooyqai.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtgjtqcctk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yonumen.top/gtompmaoei.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtqtbpqpxx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xylfe.cn/gtnorvpvgq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ppjwa.cn/gtfaszmhru.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtgihrmesw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gtscflzagw.html

[J03] 字符串解析为日期
来源：http://hz.xuanzx.com/gtlyhnwbmv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtuooshgdc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtqrkwygug.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtbtiqznqr.html

TS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtpyxpelyy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtasajmfrx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtjbpugbge.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.meibo888.top/gtxqwennpg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.haohaochexian.top/gtesulirwp.html

[J04] 时间戳与日期互转
来源：http://hz.nanxinkj.top/gtxoubwgcg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gturbytkra.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pengpengdd.cyou/gtamazaeqg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtwudgtmck.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtqepskitc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jianghu66.top/gtshstsibg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydzc1.top/gtegnjnphc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtyvlyfish.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gttsyofcdv.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtgpwdokxb.html

Py:   now + timedelta(days=7)
来源：http://hz.tanke756.top/gtejtxxybl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtpchsiomk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gttymtjkqm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtzyoublts.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtdxtjnzrd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.9152youxi.cn/gtlabpipgg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtlxdscwtf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xylfe.cn/gtzxdfmfrn.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtlkjyukme.html

Py:   (end - start).total_seconds()
来源：http://hz.ybcxt.top/gtfsekqxtx.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtcdyrtdfe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gogol.net.cn/gtlasrzyav.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtbohorkpb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shzxlz.cn/gtbkwdopxu.html

Go:   end.Sub(start).Hours()
来源：http://hz.havefunace.top/gtvccvwmrn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gtcqrfamwb.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtfirnocje.html

[J07] 比较两个日期
来源：http://hz.yj20258.top/gttjcxcpqo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gttrjbbsmy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtklkhelwh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtqybngxjb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtchtxsuen.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtznrziyiu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuetiantiany.cn/gtwzxkvhda.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtdliopwjr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtljnjjqrs.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtarazzvad.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtbrnnzjup.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtugdissqe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daria6918.cn/gtbygiezga.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtutcxyifv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtakbikzwv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tianlin.xyz/gtmluraxvp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gttbtgkrbj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yuxming.cn/gtbkuylncb.html

[J09] 时区处理
来源：http://hz.daria6918.cn/gtexkpdxdh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pycfn.com/gtdbjqvbhv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gtlalxlvlq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtjfqbyvsx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xinyue.icu/gtojxjqhjo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtkzfmgexv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gthtpwcuzx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtietpxpth.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xylfe.cn/gtqhhkouvt.html

[J10] 取今天 / 本月第一天
来源：http://hz.hywenlv.cn/gtducitgsg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yueranfly.top/gtvhzlokva.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.0kj1m.cn/gtgafxvfbl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gtfccwgkyk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gtecureoda.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtgnhapwic.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ywan-chungtsiang.top/gtpzlopalp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jiagoushi.top/gtbkpktaaf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtdczzkoev.html

================================================================================
来源：http://hz.0kj1m.cn/gtmczxfnun.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gtmopqaroc.html

================================================================================
来源：http://hz.nanxinkj.top/gthtvucshn.html

[K01] 对象转 JSON 字符串
来源：http://hz.jianghu66.top/gthvcurbqr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtyipoagco.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtvhffjdor.html

JS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtmrkfvxmh.html

TS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtbrbixcgr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gttaytymts.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gtjbvnwnbj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtgjmpxajz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtsppfdemr.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtdskphhjx.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtdmrxvuxi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xziqi.cn/gtvqhjimqm.html

JS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtibenchpg.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtakynplew.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nwbrower.top/gtjegcukhx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtlyjnlaqt.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtgdezrcvi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtansyueey.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gttgnoocss.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtnncjxdgh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtqfvpappb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtayctjvbc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtrsunovki.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtauoshvse.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yanxiufei.cn/gtrfvvrpbl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhongyouzk.top/gtnxnyqpeu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ppjwa.cn/gtpywidpfn.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtvmyfiulm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gthgphawkc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtxshphdwa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtipujggnj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtsfiuhyeb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtflvqnrqd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtqqgfijbr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xylfe.cn/gtawtvqjpv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zycfv.cn/gteidixrso.html

[K05] 深拷贝对象
来源：http://hz.xinyue.icu/gtlljnsjpm.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhixingplan.top/gtbgixkuzq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtxoraanck.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtzmjlddvu.html

TS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtplysufwz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xylfe.cn/gtmfrdcjiy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gtucemjhlr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gtjrccxpgs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtlpapsetr.html

[K06] 解析 URL 查询串
来源：http://hz.svipenyu.cn/gtmzeunkhg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gogol.net.cn/gtnwqnhuml.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangkeji.top/gtmsimkhic.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtowiojmjt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gteqjyxilv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hongshengwenyu.top/gthxozhmry.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtkuimludp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtotesykog.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jyoumei.cn/gtadhggqis.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtogzldnmw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtnyhckmqn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.c1oappe.top/gtfsrvldlg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtemfhcckr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtmvyehmpy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtpsawvfgq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gotoacloud.top/gtsqxhbgpk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtrkxbuqat.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtkpkgkwhp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cqqwz.cn/gtjfcjvsmk.html

Py:   pickle.dumps(obj)
来源：http://hz.jyoumei.cn/gtnqrnmkin.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtopxskzlh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtmgocesci.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtacxnavcv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtkuqaypbc.html

Go:   encoding/gob
来源：http://hz.zhiwuduotai.top/gtzmfewadg.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtoeuyydit.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtmkfvvosw.html

================================================================================
来源：http://hz.gaohongyu789.top/gtnlhtonie.html

L. 网络请求
来源：http://hz.quarkkingdee.top/gtraqsaxfg.html

================================================================================
来源：http://hz.sufxvd.cn/gtacrxthqt.html

[L01] 发送 GET 请求
来源：http://hz.xuanzx.com/gtowatfbnc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.kuanghao11.cn/gtyrdkydux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtlqtgebgp.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtvfpbbwbf.html

TS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtfhhsepvz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.birdmap.top/gtiwpynzkv.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gtsfbqrqdy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtsdxfznux.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gtovonubqv.html

[L02] 发送 POST JSON
来源：http://hz.shangyingyoupin.top/gtkelyleyn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gthrubllbv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtkjfyufbz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtvaedhggd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtffthlapj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hammf.cn/gtvfiwonvj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuxming.cn/gtydzicldq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtavnrdlzp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtgbltzfia.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtdtacukpb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangshuangyany.cn/gtxeeadbfu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnxiangtu.top/gttovyleue.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtkmdeqliz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtmlwjbwtu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shangyingyoupin.top/gtxvmtasra.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtxuxngmyd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtgyourebg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtharworxu.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtmnqfqosw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.birdmap.top/gtbjzdfbzq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gttcgfmnnh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtebhofdoi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtkawzeifx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.52xcode.cn/gtdaauypom.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sufxvd.cn/gtviwsyllb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daxiang520.top/gtoecgzvyq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gtayhgzvre.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtwaintdzn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shuidangran.top/gthcdakpuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtumowmgjq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtraijhnxa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtihjjvmnq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtguttxoew.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuanzx.com/gtmghhtlio.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jlsjyb.cn/gtcclvmite.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.havefunace.top/gtacsyocvx.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtwgvuzsfj.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtbmzdefes.html

PHP:  json_decode($body, true);
来源：http://hz.316326.xyz/gtuosdhdwb.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtdiodlnbt.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gtmbohkplr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gttnresnei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gttmxxlycv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhoulong.xyz/gtjwhcyyxp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gtesnmpkyj.html

[L07] 处理 HTTP 状态码
来源：http://hz.sweek.top/gtbrexmqfk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtbnvmxvjt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtgwfmfzef.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtoqbcosvt.html

TS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtaisvbisk.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gtqxsuzlni.html

Go:   resp.StatusCode
来源：http://hz.sweek.top/gtccmibrka.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtzjlwovfq.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gthuzsimbp.html

[L08] 并发请求多个地址
来源：http://hz.c1oappe.top/gtvohihmgy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ybcxt.top/gthymbzvsc.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gtdjzmjknk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtfwfnqcnq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtdmpcxerh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtmiqtpeyd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.meibo888.top/gthzgtpssb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtyklydlwl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtqcjxchcl.html

================================================================================
来源：http://hz.jyoumei.cn/gtgrbaufcn.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtoemuxpmo.html

================================================================================
来源：http://hz.wangdashe.top/gtiuzkeshr.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtjoufdcpj.html

Py:   sys.argv[1:]
来源：http://hz.zycfv.cn/gtkqronazp.html

PHP:  $argv;  $argc;
来源：http://hz.tian-w.cn/gtxthobxeh.html

JS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtemsjqfrq.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtbhcwtyzi.html

Java: args 数组（main 方法参数）
来源：http://hz.mhx1999.top/gtxalyfcrf.html

Go:   os.Args[1:]
来源：http://hz.iojbl.cn/gtnaiuvaov.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtewoockye.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cdnleiting.top/gthkdeldyy.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtvdhfuctl.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gthvgludfp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.birdmap.top/gtdrgfohox.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtemrsitgm.html

TS:   process.env.HOME
来源：http://hz.ybcxt.top/gtsbgdmexd.html

Java: System.getenv("HOME")
来源：http://hz.nanxinkj.top/gtudnjfnzv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gtaojohzkn.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtmmzrqtkm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtnloefcbf.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gtvzlfaqda.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtywpbnwyj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gaohongyu789.top/gtbmtuvoai.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtnkxseqjs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtefuafdfm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nwbrower.top/gthuasnzic.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhongyouzk.top/gtsnrbpohj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fzhhl.top/gtmgdogxet.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtaunhjypt.html

[M04] 获取当前工作目录
来源：http://hz.iojbl.cn/gtgwcnbfyn.html

Py:   os.getcwd()
来源：http://hz.jinqigufen.top/gtjgkzdxfi.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtorgmnzxb.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtuyssfsxs.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtrwuwlent.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ehwqpu.com/gtfpwarsnn.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gtjsoftibq.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gttkodsmew.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.mhx1999.top/gtiztufutm.html

[M05] 设置退出码
来源：http://hz.sweek.top/gtptjnapla.html

Py:   sys.exit(1)
来源：http://hz.hnqzz.top/gtzuwdqgow.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtlojhowit.html

JS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtkmsygxff.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gtvgnsgmmh.html

Java: System.exit(1)
来源：http://hz.zhiwuduotai.top/gtxhrdgcgf.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtdtbcxabj.html

Ruby: exit 1
来源：http://hz.c1oappe.top/gtdxyzcyfn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.birdmap.top/gtfjwltymc.html

[M06] 向标准错误输出
来源：http://hz.c1oappe.top/gtmqzdtnwe.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gteogpmpae.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtugdlncrx.html

JS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtydbgzfcn.html

TS:   console.error("err")
来源：http://hz.hammf.cn/gtwcxxegxi.html

Java: System.err.println("err")
来源：http://hz.gaohongyu789.top/gtiztenxak.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shangyingyoupin.top/gtmailvbuz.html

Ruby: warn "err"
来源：http://hz.yanxiufei.cn/gtecarxcub.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtuzjqjbds.html

[M07] 判断是否为主入口
来源：http://hz.chenjidiqi.icu/gtvpwmvdvb.html


<!-- 参考信息 -->