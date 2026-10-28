代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.meibo888.top/gtggxjwelq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydzc1.top/gtfbgjjkdf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtzmyaskaw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtwktdjlay.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtlrmobrlx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtdnlnozvo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtbgrphrbh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfdbwhqcv.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtcvnwnrmj.html

================================================================================
来源：http://hz.xuanzx.com/gtqbnsjsvw.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtwpkkvmet.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.havefunace.top/gtohppgphk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtgyqymwjs.html

JS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtfomckwmh.html

TS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtlijwljdg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gtispwjbym.html

Go:   time.Now()
来源：http://hz.jinqigfzy.top/gtvmuvrzwt.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gttqicwnin.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hammf.cn/gtehoxyuks.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtqkziwexx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtqvayazkm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtuyjhudpk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtjrptvlxn.html

TS:   d.toISOString()
来源：http://hz.pengpengdd.cyou/gtvtnmctvr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guowangkeji.top/gtihdzehqv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hysaishi.cn/gtvtcpioma.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtadzfdcol.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgufenzy.top/gtqjjlmewu.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtldfzjbwp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydjk.org.cn/gtzbpnwkqo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinghuilouyu.cn/gthdxvyult.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtpnkqfluw.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtfgjnkjji.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnxiangtu.top/gtzduqauba.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtrfoibldq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sweek.top/gtshkmybco.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.daria6918.cn/gtpbcymgkd.html

[J04] 时间戳与日期互转
来源：http://hz.gogol.net.cn/gttpiqxpxo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gtbscesasb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.quarkkingdee.top/gtdabkcbzu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtlbipwigu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtjoowjkox.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtmdrcgzvj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shuidangran.top/gtuypvevhx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtjyxqtdqd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtdglyxtev.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtwuzmrozh.html

Py:   now + timedelta(days=7)
来源：http://hz.shuidangran.top/gtlvcggjes.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtsimwhiqq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtyghzseay.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtggcjpetw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gthwggjztj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtnkbdpchl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgfzy.top/gttyomfjzz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hongshengwenyu.top/gthbueqsjy.html

[J06] 计算两时间之差
来源：http://hz.ivvv.top/gtdvqsemsu.html

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gtfxsewbrh.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtlcbbaikz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xylfe.cn/gtqplvlobz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aizwys.cn/gthalzmian.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtxjkvwxhs.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtehobtzuh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtjbddpecx.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtepeqjnwk.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtzsviqugj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtdrwwhqgl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.9152youxi.cn/gtrdvkejco.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtewnzgvys.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtboabeerj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sysykeji.top/gtcujgtcia.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtxagwwpxs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtglsbvrli.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtelavtunr.html

[J08] 提取年月日与星期
来源：http://hz.yvedp.cn/gtwocaiewm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtybggpriz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.smart0.xyz/gtxpkrpevy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gtgfdejuzk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtuwttsjna.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ybcxt.top/gtbojpdqiy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangkeji.top/gtehiwtyqu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtnxgvvykn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aibaodan.cn/gtzrmytkzw.html

[J09] 时区处理
来源：http://hz.zhixingplan.top/gtiyemoajv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinghuilouyu.cn/gtdpthsllm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtgubgwlhv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtqqjwhgsq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtfczbjtpv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gtzhhreidn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yj20258.top/gthrlsduxf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtshjmorsc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.bjfxy.top/gtlwmxxirm.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtktqvfkck.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yonumen.top/gtqirlwnwx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtlxtwhvcw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.haohaochexian.top/gtxtgqgbkj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtpfeaghhq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtxjmclipx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtmyrvqydm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtejfkgtxr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtxrkyptct.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwdfluyfl.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtscazgzbu.html

================================================================================
来源：http://hz.xylfe.cn/gtzkzcoqic.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtpznrkdsg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtetzcpuev.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nwbrower.top/gtwttievvv.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtwkfbpmku.html

TS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtmudahgcd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtxuyqtrwr.html

Go:   json.Marshal(obj)
来源：http://hz.shuidangran.top/gtuhpdlyct.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gtupbssvuy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhixingplan.top/gtxtdhtoia.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtfqikzmov.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtgivyadhb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gttnicipzy.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtevuvuweq.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtksykphny.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtkvfmnmjq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtfsziktfd.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtxcpquoxm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtdjhvqcag.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yanxiufei.cn/gtumznvcze.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtsuqwopbe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtjoeqxain.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtzkvibfpz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtkcphhjfc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gttwlugufu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtpwzvxhyg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtxpymosyx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtsmhhwhym.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gtigngvwtl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tanke756.top/gtklcknrij.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj202588.top/gtknenqqjg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gttqxxamfd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtibxnrztg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtfrzzvolo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtztotrezm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cucudq.cn/gtbktnqspn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtldlwrdts.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtbemztwto.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gttagqhzsz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtowigyyxx.html

JS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtfdildqdf.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtsrnblbmn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtxnlkpeuj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.svipenyu.cn/gthnmmsfyb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtbttiotqt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtvobgkhoh.html

[K06] 解析 URL 查询串
来源：http://hz.bjfxy.top/gtyafyusxy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtyytllqir.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gthvzdcnfi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gthdwsgeyz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtwfsswzeg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sxryk.cn/gtcxfljhek.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtushiupeg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gtytavwtht.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtjqawtdqq.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtexbmcrvn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aibaodan.cn/gtccwtmfud.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtexdczzdw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gttheqcrkr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtsgshqjtt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtsuhecrca.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtpjmnpuff.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ivvv.top/gtlozxlmai.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtbxzxwgbd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtwuueetxi.html

Py:   pickle.dumps(obj)
来源：http://hz.guannengcc.top/gtbvkdovdy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuanzx.com/gtdmbvxsrg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhiwuduotai.top/gtdayrpcxa.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtieeykrgt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.mhx1999.top/gtnlzaahhg.html

Go:   encoding/gob
来源：http://hz.yvedp.cn/gtcdxafbnt.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtkrqmowvm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtrytsgqwn.html

================================================================================
来源：http://hz.fzhhl.top/gtervmuxvh.html

L. 网络请求
来源：http://hz.xuanzx.com/gtwvpvddxm.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgbhrhuey.html

[L01] 发送 GET 请求
来源：http://hz.0kj1m.cn/gtohmtupfe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtejekpbcr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gtbeafvtkq.html

JS:   await fetch(url)
来源：http://hz.yj20258.top/gtaetqwnpp.html

TS:   await fetch(url)
来源：http://hz.shuidangran.top/gtyqkyftlw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhoulong.xyz/gtripweswr.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtgjixrdqm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxinkj.top/gthpwdikem.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigufen.top/gtaybkvbcg.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gtubtuimzq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.meibo888.top/gtaazcdrvi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tanke756.top/gtlqzschix.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtekbemhap.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gtgsplmljv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gttndgneut.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gttkuchwtb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.birdmap.top/gthpnyeqns.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cqqwz.cn/gtpyfxwmiw.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtgnjqdqxr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtmpuzwpeo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtmkdckczu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtdbxmrabx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtzeukrgot.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gtcjrekppb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtfqbjkplo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtcgowugnz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtnpiqndrm.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtnmantvsp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sufxvd.cn/gtgvmqxkyv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guowangkeji.top/gtpxznveky.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtrzykrboa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtazwrydlm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gthqxcgyor.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jiagoushi.top/gtmasdhpdi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtbpgivbof.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtllgahmkh.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtagnppwpp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtfszbelsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gthfaffhzw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtoqvslxos.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtbkxzssgj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gotoacloud.top/gtzbhpyrwe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gtffsymamp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtsajyefnj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.pengpengdd.cyou/gtsqqmusqc.html

[L06] 解析响应为 JSON
来源：http://hz.guannengcc.top/gthbufixps.html

Py:   resp.json()
来源：http://hz.sysykeji.top/gtoocgyfdt.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtntfjflwo.html

JS:   await resp.json()
来源：http://hz.pycfn.com/gtkvpqeroh.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtaonflnuz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.316326.xyz/gtxkjdjmhv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gtlgacxlln.html

Ruby: JSON.parse(resp.body)
来源：http://hz.bjfxy.top/gtfirojabp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gzhubu.top/gtluqdlzhi.html

[L07] 处理 HTTP 状态码
来源：http://hz.aibaodan.cn/gtrxyfqvfi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sxryk.cn/gtzbqjjagn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigfzy.top/gtudabdotd.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtsbussnbd.html

TS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtwnyzfymx.html

Java: resp.statusCode()
来源：http://hz.yvedp.cn/gtlwrswlgz.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtlkuxlskh.html

Ruby: resp.code.to_i
来源：http://hz.kuanghao11.cn/gtnxegfoqh.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtcjtzbjhh.html

[L08] 并发请求多个地址
来源：http://hz.hysaishi.cn/gtcjhiwpap.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtbcvewtva.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhoulong.xyz/gtoahtazlk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtpafzmdxy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtlrppbjbn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.dianchejie.cn/gtnjejojpu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtcghbstph.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gtfkdzsbfw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigufen.top/gtgbptrszx.html

================================================================================
来源：http://hz.birdmap.top/gtdxfdnxmg.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtisfpzjho.html

================================================================================
来源：http://hz.yueranfly.top/gtpgkawgnk.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtqvkjbncx.html

Py:   sys.argv[1:]
来源：http://hz.hysaishi.cn/gtwellonbb.html

PHP:  $argv;  $argc;
来源：http://hz.sxryk.cn/gtxgncskzh.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtzzkjoezb.html

TS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtfuteikhm.html

Java: args 数组（main 方法参数）
来源：http://hz.zdqjudy.top/gtkgaerwtu.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangkeji.top/gtdggkpzxd.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtupjhdlwh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtxpqsedvx.html

[M02] 读取环境变量
来源：http://hz.chenlongwang.top/gtfyosozmt.html

Py:   os.environ.get("HOME")
来源：http://hz.xziqi.cn/gtmxhwvpoy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gttueomrfj.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtulkwaigv.html

TS:   process.env.HOME
来源：http://hz.wangdashe.top/gtylnkxulp.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtljijvacw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258888.top/gtvxhyieji.html

Ruby: ENV["HOME"]
来源：http://hz.tianlin.xyz/gtocaovpxh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aizwys.cn/gtenwhhcvc.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtpspukqej.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigufen.top/gtsgegsqvj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtjvherlxj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtftrwtmwk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtnwwulfar.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fzhhl.top/gtgrkkwddc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtteymdolv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daxiang520.top/gtkfpeczpi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtjdxwbjyt.html

[M04] 获取当前工作目录
来源：http://hz.sysykeji.top/gtkxpnztog.html

Py:   os.getcwd()
来源：http://hz.pengpengdd.cyou/gtqtjrcwkk.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtxfghvslu.html

JS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtjfshkida.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtsopzdtbb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtlfxdcrsf.html

Go:   os.Getwd()
来源：http://hz.c1oappe.top/gtlthkofxv.html

Ruby: Dir.pwd
来源：http://hz.hnxiangtu.top/gtikzaoemr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnqzz.top/gtyutayecf.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gteheycfru.html

Py:   sys.exit(1)
来源：http://hz.wangdashe.top/gtuecbkwyl.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtatproqgk.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtoqpgykcr.html

TS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtbciowkxy.html

Java: System.exit(1)
来源：http://hz.yuanzhike.top/gtqyshmecj.html

Go:   os.Exit(1)
来源：http://hz.pengpengdd.cyou/gtlbgnkaar.html

Ruby: exit 1
来源：http://hz.daria6918.cn/gtnvermaqe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtbzvxjuhn.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtbynfxrqd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.52xcode.cn/gtersrvvwg.html


<!-- 参考信息 -->