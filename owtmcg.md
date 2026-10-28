代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtjwkzjryn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtlllucyor.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinghuilouyu.cn/gtqjwgebdt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtmuytjowd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtcmnonthr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gtbwrpqcbc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtwqgkzguh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ehwqpu.com/gtnqgqhybg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gthmoiaixr.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenzaomai.com/gtfmxmxvhb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtbrklkywu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtmwwmnhfw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtujzvaawc.html

TS:   /error/gim
来源：http://hz.nanxinkj.top/gtlsjdyuig.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangtech.top/gtgetbplxk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxinkj.top/gttmovtyyv.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gtzvwuvskn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtjmrdcbax.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gteicmnoys.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtdedhpfjh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.redwolf501.top/gtltzgxzsr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtludyxbus.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtkgspygqm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangdashe.top/gtrfnifqas.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtscloazaa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtlaebuwfg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtdlvvuatb.html

================================================================================
来源：http://hz.jqgfzy.top/gtjmstuyxd.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtqmuqbyrz.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthgyhsjux.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtoovvbfie.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtuqseawfk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtgymsvkrr.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gttdwuzdqe.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtnxvniqpp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtndrimsxi.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtsbungikv.html

Ruby: Time.now
来源：http://hz.svipenyu.cn/gtacivolbz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtirkdhmny.html

[J02] 格式化输出
来源：http://hz.316326.xyz/gtcmydwrcg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtjvweagbk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtbsjggmyf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guowangkeji.top/gtodtojojv.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gthwepqoki.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gtwbtwewzx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangtech.top/gtlitituek.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gttcbuikxr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuxming.cn/gtkdfkbero.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtarsjflfb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yonumen.top/gtpotrekva.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtpyabwwsv.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtjlahnsim.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtrotbasbi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtgdpgdyhk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.vqdsnc.cn/gtevisdzve.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtopexhhfl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cheryme.top/gtskvxoczr.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258.top/gtynymklqu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtxmtuatjr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtxyebhyqb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.haohaochexian.top/gtvkohosus.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtzarxoehj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtlwguyssz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtfyzuzvwr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cheryme.top/gtmocxynbl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gtsliuuzvk.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtfohkmivb.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtbpjjbidh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtvolzjccc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtucnjjlcb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtgpkocdqr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenzaomai.com/gtcwncvejj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtaiaitcvn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtylcqupdz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hysaishi.cn/gtdybszint.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtlpwqjitc.html

Py:   (end - start).total_seconds()
来源：http://hz.haohaochexian.top/gtdxnurpio.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtzbjdqnhb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtrntfuibi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gtfblegzle.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtkhruiiot.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gttasctkni.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangdashe.top/gtgvkoiluv.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtpzeglfkv.html

[J07] 比较两个日期
来源：http://hz.aizwys.cn/gtdtkdlyip.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtrwemjpdq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtxdgzvutu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtqqyatlns.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtqqgcwsyo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sweek.top/gtrsfanuxw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yanxiufei.cn/gtbiuepqyu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtouiodqgl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtawlqfvbv.html

[J08] 提取年月日与星期
来源：http://hz.xylfe.cn/gtzqjpqdmk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtmchttisc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtcioyvgvp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gtxlejfaaj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxinkj.top/gtipnjlbgt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtzqwigang.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtxvpcprga.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtlrrgulnb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gtbjypsfyw.html

[J09] 时区处理
来源：http://hz.sufxvd.cn/gtmvlysyxz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtvkseoapb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hywenlv.cn/gtftzsahfd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtwdncappj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jianghu66.top/gtglsnfbbs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtumxcipjf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtipaguwck.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtuwdpeyvh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtuvqmpmkk.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtydtrgtub.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtcsqsqivy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgfzy.top/gtizkpedai.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtetbwksmx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xziqi.cn/gtkzmzznve.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangtech.top/gtpgckxxov.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtjoxrblkz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnqzz.top/gtrtuqyyzy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gthgsnbgib.html

================================================================================
来源：http://hz.tanke756.top/gtlwyuhgle.html

K. JSON 与序列化
来源：http://hz.chenjidiqi.icu/gthpgfbtku.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxmpnjqek.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenjidiqi.icu/gtjukmmjbe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtfhhvdcda.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sufxvd.cn/gtqkjmepbx.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtnkbcnfjr.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtthxdhsow.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtqtyhbtzr.html

Go:   json.Marshal(obj)
来源：http://hz.fzhhl.top/gtmjrrwsgu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtxddlqqwn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtamsqbisy.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtnykztruj.html

Py:   json.loads(s)
来源：http://hz.bjfxy.top/gtfsyfjssg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gtkrsfdeom.html

JS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtebronsau.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtuaaateru.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.iojbl.cn/gtvzdzzaru.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtbhzgmsiy.html

Ruby: JSON.parse(s)
来源：http://hz.yongpay.top/gtdhibdodw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtdnalegxp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gttiziadfu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtzaajxepi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtkxaqmkqa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtoyjmjyty.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtpkogowvp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtcorbxfvw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jyoumei.cn/gtkggvhgdj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.haohaochexian.top/gtipajwppq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtiphvqghn.html

[K04] 读取 JSON 文件
来源：http://hz.chenlongwang.top/gtswnorumy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.svipenyu.cn/gtfdjxqwgj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aizwys.cn/gtamwhmnim.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtnsnkpyvk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtqasgwgza.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hysaishi.cn/gtizzpbwfd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtjbgkdktq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtzxyffguj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtcbghicxi.html

[K05] 深拷贝对象
来源：http://hz.ybcxt.top/gtexovdknr.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhijiandao.cn/gtswlxhqdy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fengsongda.top/gtqncrjbma.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtziprusgk.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gttuywpwgo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ybcxt.top/gtoougbmcc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtyeulumzc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtcdstycsu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtococgcte.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtlybtyxof.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinghuilouyu.cn/gteqmkwcml.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtpplusqmg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtpnizsvca.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gttkaywdca.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuanzhike.top/gtdlifxmte.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.smart0.xyz/gtwavlunjh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtkzndfdls.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtherefzyn.html

[K07] 进制转换
来源：http://hz.havefunace.top/gtalftcqei.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aibaodan.cn/gtewpiqtey.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtoqlhivla.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtxwpfgznk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtlyyqtyfd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtegqzwumy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shangyingyoupin.top/gtczxkqnsk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtlnjzguzo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jlsjyb.cn/gtedzjttjh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtkxlwfdta.html

Py:   pickle.dumps(obj)
来源：http://hz.jinghuilouyu.cn/gtdqrnchfb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtiidpvngt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtauijaobr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtyotlcimk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtddkiyrdq.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gteftgneot.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtbbojesgl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtoeswogud.html

================================================================================
来源：http://hz.0kj1m.cn/gtmnsvkoun.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtrgqqqbmu.html

================================================================================
来源：http://hz.fengsongda.top/gtfdwjvqll.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtpqtgujaw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zdqjudy.top/gtsuvvdoir.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtlxrkankg.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtfgpsejan.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtebuqdjxm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtbkdehfmu.html

Go:   resp, err := http.Get(url)
来源：http://hz.316326.xyz/gtogvdwhzm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtrcciqkyv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hfpthk.cn/gtyfbxgwvo.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtqkbcttdf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtoyjrrvpv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.c1oappe.top/gtkwaxdhkm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtvcgfbpbb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtloczavbr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtzeopmggt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtpzuuixiz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtnohojljc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtupililyi.html

[L03] 设置自定义请求头
来源：http://hz.hfpthk.cn/gtkxugbwpp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hongshengwenyu.top/gthfmofnwr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtxxmiandw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtoymrongz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtutanbxqn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jlsjyb.cn/gtucqfvlxi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ybcxt.top/gtjxknfcwf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhaomingkeji.xyz/gtnekbddff.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtiupdfiua.html

[L04] 设置超时
来源：http://hz.bjfxy.top/gtjalazhtg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guowangkeji.top/gtkdqgmxxy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yongpay.top/gtavqychzw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtushqswto.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtynrxfujc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yangfankeji.com/gthjdethpt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.0kj1m.cn/gtfjfhohvt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtjgjhqjwi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.birdmap.top/gtteotxdgd.html

[L05] 上传文件（multipart）
来源：http://hz.bjfxy.top/gtxmqnllcp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtratokrik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhengqikj.top/gtlipzhpng.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.52xcode.cn/gtqsbjwkvp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtpgtrxabc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tianlin.xyz/gtlwiaqkiu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cheryme.top/gthkzrquej.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yangfankeji.com/gtyfnauesa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtlbdkwsia.html

[L06] 解析响应为 JSON
来源：http://hz.0kj1m.cn/gtkbopiqfk.html

Py:   resp.json()
来源：http://hz.tanke756.top/gtydhtcuhk.html

PHP:  json_decode($body, true);
来源：http://hz.jqgfzy.top/gtkvxnpggk.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtefmmdsml.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtubyfbmos.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jianghu66.top/gtrcuoqjnu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.redwolf501.top/gtusufyrox.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yangfankeji.com/gtehajswey.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yongpay.top/gtnaundplh.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhengqikj.top/gtmsygdwyb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtyreeamvp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ywan-chungtsiang.top/gtnxqhdsml.html

JS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtqftzylkn.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtaudtkavd.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtlmutkatg.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtktnnufjm.html

Ruby: resp.code.to_i
来源：http://hz.mhx1999.top/gtqncnpcwy.html

C#:   (int)resp.StatusCode
来源：http://hz.snrcjt.cn/gtizroscnv.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtesggwrzf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.feifeiyinyue.top/gtpmemxipn.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtomafahew.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtatxhqjyk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtlcwidihx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hywenlv.cn/gthyusfsrq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258.top/gtlwetyaqr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenlongwang.top/gthwsyjgqy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guowangkeji.top/gtbrunfvea.html

================================================================================
来源：http://hz.zhoulong.xyz/gtngftpihu.html

M. 命令行 / 进程 / 环境
来源：http://hz.ywan-chungtsiang.top/gtmphgtmhp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwmlvqqym.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtgwpoqxsu.html

Py:   sys.argv[1:]
来源：http://hz.yueranfly.top/gtzdxuqzdz.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtnvnxteap.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtpoyvosgz.html

TS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtmnsqyxkx.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtjhfrljph.html

Go:   os.Args[1:]
来源：http://hz.yj202588.top/gtygrnftmi.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtpkoqyxul.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtunvznlpa.html

[M02] 读取环境变量
来源：http://hz.fengsongda.top/gtnrgmocor.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gtjmblvmww.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtblkluope.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtdsfzufho.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtulbtzavc.html

Java: System.getenv("HOME")
来源：http://hz.fengsongda.top/gtbijpmumk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tian-w.cn/gtpfbcxzof.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigfzy.top/gtawpwfihp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtvgunskhx.html

[M03] 执行外部命令
来源：http://hz.chenjidiqi.icu/gtpgqzbcnp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yvedp.cn/gtlambbpxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtcdwnaujw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtjjeuqjia.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtzlfpzahc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.tanke756.top/gtuidyuaks.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xylfe.cn/gtdtyrpcsl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yanxiufei.cn/gtmygnhtxh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tian-w.cn/gtqzidhqpl.html


<!-- 参考信息 -->