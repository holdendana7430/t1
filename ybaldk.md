代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gtnexojdcm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtnbvebvof.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtbuihhize.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gteyhjhcwt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtytypuhzx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtqiimhmzs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.andypj.xyz/gthiraagzf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtfekowogn.html

J. 日期与时间
来源：http://hz.jinghuilouyu.cn/gtzvhueuyd.html

================================================================================
来源：http://hz.ybcxt.top/gttalcobbp.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtixnehryu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtmyvikknr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtlnksuswv.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtisahaclm.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtsuuinxgu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gtcexdjjqd.html

Go:   time.Now()
来源：http://hz.yj20258888.top/gteowvoiee.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtisrclxow.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtgksfyztz.html

[J02] 格式化输出
来源：http://hz.cashguo.top/gtdgppsuyv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtyvdkqvzq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtpfehqkuq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guannengcc.top/gtlrtqnqbq.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtgvrrtwex.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gthgmuleyh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gtjzimpfmj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtgscemcjj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gthhgnazvh.html

[J03] 字符串解析为日期
来源：http://hz.zhaomingkeji.xyz/gtjntnbbns.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuxming.cn/gtkjeoscwa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtdxypylwz.html

JS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtkknxfvaz.html

TS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtrkpjdajz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gttkwtcszz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtyfowhhdm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pycfn.com/gtbtxtqmic.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtzxxmupuq.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtzllcxmwl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtwkiecojg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gtxsxjzxyf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtwqifszem.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daxiang520.top/gtdbmkkbuh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtdogcaxwe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pengpengdd.cyou/gtxjsbismn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fengsongda.top/gtnjdyawzz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtcrpcjpuq.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtghxbdanl.html

Py:   now + timedelta(days=7)
来源：http://hz.guannengcc.top/gtpvjrbean.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hammf.cn/gtgzzulbdz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtecuowpxk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtskehgxyg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtfuaihhge.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtpjmsccxc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hongshengwenyu.top/gtfzwuamzm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dianchejie.cn/gtxeroiiea.html

[J06] 计算两时间之差
来源：http://hz.yvedp.cn/gtuxpgbtve.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtajlhomae.html

PHP:  $end->diff($start)->days;
来源：http://hz.iojbl.cn/gtpryjpabo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhongyouzk.top/gtzxyddact.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gtdspwelxg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtbajmyntr.html

Go:   end.Sub(start).Hours()
来源：http://hz.iojbl.cn/gtvajrvjuy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258888.top/gtsqcecjrh.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtftnrxlny.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtekzlghdw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtsqfcwznz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gtyuhaxqrf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtbeqjodia.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtocqwtqlp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhaomingkeji.xyz/gthxhisajx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtjjkqtaul.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtwlhibjpk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gthetirijh.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtmixhsuqm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cdnleiting.top/gtmlhymhiw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yonumen.top/gtzyebzvsm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ivvv.top/gtdrmuyjgb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenlongwang.top/gtmdnazcxk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtmyhfcedf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fzhhl.top/gtgsycbyma.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtqwmyxxpz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtocqrzxtc.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtmungecqf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.vqdsnc.cn/gtptxdzxrc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtrhmwizri.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtlcipywxw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtyzkenapz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dashuyun.cn/gtgaqwtohj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gtdhskykjm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtpydehpvy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnxiangtu.top/gtsxnckokt.html

[J10] 取今天 / 本月第一天
来源：http://hz.jiagoushi.top/gtkicokklj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtrwgfogxc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtdqodscmy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtaixqyvkm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gteyjbfrjk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtukzvgacs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtuzzcpgym.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yanxiufei.cn/gtumqxtsqr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtxhtzpmyc.html

================================================================================
来源：http://hz.hnqzz.top/gtcpywuybr.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtbckwbdcu.html

================================================================================
来源：http://hz.jinqigufen.top/gtbvxfextp.html

[K01] 对象转 JSON 字符串
来源：http://hz.daria6918.cn/gtgubgvdng.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtoxnpxjxn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gthokhaben.html

JS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtsegfxdyk.html

TS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gttjbvvytt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtqjktapnd.html

Go:   json.Marshal(obj)
来源：http://hz.zhiwuduotai.top/gtnanazabz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hfpthk.cn/gtktmodmck.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtzoolokns.html

[K02] JSON 字符串转对象
来源：http://hz.vqdsnc.cn/gtoioyqzpk.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtxvneszzl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtdznobeun.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gttvkqkmsv.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtdejclkww.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtlunddmim.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gttdnbwhug.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtobjgkpzq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zycfv.cn/gtsyydqrou.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.havefunace.top/gtihrcoyni.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yongpay.top/gtazsckxrr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtyxhqnuvw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtrquibxjt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtlnlzbygs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtxragntqw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtkcukhmid.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtmqonvkww.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtcbktxtko.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtktfzvlan.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gthvybvjny.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtlenhlqkg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtcoqwqrvb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gteqyyewsc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtetfutuxu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtfdhaognl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtostxaauw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtxmvhphsa.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtqamqznnx.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtmngazstn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuxming.cn/gtuqucxudl.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtowswtctd.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtkxyaqlky.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtavhsvtxy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtrlntedtw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cdnleiting.top/gtpfxtkjoq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ybcxt.top/gtdoqqhjkh.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtvoqyywmb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhixingplan.top/gtuwtovsqw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtmobpwrbe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtwqttlquz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtsywtshfh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydzc1.top/gtkkzcvmnz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xziqi.cn/gtjmodurse.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtfvwkarte.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgfzy.top/gtxhpfsijx.html

[K07] 进制转换
来源：http://hz.jlsjyb.cn/gtbmqdilnz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.316326.xyz/gtzpdmzsri.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.meibo888.top/gtuyylqbfo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtcnkcghxc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtymecwotk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gthhndkaxr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gtoweqebep.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtsehwfsgc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtjkcmepfa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtnllnqevi.html

Py:   pickle.dumps(obj)
来源：http://hz.kuanghao11.cn/gtqbebnzco.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtgmmafauo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtdbegappz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtbrytisjs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtdpgvepjs.html

Go:   encoding/gob
来源：http://hz.ppjwa.cn/gtzofzscwz.html

Ruby: Marshal.dump(obj)
来源：http://hz.mhx1999.top/gtedxkqyvo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.0kj1m.cn/gtnlrarnnn.html

================================================================================
来源：http://hz.jqgfzy.top/gtdsmdhusy.html

L. 网络请求
来源：http://hz.ppjwa.cn/gthwgmvkuq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtjhcschqb.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtdotfsqvr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gtoysooqzm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtzkaoxubi.html

JS:   await fetch(url)
来源：http://hz.316326.xyz/gtcabowtql.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtnkveoggv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtwhcfsrqi.html

Go:   resp, err := http.Get(url)
来源：http://hz.9152youxi.cn/gtfskydnch.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtfplvyklq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtmsjhnyem.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtqoffvcwa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtzkehdyph.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.quarkkingdee.top/gtsvavnvwg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gthjtxidgc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gttdcxdgdq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gtndaqktjv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aizwys.cn/gtvneyxruh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ybcxt.top/gtvfqdwuwa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtcmlstwnn.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gtckdofgfb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gthjsuvvaz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gtckrwtqnu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtivsxpqyn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtcgfrmbfq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yangfankeji.com/gtkeaaqygw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtgbmpjyji.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jlsjyb.cn/gtohlnimmq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtpbwofnrv.html

[L04] 设置超时
来源：http://hz.zhixingplan.top/gtwiblhxyy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangdashe.top/gtjfkbvxwd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtrheywcwk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtzbnajvkg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtftbxkobz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuanzx.com/gtxxyseles.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yanxiufei.cn/gtrzzzpjxg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gteabbsbal.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtbcjvavok.html

[L05] 上传文件（multipart）
来源：http://hz.0kj1m.cn/gtvplirfyd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtpxyxliur.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtuibnzsxw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtcmnbbqfm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtfcprhydz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtmvkinlaq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ivvv.top/gtuwbvnagq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tanke756.top/gthphgfziy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtvdjayyim.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gtzuvbnupx.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtlopdtjjc.html

PHP:  json_decode($body, true);
来源：http://hz.hammf.cn/gtbsrltrbc.html

JS:   await resp.json()
来源：http://hz.tanke756.top/gtvxechbbi.html

TS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtlwnsfwcj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gthptizmsd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxinkj.top/gtvnwqavyy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtapasdyeb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtyshpqvuk.html

[L07] 处理 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtqnujoltw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigufen.top/gtibvoblpc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtkgybqyqp.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtiqoiboov.html

TS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtlwvafpls.html

Java: resp.statusCode()
来源：http://hz.andypj.xyz/gtznfjadwx.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtdbearigd.html

Ruby: resp.code.to_i
来源：http://hz.iojbl.cn/gtgrgjtjyr.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigufen.top/gtjxzphbui.html

[L08] 并发请求多个地址
来源：http://hz.yongpay.top/gtsfkogbxo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtkbacqzfb.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuetiantiany.cn/gtretzsoou.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtpatmlgvj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtrxceozjt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fengsongda.top/gtvwcwkpex.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nwbrower.top/gtdpdfmnmn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtitayrbry.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jyoumei.cn/gtgeyxivsm.html

================================================================================
来源：http://hz.yongpay.top/gtohplbcuj.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258.top/gtrsedoznq.html

================================================================================
来源：http://hz.9152youxi.cn/gtlxrkerwo.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtgtrmafjv.html

Py:   sys.argv[1:]
来源：http://hz.ybcxt.top/gttacitphf.html

PHP:  $argv;  $argc;
来源：http://hz.mhx1999.top/gtutzgeoqg.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtavkaqpmf.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtkrjtxzoc.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtdlsaydwa.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtfcgehtnf.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtwtwefpyg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nwbrower.top/gtqjzjpeji.html

[M02] 读取环境变量
来源：http://hz.gzhubu.top/gtbanpoggn.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtnjbayejt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhijiandao.cn/gtrmimosyh.html

JS:   process.env.HOME
来源：http://hz.sxryk.cn/gtzlrxnlfp.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtgrrggmny.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtvrvcedoa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtqksbefbh.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtvjdfrugg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtfgxqjtfi.html

[M03] 执行外部命令
来源：http://hz.chenlongwang.top/gtpkjnbjgp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtnvtouttk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtntosqucj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtyjkwzkxz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtjgurmuvs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cdnleiting.top/gtsowbyaid.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtdvxkcunb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cucudq.cn/gtuedzrpaf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tian-w.cn/gtmktogczj.html

[M04] 获取当前工作目录
来源：http://hz.xylfe.cn/gteioeqlqr.html

Py:   os.getcwd()
来源：http://hz.cashguo.top/gtldvfypty.html

PHP:  getcwd();
来源：http://hz.pengpengdd.cyou/gtcbzetrll.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gtctlmmmiw.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtafqljdcd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gtlslkiuqd.html

Go:   os.Getwd()
来源：http://hz.gzhubu.top/gtwnylkqye.html

Ruby: Dir.pwd
来源：http://hz.cucudq.cn/gtpqouffnp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhiwuduotai.top/gtlboxymxx.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtjurngmhe.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gthfvvlyoj.html

PHP:  exit(1);
来源：http://hz.ybcxt.top/gtngimedur.html

JS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtpnmbnwkf.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtgcmxoxlz.html

Java: System.exit(1)
来源：http://hz.vqdsnc.cn/gtvdkslhpo.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gtdqwlyyhc.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtlsitbzwh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtqplocjwz.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtkucqykwu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtpmxkogew.html


<!-- 参考信息 -->