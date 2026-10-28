代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtlnbxofqw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtiburgatt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtqzmieavq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtzjonemrf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtjrhqdtye.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtjrpvibmj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258.top/gtkutftkcv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gotoacloud.top/gtjbltestr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtykvszhdz.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtmlgkivcg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shangyingyoupin.top/gtyfjyuefb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yanxiufei.cn/gttzklpcnd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gaohongyu789.top/gtntqlybdn.html

TS:   /error/gim
来源：http://hz.sysykeji.top/gtuafmyhmk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtwznynzye.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtkurgtafy.html

Ruby: s.scan(/error/i)
来源：http://hz.svipenyu.cn/gtycfuwgre.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtwuetcoaw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.andypj.xyz/gtmcnuxlme.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gtqyojjutm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtelvzffme.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtguzosadk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtrfwexysy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtbkrthpxp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj20258888.top/gtlqzobqmw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tian-w.cn/gtlvbjpevk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtmvjwhgds.html

================================================================================
来源：http://hz.yuanzhike.top/gtikpsbptk.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtnweyywei.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtwrzhejcv.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtmglmotth.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtmwfxvldh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gttjfxezag.html

JS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtgnicqahj.html

TS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtzlxoyukq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtsvtvmocp.html

Go:   time.Now()
来源：http://hz.yvedp.cn/gtvdflltwk.html

Ruby: Time.now
来源：http://hz.xuetiantiany.cn/gtsfcthgpl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtgglzyvwe.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtxwqyhoaq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtdbppandj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gtqsmhslyl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtmkhjhhpb.html

TS:   d.toISOString()
来源：http://hz.sysykeji.top/gthiovuozi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhixingplan.top/gtxjdwcgeb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.svipenyu.cn/gtbucugyvp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtqkczdnxf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jlsjyb.cn/gtyakxkxlj.html

[J03] 字符串解析为日期
来源：http://hz.nwbrower.top/gtwhbwthoy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtayycdlnb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shangyingyoupin.top/gtifbbpelu.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtrfwlnume.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtfsjdwazy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtiuxbshjq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sufxvd.cn/gtujvyjxvd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtdoyceusr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtkkgzigaz.html

[J04] 时间戳与日期互转
来源：http://hz.nanxinkj.top/gtykodczos.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtipfivlte.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangkeji.top/gtvxkrjvzf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daria6918.cn/gtfeebrrpb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnxiangtu.top/gtrojnuyfd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtlbtiqwlc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtcngcioze.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinghuilouyu.cn/gttbguopeg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtyeudieqc.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj202588.top/gtnqqdcmsz.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtjcqcfkci.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daria6918.cn/gthkxrffwt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtvrnpinos.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtgizwvbux.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangdashe.top/gtvwrwdoqz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtboqdraoy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yangfankeji.com/gtwoigupbl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtjqymrvtx.html

[J06] 计算两时间之差
来源：http://hz.yvedp.cn/gtozcbacwm.html

Py:   (end - start).total_seconds()
来源：http://hz.aizwys.cn/gtesqtnpvx.html

PHP:  $end->diff($start)->days;
来源：http://hz.aizwys.cn/gtvgtghzlv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtyxolydco.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xingfuxueyuan.xyz/gtydamwmok.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.bjfxy.top/gtxhxhqziu.html

Go:   end.Sub(start).Hours()
来源：http://hz.guowangkeji.top/gtxuwbeima.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtcvlbryoe.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangdashe.top/gtjcpvuhoc.html

[J07] 比较两个日期
来源：http://hz.birdmap.top/gtqrlwltlk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtpccinsgf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtfshygebt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtedkysspw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtrlpkoqdq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gthtqcvkyb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gtruomgatw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtvihyjfwc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtmtbcfabv.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtnuutjdfz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gtribelofa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtplccpxdm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ehwqpu.com/gtvonbplsa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtfigzmxun.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtmvjhrtbq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guowangkeji.top/gtlibpggrt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydjk.org.cn/gtrdkuqhin.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ybcxt.top/gtqkxeigcj.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtkszqkchl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinghuilouyu.cn/gtxvtfxkgl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtrteoizuq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtblguiubk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtgxolekub.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gtwacdksyc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtjcaoomiu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zycfv.cn/gtpmlcgsvg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtpjwcpmer.html

[J10] 取今天 / 本月第一天
来源：http://hz.shzxlz.cn/gtdnwoekvg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhoulong.xyz/gtfbctksup.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gticpldkov.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yanxiufei.cn/gtebwjdbpq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cashguo.top/gtirazlmcp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtajnkisll.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtqgukyvoq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yangfankeji.com/gtpnvrdqyk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zycfv.cn/gtsrkzdkfg.html

================================================================================
来源：http://hz.cashguo.top/gtmqkgqnqc.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtxztxgbhc.html

================================================================================
来源：http://hz.cqqwz.cn/gtkffbnnoa.html

[K01] 对象转 JSON 字符串
来源：http://hz.gzhubu.top/gtyfljhyfb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtpfnrjcof.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtbwgckttr.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtgobezbyk.html

TS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtbwkudqrm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtenddaqwh.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtmidmnhtd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yueranfly.top/gthbwncdgc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtmttvdbcs.html

[K02] JSON 字符串转对象
来源：http://hz.jqgufenzy.top/gtfaqsmcen.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gtoeqkjxzz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtlcvqvvtl.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtrnejlobl.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gteeryafjb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sweek.top/gtgjjzztcf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tianlin.xyz/gtppttugvv.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtgbdfduoe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtawcloptv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtgawxqnfl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtivopqfsk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gttanuelcd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtouhofbhx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtuifiwcwy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xziqi.cn/gtijmhszsc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtkcjfrjma.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gttghbjxdq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtptekathm.html

[K04] 读取 JSON 文件
来源：http://hz.cucudq.cn/gtrayjtmrg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtdxsgsovk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtrqlmisjq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtmydqnbfb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtkobabvyb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtjlpxwldb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtfvskkval.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydjk.org.cn/gtelmfbbqb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhongyouzk.top/gtpswmaewc.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtpiaitmcg.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtdprwhdyw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuanzx.com/gtmzmbztnp.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtxgkdfees.html

TS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtwwzsihtm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dashuyun.cn/gtnvastspg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gzhubu.top/gtiiaucrat.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnqzz.top/gtrmiubkzh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shzxlz.cn/gtntsowtlx.html

[K06] 解析 URL 查询串
来源：http://hz.yonumen.top/gtfzhseibm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtujsfiymn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gttcrexhve.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtfwfepzsv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtsgvplwwv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtknwmymjl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtjsbczzlo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtzxpkhwcp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtthiufdrn.html

[K07] 进制转换
来源：http://hz.cqqwz.cn/gtsqekmmla.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenzaomai.com/gtpifqagkj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gteaftbdve.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtzfhakiok.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtwtksjxzv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtushoxwyu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gthvsfvjpw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gthbrofcvr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtjvnyhksc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.smart0.xyz/gtbrhftorb.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigfzy.top/gtfdvkoaih.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.iojbl.cn/gttajpcldn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtskzehiym.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtrmsgziza.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtsdfjmpea.html

Go:   encoding/gob
来源：http://hz.yuanzhike.top/gtudjveiix.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinyuanbaomall.cn/gtfqiapdre.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtjteazixs.html

================================================================================
来源：http://hz.yanxiufei.cn/gtforoslep.html

L. 网络请求
来源：http://hz.tanke756.top/gtxrtgvneq.html

================================================================================
来源：http://hz.hnxiangtu.top/gtxhnhvhcr.html

[L01] 发送 GET 请求
来源：http://hz.zhiwuduotai.top/gtgmiasjbh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtyenusnrj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtnlepxcyq.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtblfcztwf.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gterqycypb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gtpocqillw.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gtxenunttb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pycfn.com/gthcoxgvap.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtysgxrigq.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gtlaexgbbl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gtvgxxfhbd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guannengcc.top/gtcifxaipz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtutecfvcg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtsncdunnq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gtkjqsuqgx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtdrhivanm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhijiandao.cn/gtomajfarl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gthkacnscg.html

[L03] 设置自定义请求头
来源：http://hz.ehwqpu.com/gttpfobzvv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.52xcode.cn/gtmsavmnpe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuxming.cn/gtpvvqjitx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtbxvreukd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtcnqxypne.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nwbrower.top/gttpqtbykm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gthasjefux.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gtmvhbmjuk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtcpzunqwk.html

[L04] 设置超时
来源：http://hz.hnqzz.top/gtjonrbwnl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxuanxn.top/gtvxynbceh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydzc1.top/gtkhqfztrl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtfrxtusdi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtuudjdhac.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gtreohktse.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aizwys.cn/gtcfenwwrb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtbhurswsc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtkyjwyunp.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gtjblubhhl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.9152youxi.cn/gtidupzfcf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gtqdljknwv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtesqnbcbg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtnehliysd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.redwolf501.top/gtfplrrzgx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtsaujtkob.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtcdlnsepm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gtfffrqrtn.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtqvhmcaua.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtvezgyksd.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gthvworgbg.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gthrupbblv.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gthbkonsyh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtaofslhgf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jyoumei.cn/gtzvhumiix.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtinlvhzjk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.snrcjt.cn/gtvrhijdmi.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gttvjfhdfm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fengsongda.top/gtludclldv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gogol.net.cn/gtejpmygih.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtiyuhowzm.html

TS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gteufkbjtj.html

Java: resp.statusCode()
来源：http://hz.jinyuanbaomall.cn/gtceglmenz.html

Go:   resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtlcfsubnc.html

Ruby: resp.code.to_i
来源：http://hz.smart0.xyz/gtgetkhsmb.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtcxngfzom.html

[L08] 并发请求多个地址
来源：http://hz.zhengqikj.top/gtqfhugqqs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtxhryamdj.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtuhmctwrd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtlgcdtcdh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtbgrciybp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtejdwelkv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtqvdcilsi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtbpljyjcf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.bjfxy.top/gtqzndgcbp.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkahkcnxw.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtjesweodj.html

================================================================================
来源：http://hz.gogol.net.cn/gtctkwcqvj.html

[M01] 读取命令行参数
来源：http://hz.gzhubu.top/gtuuwghjhc.html

Py:   sys.argv[1:]
来源：http://hz.redwolf501.top/gtlqkcasgt.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtmczrbijp.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gttuygbjgn.html

TS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtnzutytcd.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtaajszirj.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtbdhfdhez.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtcpttogjd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtqevrfwpe.html

[M02] 读取环境变量
来源：http://hz.jinghuilouyu.cn/gtfpqqflur.html

Py:   os.environ.get("HOME")
来源：http://hz.fzhhl.top/gtlhnuqusc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtussafwsi.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtajqanfaz.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtmfnqzgrj.html

Java: System.getenv("HOME")
来源：http://hz.shuidangran.top/gtthluevrr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgfzy.top/gtgtbeuabi.html

Ruby: ENV["HOME"]
来源：http://hz.daxiang520.top/gtcjoevgvm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtkacahplc.html

[M03] 执行外部命令
来源：http://hz.pengpengdd.cyou/gtthioegpe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangdashe.top/gtaehrvmdr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aibaodan.cn/gtcrzgyvan.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuanzx.com/gtrbxhtasn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtlgrmarjw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gtbvqoogrx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgfzy.top/gtbbexkuow.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hysaishi.cn/gtgajxhali.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zycfv.cn/gtcepjxijs.html


<!-- 参考信息 -->