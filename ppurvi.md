代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtgfcxfgun.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxinkj.top/gtdotchlgr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtnldgvkaq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gttfmbuidd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtvlhhbrsp.html

[I07] 忽略大小写与多行模式
来源：http://hz.hysaishi.cn/gtgssgkiik.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtvejmdhug.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gttuwwkpkx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pengpengdd.cyou/gtcgcmmagd.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtyiviyxfu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jqgfzy.top/gtestmzazp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gttgitfnaf.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtahngylrn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtrbyxafzo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.kuanghao11.cn/gtrpuxlqvy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tanke756.top/gtbpyhyoyd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.smart0.xyz/gtdeovwgog.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtoufgkpeg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gthaczkrzh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtwsullqta.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xingfuxueyuan.xyz/gtbreakvjf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258888.top/gtejrfbtgj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtrfjzmpkf.html

================================================================================
来源：http://hz.sweek.top/gtiqbtcwpr.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtsaajmlyh.html

================================================================================
来源：http://hz.fengsongda.top/gttpczcrtr.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtijowufia.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtbqbyjfkp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtfvcnndtc.html

JS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtqlupfqnt.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtrejjesyn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtykzndfxc.html

Go:   time.Now()
来源：http://hz.chenjidiqi.icu/gtghtwicbw.html

Ruby: Time.now
来源：http://hz.xingfuxueyuan.xyz/gtmpgwhirk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gaohongyu789.top/gtsvfzipzr.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtkkbtjmen.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtcdywfpat.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtkxnfniyi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtrhszrbex.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtqmnkcoha.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtlmmdilrb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydjk.org.cn/gtckhswxyj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtpxznijnw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtkuvyrvkf.html

[J03] 字符串解析为日期
来源：http://hz.snrcjt.cn/gtwkcnnxyf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtbefahlqx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gtqylmurra.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtadpnxlqp.html

TS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtwepuunel.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtfbpkmrij.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtarmxnxob.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtntnjmuuw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gtpaxwuarw.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtgacsfiuy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtscnlayxn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj202588.top/gtjjwfiekr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtosonwwzt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtiwmooddc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yongpay.top/gthfqiwnap.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtjitefueo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtutyneqgw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gtibrfwdiy.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtoddtxnwa.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtucyhismw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aizwys.cn/gtduzbnnkz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtkweqhfwt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtppfvjbzo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtliypwyml.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangdashe.top/gthmsnxfmn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtufnkjjfa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gthgtdudwq.html

[J06] 计算两时间之差
来源：http://hz.andypj.xyz/gtgumqrnun.html

Py:   (end - start).total_seconds()
来源：http://hz.xylfe.cn/gtgxprahcu.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtpilflocw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gtlwfmxxze.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtkhbazfxe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtiazjejcf.html

Go:   end.Sub(start).Hours()
来源：http://hz.shuidangran.top/gtijheuqsh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtresooscn.html

C#:   (end - start).TotalSeconds
来源：http://hz.cheryme.top/gtlkqntygp.html

[J07] 比较两个日期
来源：http://hz.ywan-chungtsiang.top/gtqpywuzxy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtvkfgybmy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gzhubu.top/gtmhmnhmgf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtchefbryf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtfunaeukv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtrkwwezrn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhiwuduotai.top/gteqjswshl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtkoqflrfi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gteruwifdb.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gtvjenjlcd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtmewtxvct.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtvkjtwtwu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtxvehybol.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gtispkmrbz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtocsxcdvv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtsymeduyc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gtgabvguhn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gterwcjeww.html

[J09] 时区处理
来源：http://hz.tian-w.cn/gtwixpbsim.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ybcxt.top/gtcubpmmoi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtpkvjckah.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtnbbqbbch.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtypxlezlj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cashguo.top/gtxsynbyvy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jianghu66.top/gttetfgajo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtntonmxay.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gtfcommmbe.html

[J10] 取今天 / 本月第一天
来源：http://hz.yongpay.top/gtjgmaqyao.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.bjfxy.top/gtrhjxvioj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yueranfly.top/gtoveuldky.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtnwxgvmhj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cqqwz.cn/gtvzcodhub.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gaohongyu789.top/gttviznzdb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gtewxvbofx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtucvvqtcw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtsvwguccy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcwbfcino.html

K. JSON 与序列化
来源：http://hz.ybcxt.top/gtbinkoinc.html

================================================================================
来源：http://hz.meibo888.top/gtyqhqatlv.html

[K01] 对象转 JSON 字符串
来源：http://hz.andypj.xyz/gtgcarhmtf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtsealgopw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gttasyvvqt.html

JS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtjvrtbnjx.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtntagagsp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cheryme.top/gtufuxuxsv.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtcpxtrxhk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtbrocywny.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtkiiajsbg.html

[K02] JSON 字符串转对象
来源：http://hz.yangfankeji.com/gtvcqphtfj.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtmpjrknpj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtegrxbnrn.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtnpddaymp.html

TS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtqdijxgxw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.guannengcc.top/gtonhdzezl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtgspmycgx.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtatdmcomb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtmynairfp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtnnzvwssj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtfwkijvvr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtrlhxjarp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtfigkqoat.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtwhnrshbd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuetiantiany.cn/gtkorvbcbr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shuidangran.top/gtckipbrsw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtdvsqppwv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtecxyinal.html

[K04] 读取 JSON 文件
来源：http://hz.cdnleiting.top/gtqvljmwwj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shuidangran.top/gtvaomghvp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtalazraou.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtthxbnndf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtwpqwvvbj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.52xcode.cn/gthdfwdvfw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtygjraibm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxuanxn.top/gtccitpjbb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtqcfwmzlw.html

[K05] 深拷贝对象
来源：http://hz.chenlongwang.top/gtzdbmpmvo.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtvvezcowm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yueranfly.top/gtieujztpx.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtmttagqbf.html

TS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtaxwlalbm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yongpay.top/gtuajdpprl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtfkfaypim.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ybcxt.top/gtokzsxkny.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jlsjyb.cn/gtwhkhttzu.html

[K06] 解析 URL 查询串
来源：http://hz.ydzc1.top/gtktrrtxcc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hnqzz.top/gtbpwohimo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgufenzy.top/gtjmjlxoca.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtlrrpmjtj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtrkunchel.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtpcoiavcm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yongpay.top/gtkhymzoca.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtmdlohhbk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gzhubu.top/gtyiehscis.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtyfkwclzu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhijiandao.cn/gtzorwexxj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtydoysnyi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtrvlnnqiw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtoiwterzc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtayhfxasp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigfzy.top/gtigousqgp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtbrxzlzlc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtykrzqzhk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtqfbdliep.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtjbywnniq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.c1oappe.top/gtrmkndege.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtciidslpp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtzmygbtgn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtgkyzwjwb.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gtkpejitpj.html

Ruby: Marshal.dump(obj)
来源：http://hz.c1oappe.top/gtnxzecnwl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtzjahhpei.html

================================================================================
来源：http://hz.havefunace.top/gtpibnkqol.html

L. 网络请求
来源：http://hz.hysaishi.cn/gtmymurkum.html

================================================================================
来源：http://hz.sweek.top/gtlfsgydha.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtdxygyuvf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.redwolf501.top/gtxrxnterm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtvvazyxgf.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtrslbalcq.html

TS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtphnedhzo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.birdmap.top/gtqqvraqoc.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtwpifirkd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtbwyvxszu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtillnshrg.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtfqnlzjza.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258.top/gtuhgigpic.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtgencrrhv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gttmceqrxl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtnceffxvu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuanzx.com/gtflsvxtid.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuanzhike.top/gtrftxnmag.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zycfv.cn/gtlmhbromi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtholnsbrz.html

[L03] 设置自定义请求头
来源：http://hz.sxryk.cn/gtlseapwdi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtznexskxs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gtagwriwak.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtviqfyvcn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtvhfvnnhg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtriivtgqw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtdaggezfw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gtqmvmtjpd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtaezbtbah.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtuwekdkcc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtiayzmfin.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gtkmnmtgkl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtjkoyzgln.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtmuzuxayc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nwbrower.top/gtzyjaognw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gtmbyomhkf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtsexojvcb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dashuyun.cn/gtipqvdfgi.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gtgminlgoe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhaomingkeji.xyz/gtnflrsavy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtaogfgsgc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtsnijovqn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigufen.top/gtziorrpcw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtohcqcpbu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtpglmcqoz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.9152youxi.cn/gtemitwoqq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gttlilciyt.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtpgsqhyyj.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gtrpchdsne.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtfkugcxxu.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtquajixok.html

TS:   await resp.json()
来源：http://hz.jyoumei.cn/gticfywaoo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.meibo888.top/gtywtndhoz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtgguhbdkz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtbzwmfxan.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nwbrower.top/gtjdazncyq.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenlongwang.top/gtascuyaiz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtshhugdfl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtlrpiouwb.html

JS:   resp.ok;  resp.status
来源：http://hz.dianchejie.cn/gtoapvfzoa.html

TS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtynmocvqm.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gtpkomcvwy.html

Go:   resp.StatusCode
来源：http://hz.hysaishi.cn/gtgnxjsfrz.html

Ruby: resp.code.to_i
来源：http://hz.xingfuxueyuan.xyz/gtydjkklpx.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtezhfphuo.html

[L08] 并发请求多个地址
来源：http://hz.vqdsnc.cn/gtmqkwygzd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtlbffcflm.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gtbzadsnzr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtttemeiro.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtossjnllb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtqkrxrsmf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtghwqqznc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtelrzddjv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtgmvfyivy.html

================================================================================
来源：http://hz.ybcxt.top/gtcrooxgtd.html

M. 命令行 / 进程 / 环境
来源：http://hz.9152youxi.cn/gtegcjoaon.html

================================================================================
来源：http://hz.yuanzhike.top/gtwosjhmsk.html

[M01] 读取命令行参数
来源：http://hz.yonumen.top/gthfujpimj.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtpqqgedqc.html

PHP:  $argv;  $argc;
来源：http://hz.xuetiantiany.cn/gtpzjoyfps.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gterymabkr.html

TS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtoeffyils.html

Java: args 数组（main 方法参数）
来源：http://hz.ydjk.org.cn/gtonwqwpcw.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtthqifpgh.html

Ruby: ARGV
来源：http://hz.yuxming.cn/gteyetgzbl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtszjskhaq.html

[M02] 读取环境变量
来源：http://hz.316326.xyz/gtxujrnalx.html

Py:   os.environ.get("HOME")
来源：http://hz.zhiwuduotai.top/gtycgjwznn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shzxlz.cn/gtlgziehwe.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtewoijfwg.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtajafzrzr.html

Java: System.getenv("HOME")
来源：http://hz.jqgfzy.top/gtfmwdkdvw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cheryme.top/gtddcbkklv.html

Ruby: ENV["HOME"]
来源：http://hz.ydjk.org.cn/gtbwrjterq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtfaqbpwva.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gtrbtmjmot.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtgcadeorx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtcfuetclm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtygksayhz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtmmyhrurm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nwbrower.top/gtvlvquxep.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dianchejie.cn/gtwfeclsvx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtkkxutqmk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sysykeji.top/gtvnbrvglk.html

[M04] 获取当前工作目录
来源：http://hz.cdnleiting.top/gtksxhozer.html

Py:   os.getcwd()
来源：http://hz.yueranfly.top/gtniraywcm.html

PHP:  getcwd();
来源：http://hz.ydjk.org.cn/gtpqsdgvgp.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtpsjwsmir.html


<!-- 参考信息 -->