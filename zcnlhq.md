代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtuzelauam.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daxiang520.top/gtxbequghd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtmdentziu.html

================================================================================
来源：http://hz.52xcode.cn/gtobiyqwlh.html

J. 日期与时间
来源：http://hz.sufxvd.cn/gttbrjlkgt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtjzjuatzp.html

[J01] 获取当前时间
来源：http://hz.snrcjt.cn/gtwuwiiovb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tanke756.top/gtbnozfqph.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtjknbmgsd.html

JS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtufomcisd.html

TS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtxbvwuemn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gthwzbilgr.html

Go:   time.Now()
来源：http://hz.ydjk.org.cn/gtoacsgbpl.html

Ruby: Time.now
来源：http://hz.jianghu66.top/gtmcnneqyf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtltneafcc.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtroheqnwq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtsvgcqnez.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtpmvwqdmz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtvyaeupqj.html

TS:   d.toISOString()
来源：http://hz.quarkkingdee.top/gtiencgwga.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zycfv.cn/gtigqrkpaw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtszudsqxf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtseiltkqe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cqqwz.cn/gtpnvlaxtn.html

[J03] 字符串解析为日期
来源：http://hz.gogol.net.cn/gtygcohehw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtltuhzsff.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.316326.xyz/gtejabcwmc.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtrkcncjsj.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtrofqicql.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtfgtazbez.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtthilgwnc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtixeqgxnq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hongshengwenyu.top/gtqsqlhkfv.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtygbypuug.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aibaodan.cn/gtzfkyexpl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxuanxn.top/gtletcuuxm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.havefunace.top/gtcgrvoevy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guannengcc.top/gtsymievzq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtwazlfixu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xziqi.cn/gtllwtlejp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fengsongda.top/gtcfdxttbu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gteblwoxgi.html

[J05] 时间加减（加 7 天）
来源：http://hz.hysaishi.cn/gtncxkgvdn.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtzpfsykzr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.quarkkingdee.top/gtaweorjbi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtxdoppucr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtfyjabvhh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jyoumei.cn/gtmppxbxhc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jlsjyb.cn/gteagjwvwh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cheryme.top/gtvtkclinu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuxming.cn/gtjlrphfgm.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtnpujexro.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtcpguqwfe.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhoulong.xyz/gtfaguxdhw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gtpkyxwiof.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtgyfaxlpe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtkmlqvamt.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gttyysaajl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gthjxhwfzr.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtecnmfzhy.html

[J07] 比较两个日期
来源：http://hz.yanxiufei.cn/gtnwrlouxx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtwdjnjcgg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhijiandao.cn/gtugkgtxub.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtauhhqxjo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gtmamnbhgn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.snrcjt.cn/gtjftyadlp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtfzrcplzz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtjntrlfkn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtfvfiqvrq.html

[J08] 提取年月日与星期
来源：http://hz.yuanzhike.top/gtthqokmda.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pengpengdd.cyou/gtckhefhol.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghu66.top/gtluatkpbk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtwumbbuqb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnxiangtu.top/gtscjgxzsr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigfzy.top/gtwxexosei.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtrrzbaeng.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtmrpmjcvk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.haohaochexian.top/gtlotmjnbj.html

[J09] 时区处理
来源：http://hz.jyoumei.cn/gtrmelndoe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gthrhxswtp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtwtckdydf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtyrchdizw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtlsflyapb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtmsuyymhk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.snrcjt.cn/gtzybnxuag.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtaorskcmj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aibaodan.cn/gtjubmditl.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtxwqswtoe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuxming.cn/gttvkmivuy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.0kj1m.cn/gtcvmbwkte.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtuzjjymgt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.redwolf501.top/gtcmajnjkr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gttnzobpnd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.feifeiyinyue.top/gtyiabtiuo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangtech.top/gtqwvqfgvw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gtzvodsdtq.html

================================================================================
来源：http://hz.hammf.cn/gtfyybpche.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gtpevilaho.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzsbxswoo.html

[K01] 对象转 JSON 字符串
来源：http://hz.xylfe.cn/gtyzfuidxo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtlwwrgktz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtguihrjap.html

JS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtxzwzbilq.html

TS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtblbnvqyh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ehwqpu.com/gtrclekjee.html

Go:   json.Marshal(obj)
来源：http://hz.pycfn.com/gtpylvyzqw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtforyqspg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtvrtxvtkg.html

[K02] JSON 字符串转对象
来源：http://hz.cqqwz.cn/gtakyywdwr.html

Py:   json.loads(s)
来源：http://hz.zhiwuduotai.top/gtfuachoya.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xingfuxueyuan.xyz/gtvzmgdlvu.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtspjizlsl.html

TS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtokjcbwqq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.redwolf501.top/gtusszhfmz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtsejsvxex.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtdjpzszku.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtbhzjgnwg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtjulsbixh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtblgdduhj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtowpbcmxh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtenkfypni.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtxhbzakwm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dianchejie.cn/gtvhypcota.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtzfrftzor.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gtnzcfhaym.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtymbcsigf.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtqijdlkur.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.quarkkingdee.top/gtivywwmpy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtwqnnrtol.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gttxwwjqtm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtlqzrhume.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgfzy.top/gtzywtgmxh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtrhzqcczq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gtaqwiysqt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.9152youxi.cn/gtgugevmwj.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gtbjhevjwk.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtfxiiwhbb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yangfankeji.com/gtludckhih.html

JS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtfqyiujer.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtvjgqhxrx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.c1oappe.top/gtyifmjccy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gtfnlxjedw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtknshorys.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtfocicsqb.html

[K06] 解析 URL 查询串
来源：http://hz.ydjk.org.cn/gttxktipmb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtwjlenzud.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.bjfxy.top/gtxbjqtorz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtbqseccau.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtzbkbkoyk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinghuilouyu.cn/gtxxcckubb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cqqwz.cn/gtqzofidwr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gtcxmgyxdt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.9152youxi.cn/gtlgdqarnd.html

[K07] 进制转换
来源：http://hz.jinqigufen.top/gtxvmvmnat.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tian-w.cn/gtnbnoidtz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtxkuqmelr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtqegjiniv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtgjqmofgv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtjktvhmai.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.52xcode.cn/gtwnteqhuh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aibaodan.cn/gttvppmkhk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.snrcjt.cn/gtsaovclfa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtzcqrydmx.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtfvsuxgai.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtfuiuztpq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtjyxlukje.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtklkrwexw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtkdihdwqh.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gtcsqhouwt.html

Ruby: Marshal.dump(obj)
来源：http://hz.dianchejie.cn/gtugyreiou.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.smart0.xyz/gtnunfamcb.html

================================================================================
来源：http://hz.tian-w.cn/gtfaerrqko.html

L. 网络请求
来源：http://hz.shuidangran.top/gtqqcqcshv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqhhtdjlm.html

[L01] 发送 GET 请求
来源：http://hz.chenlongwang.top/gtyiikupfq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtspzyuchk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gteaoalvzs.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtezzkiecj.html

TS:   await fetch(url)
来源：http://hz.yangfankeji.com/gtavkyzdxa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtkvqphmxo.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gtauvsjzsu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtkuvcvyqq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gtqycwsdku.html

[L02] 发送 POST JSON
来源：http://hz.jqgufenzy.top/gtaodddppv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sysykeji.top/gtfnpitiqu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daria6918.cn/gtmabznxol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtibwrjpdv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtbhsmaasc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtrzmjjvvt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinyuanbaomall.cn/gtjsyahwqp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jlsjyb.cn/gtterjiwff.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtywvcaygy.html

[L03] 设置自定义请求头
来源：http://hz.ydzc1.top/gtvutwrqmo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tanke756.top/gtjxvnwokx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnqzz.top/gtoaqcvmnl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtvxwrzuat.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.iojbl.cn/gtnalkkgew.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.316326.xyz/gtxecyfxgx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtkrozhoel.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtervvpvet.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtioshovzm.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtnmbusmlw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jlsjyb.cn/gtbiruucab.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hongshengwenyu.top/gtnqtsymuo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtinkkvznf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtztitlweg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shanyushiyangkeji.top/gtneulylkp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gtzfvaakfb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.svipenyu.cn/gtlbdgtric.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xingfuxueyuan.xyz/gtqgqkzkcn.html

[L05] 上传文件（multipart）
来源：http://hz.jinqigufen.top/gtmhwwxntr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhengqikj.top/gtqskpgdcp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtviqsiubl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtjcpmclme.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtsgjvfttn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.vqdsnc.cn/gtbvfcfdcq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtugqqbdax.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gthjzkdoev.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtufzqltev.html

[L06] 解析响应为 JSON
来源：http://hz.sweek.top/gtblvpfowj.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gtileqandx.html

PHP:  json_decode($body, true);
来源：http://hz.gzhubu.top/gtulgazzyi.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtxgnazowg.html

TS:   await resp.json()
来源：http://hz.52xcode.cn/gtbpvwulch.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtivyprrqu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhixingplan.top/gtxnzzbzls.html

Ruby: JSON.parse(resp.body)
来源：http://hz.316326.xyz/gtsbyfmaoe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xinyue.icu/gtepjlxwzd.html

[L07] 处理 HTTP 状态码
来源：http://hz.ppjwa.cn/gtdhizsiha.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtctglonpa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuetiantiany.cn/gtetvpxgry.html

JS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtgrmpkbbe.html

TS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtxaskcizy.html

Java: resp.statusCode()
来源：http://hz.birdmap.top/gtvcnslyuh.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtuytqifrc.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtmlapxpdb.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtnukmcden.html

[L08] 并发请求多个地址
来源：http://hz.yongpay.top/gtsuccuyhz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtdtiucnoc.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gthufrqqjf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtehoiyaqd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gthavsrxzr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cqqwz.cn/gtktkyrljv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtcllfoukp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuanzhike.top/gtwtnimmtz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtdmxupqla.html

================================================================================
来源：http://hz.nwbrower.top/gtzlmmuhts.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtvowyxhom.html

================================================================================
来源：http://hz.xuanzx.com/gtkrluewyx.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtvtkcpois.html

Py:   sys.argv[1:]
来源：http://hz.meibo888.top/gtlrprlsha.html

PHP:  $argv;  $argc;
来源：http://hz.xinyue.icu/gtriizvuzd.html

JS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gthteignsn.html

TS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtnltllyyg.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtxzbxjrow.html

Go:   os.Args[1:]
来源：http://hz.xuetiantiany.cn/gtgpeipwbl.html

Ruby: ARGV
来源：http://hz.hongshengwenyu.top/gtdtyuadwv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtzkbhaylx.html

[M02] 读取环境变量
来源：http://hz.nanxuanxn.top/gtwcheashi.html

Py:   os.environ.get("HOME")
来源：http://hz.feifeiyinyue.top/gtsbpvpqrv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtgnxcgtbh.html

JS:   process.env.HOME
来源：http://hz.jinghuilouyu.cn/gtlwkdfios.html

TS:   process.env.HOME
来源：http://hz.zhaomingkeji.xyz/gtdlahqonq.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtwecequfe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gtbxsxulyv.html

Ruby: ENV["HOME"]
来源：http://hz.yanxiufei.cn/gtmbugweyh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yueranfly.top/gtodnaluuz.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtkamukwrc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuanzx.com/gtmjjrjglj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuxming.cn/gtjhuynnqw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtpuvdnzcn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtulmqmfct.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtoxnjotis.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgfzy.top/gtetcatnqe.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtpupkmspg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhixingplan.top/gtainsqsoq.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtqfduweki.html

Py:   os.getcwd()
来源：http://hz.ydzc1.top/gtxlpjkhdr.html

PHP:  getcwd();
来源：http://hz.xinyue.icu/gteneecadi.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gtcchkhert.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtufrsnaii.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gtyepsuaqb.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gtbfoevrlc.html

Ruby: Dir.pwd
来源：http://hz.daria6918.cn/gtwsssjqfo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtrprrtioy.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtnrhfikrv.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtrkkybcop.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtfajuojta.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtwtkwebtn.html

TS:   process.exit(1)
来源：http://hz.yj20258888.top/gtjuqfbkpb.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtsbwigsfv.html

Go:   os.Exit(1)
来源：http://hz.wangshuangyany.cn/gtutbibhaz.html

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtrzuidemy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtqtlpbfsh.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtpwathehc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zdqjudy.top/gtxqkvfmht.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhengqikj.top/gteclcuzza.html

JS:   console.error("err")
来源：http://hz.cheryme.top/gtlcdlbugs.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtajxlsaan.html

Java: System.err.println("err")
来源：http://hz.zhongyouzk.top/gtsqbuxtyj.html


<!-- 参考信息 -->