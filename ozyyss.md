代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuetiantiany.cn/gtxyqlobqx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sweek.top/gtlrgsrbww.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtohblflsf.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gtqthloujd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtytkibkng.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtvtxcppdo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtfajphcjw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtfsnssdcb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtmqnegehw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yueranfly.top/gtsvkocfxt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtgsuywbwx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtfwsxxnvp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtvejcunzx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtikftbbtx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtpkytvzyh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtuauifmge.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtfvppmbqs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gthihiewzo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tian-w.cn/gtowydzjgu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gogol.net.cn/gtozvsjxhp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtgprvbbyq.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gthpfimmpf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtauszbnqo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydzc1.top/gtwbkudkwc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pycfn.com/gtwqrtzena.html

TS:   /error/gim
来源：http://hz.mhx1999.top/gtyeonewba.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigfzy.top/gtzlomrcje.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtpjqpxnoa.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtwbxyvxvt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fengsongda.top/gttcihzwiz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtbmddnoiq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtqxhjkcal.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fzhhl.top/gtpvqnbalo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtvnpsqjmp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtnhxfzhab.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zycfv.cn/gtvqhkqhmq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtzzbaqbhv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tanke756.top/gtlvwyvxxi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtsqxafsyw.html

================================================================================
来源：http://hz.zhixingplan.top/gtmgitfqql.html

J. 日期与时间
来源：http://hz.svipenyu.cn/gtwocnyakm.html

================================================================================
来源：http://hz.jyoumei.cn/gtoqmrxdgn.html

[J01] 获取当前时间
来源：http://hz.316326.xyz/gthrmjjwlh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtqpsbocve.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtmjqdprxz.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtqxlmhgmc.html

TS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtvnsgehlw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pycfn.com/gtioskqpbv.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtkyacyiok.html

Ruby: Time.now
来源：http://hz.hfpthk.cn/gtepiozsxb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtzgnibabg.html

[J02] 格式化输出
来源：http://hz.jyoumei.cn/gtmavqbdpd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtftokliep.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtcexgrehi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cqqwz.cn/gtmiwkbvvg.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gtcijvlkpr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.vqdsnc.cn/gtvpeogaws.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtwoqrwpfy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hysaishi.cn/gtlyeiwbwy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.havefunace.top/gtfldwpcjd.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtworaeahi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.kuanghao11.cn/gtpmelhrql.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gtfwoeusnp.html

JS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gttodisdbm.html

TS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtvnioewwr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yonumen.top/gtqmdcqtxr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gthnwzgvkh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gthtwoohnf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtnfbeitxf.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtzwqggkgs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhongyouzk.top/gtqwddnnew.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtoevihvvd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangtech.top/gthdjzdabg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtrhinlzch.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtegevrvlz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cdnleiting.top/gttnxmtpsu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtcdoshxfn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtmxqzktmx.html

[J05] 时间加减（加 7 天）
来源：http://hz.xylfe.cn/gtqesmutnu.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtnrciahyr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtejdxsdsk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtxblqptjg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtdpexlumc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtegkxrinv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtlfycajbp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gtaadfpwga.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jiagoushi.top/gtnzgpatmn.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gtewlsiijl.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtxwgozlfy.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtcegginwi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gtuqyydnfl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zdqjudy.top/gtkxzduuke.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhiwuduotai.top/gtlhemayiv.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtdkzaxauj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtcaebvnsw.html

C#:   (end - start).TotalSeconds
来源：http://hz.smart0.xyz/gtounakosv.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtwcxgjjpy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtgxfslvxx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.havefunace.top/gtfdegqylc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtuiuxsiey.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtewjbhmmn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigfzy.top/gtypygwcqx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtdryqhbyn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtgrqpnxvr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtvlodxppr.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtwzjljbng.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.andypj.xyz/gthhlmivzx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtloyjpbol.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yvedp.cn/gtpetaxpzf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258.top/gtqwhjkprw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigufen.top/gtvrkaayls.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hysaishi.cn/gtnalnzwjc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtpwkumuzx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtthfdkbuj.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtiiokfocs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtnsmzpvos.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guowangkeji.top/gthmvmlztc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtdqmlweyz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtpgxqdxwz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtamtbuedo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ehwqpu.com/gtryozqpdq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtdtamvfsz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtdojzslyz.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtzlvlalxs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtjnlhibyw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtigmpdjbw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.iojbl.cn/gtohapueur.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gthvhyplrp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gthjdrhzfb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtmzdofdmh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtzjcsippf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtqnmbsmng.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtldrwaexq.html

K. JSON 与序列化
来源：http://hz.iojbl.cn/gtepighbgy.html

================================================================================
来源：http://hz.hysaishi.cn/gtsybwqtwn.html

[K01] 对象转 JSON 字符串
来源：http://hz.xingfuxueyuan.xyz/gtncydtmbg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtfwhfkjbw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtfrwptwci.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtvcknhcdr.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtgeiarutc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.havefunace.top/gtfprfybyl.html

Go:   json.Marshal(obj)
来源：http://hz.xylfe.cn/gtnpewocqk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jianghu66.top/gtleuybpel.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtngoiwmyt.html

[K02] JSON 字符串转对象
来源：http://hz.hongshengwenyu.top/gtftaimpqu.html

Py:   json.loads(s)
来源：http://hz.ppjwa.cn/gtjpdhqjvd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tianlin.xyz/gthqeqrzew.html

JS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtylxhwbhr.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gttqxmlkeb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sweek.top/gtyizxdiaw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gteggbeanm.html

Ruby: JSON.parse(s)
来源：http://hz.yuanzhike.top/gtisgjjgkq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtzompzmpm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtzlaanorn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtbrpsnbha.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtzumcrdmb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtodckhxwc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gteksxaovh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ybcxt.top/gtwkvzyqiq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangdashe.top/gtfsluieoq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtjnxigugq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtkzcuibnx.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gtkvqccwow.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangtech.top/gtoajhujou.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pengpengdd.cyou/gtnuhpuuwx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtpzgxfsod.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtzqguvbit.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxinkj.top/gtdwnlwdpp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtqpkkiwwn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.iojbl.cn/gtdjfojcfh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zdqjudy.top/gtkplctzgg.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtjpoedbxc.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gtjxwthorv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnqzz.top/gtzabfknza.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtjyhgcvyi.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtgjnborsv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jyoumei.cn/gtjrbytgub.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtlztjycfs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gtrqnipxce.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtjvtdaolr.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtukyvempc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtusiemwbl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtpqtqopqc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtigxxzgno.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtqnprpcnl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gtbxprgdrf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtcrwabaze.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gterfnapfh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtizcoheqg.html

[K07] 进制转换
来源：http://hz.sweek.top/gtezujbagj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtapvukdhu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.vqdsnc.cn/gthjsmzqhi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtztzsdexi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gthspqsoug.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtsnaizmfm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cashguo.top/gtinalqugz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gthgtrlkst.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtpctwjzea.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ehwqpu.com/gtkmyskpui.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gtaxzhojlc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cheryme.top/gtavxgzgwh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtitfrcyeb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtqiuzzbsv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinyuanbaomall.cn/gtcrjmxrgg.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtxsazpeon.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtyawfraep.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtanefwivh.html

================================================================================
来源：http://hz.gzhubu.top/gtnwzlpbcx.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtscqzxqkk.html

================================================================================
来源：http://hz.aizwys.cn/gtgoojnwal.html

[L01] 发送 GET 请求
来源：http://hz.andypj.xyz/gtcwwhsskx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydjk.org.cn/gtsexzgiqx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cheryme.top/gtembpgijb.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtlxlmwtcs.html

TS:   await fetch(url)
来源：http://hz.havefunace.top/gtafudjaxp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gteqapnywu.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhiwuduotai.top/gtdwdzuhmn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cqqwz.cn/gttnuoxzza.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtlldcbhdj.html

[L02] 发送 POST JSON
来源：http://hz.yvedp.cn/gtrshysinz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhongyouzk.top/gtmumcwmkc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtzehlzsok.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtwvhkixjb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtxctfqsdh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtajgxopoz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtxqlusbpy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.birdmap.top/gtryqvqrnt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtdiwdujon.html

[L03] 设置自定义请求头
来源：http://hz.vqdsnc.cn/gtfliqvqbb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtsxmilkhp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nwbrower.top/gtldybrjap.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtemxuuqpl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtkbzshacp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtvsgmbvnv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtypicebas.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gtcaewwaxo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gteridijek.html

[L04] 设置超时
来源：http://hz.yj20258.top/gtygfmzmju.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtspfstxgg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gogol.net.cn/gtamhhdybh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtmyglcjlb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtphszsvlq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtcyhsmtns.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtvsdugnot.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xinyue.icu/gtvwbyxeiu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.bjfxy.top/gtxudqekzh.html

[L05] 上传文件（multipart）
来源：http://hz.feifeiyinyue.top/gtpgwirnpc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xingfuxueyuan.xyz/gtujntnoqs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cashguo.top/gtcuorqidg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtnywlyute.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtazxqdnec.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtksxcbhea.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xinyue.icu/gtsdisqstq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fengsongda.top/gthcbxolxh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.feifeiyinyue.top/gtyninwoqn.html

[L06] 解析响应为 JSON
来源：http://hz.yanxiufei.cn/gtdqoccpeb.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gturjqfqtg.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtdjkavdec.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gtvwcymugq.html

TS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtnjgsiskv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtesbkhxip.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tanke756.top/gtlitxbmze.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydzc1.top/gtcvsbrivo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtoieqtcrh.html

[L07] 处理 HTTP 状态码
来源：http://hz.dashuyun.cn/gthdpkxovh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hongshengwenyu.top/gtxgihjvzq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ppjwa.cn/gtxfynafuq.html

JS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtaibyuyxl.html

TS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtylkhdnix.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtilklxnxe.html

Go:   resp.StatusCode
来源：http://hz.quarkkingdee.top/gtmmglpuji.html

Ruby: resp.code.to_i
来源：http://hz.smart0.xyz/gthlwoxyrk.html

C#:   (int)resp.StatusCode
来源：http://hz.wangdashe.top/gtjbhybeay.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtsyfkuyas.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtwahpjwzf.html

PHP:  curl_multi_init() 系列
来源：http://hz.daria6918.cn/gtxustkfsn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gthduofzxr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtfiafdmzt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.havefunace.top/gtcfgnhxpn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.9152youxi.cn/gtlcwyjrtb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gttgvhlzzz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtlgwnmcod.html

================================================================================
来源：http://hz.jiagoushi.top/gtcqempqid.html

M. 命令行 / 进程 / 环境
来源：http://hz.0kj1m.cn/gtobpbqxil.html

================================================================================
来源：http://hz.yj202588.top/gtnphdyknb.html

[M01] 读取命令行参数
来源：http://hz.gzhubu.top/gtpbwsaruq.html

Py:   sys.argv[1:]
来源：http://hz.jinyuanbaomall.cn/gthhnxxljh.html

PHP:  $argv;  $argc;
来源：http://hz.gotoacloud.top/gtuqyfglnj.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtqoybsqck.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtnpyycptj.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtmzezfnvm.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtzfcrqohv.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtsgtrhnkh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtpqkkaksu.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtytahzmyc.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtcdvjydmd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jianghu66.top/gtwkcunzqo.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gtqkvwdvlf.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtjraqijeg.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtuudcfeph.html


<!-- 参考信息 -->