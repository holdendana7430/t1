代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtgwhkkdmv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gtriovzzzs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtpdxktqga.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ybcxt.top/gtpzwdjadb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gtttwztrbb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gthehkenly.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtmcmkskzs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtslzdrpkk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtylbmohej.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gttasbywqw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gogol.net.cn/gtjhxfvrzz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtaicfpsyy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtyprsogwo.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gtvkcxfbtn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.bjfxy.top/gtfblkphur.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtfolcnioy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yvedp.cn/gtauzzaqty.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtjlvhmbnw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtbcnlljzp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhoulong.xyz/gtqflkhaoe.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtatfwrpaw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cashguo.top/gtoatpvfti.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtyzarabun.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtyxraygyo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtyihiaziu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtacqdfnrm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtiynlnyfu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.redwolf501.top/gtlibjgent.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnxiangtu.top/gtxnemcezj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dashuyun.cn/gtuhxoisov.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtpzlfnknp.html

================================================================================
来源：http://hz.ydjk.org.cn/gtavesuegk.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtwmegqwah.html

================================================================================
来源：http://hz.meibo888.top/gtymrxgzjk.html

[J01] 获取当前时间
来源：http://hz.0kj1m.cn/gtfijrtbom.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yonumen.top/gtfsecnrjc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtfjijorni.html

JS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gttzgvhgll.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtmzjyeeln.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuxming.cn/gtvmiqxhtl.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtfpsvekxv.html

Ruby: Time.now
来源：http://hz.c1oappe.top/gtzxubpxxq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tian-w.cn/gtjriddwyn.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtdozclpat.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtvwxaabck.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sysykeji.top/gtabbrplhr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtfavafbzt.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtiwdwshwh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gttuqywhzb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtkthrvlkt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtkbojlcas.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gtgrluflte.html

[J03] 字符串解析为日期
来源：http://hz.wangdashe.top/gtllmwsezd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gtnderxxkt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jiagoushi.top/gtdvnqhryk.html

JS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtnxexcybt.html

TS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtsyvwgjsl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnxiangtu.top/gtcivpzkhy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtqzqfufsr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtohsmyepa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tanke756.top/gtedxretek.html

[J04] 时间戳与日期互转
来源：http://hz.xinyue.icu/gtxyaljakk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gtvjodunsa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtnmxegduk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jianghu66.top/gtvgmgscet.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ybcxt.top/gtqtbrplgs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gtpxwjzaqe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtidmugcdc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtwhcagcjy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gtkahcqwjs.html

[J05] 时间加减（加 7 天）
来源：http://hz.kuanghao11.cn/gtlqvuinrq.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtqnmtwfky.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuxming.cn/gtqxcapotb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtrumzbtgw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtpxznhwdj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jlsjyb.cn/gtfgvagcuj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yueranfly.top/gtbodvhqdl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.mhx1999.top/gtdpykeliq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtozgxcxmr.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gtbjsiebvv.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtvcpuurio.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtrscvdoti.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fzhhl.top/gtarlrwohp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtpzlzbfmw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtambvtcau.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuanzx.com/gtnpavzzye.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtcvolkvjm.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtwttahnat.html

[J07] 比较两个日期
来源：http://hz.guowangkeji.top/gtdfxkbqaj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtvzadcwex.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtxvtgrqmz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtfwommynn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtejbuygez.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aizwys.cn/gtjvreoowd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtywflwhrz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtnnbxghdd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtokkgclux.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtwhgzriob.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtogmwjify.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenlongwang.top/gtxgdcdtst.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtbwqqutvf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.iojbl.cn/gttxpkpfpv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhaomingkeji.xyz/gtxkcqtlxo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtgfwbqlyc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtqieakipw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jiagoushi.top/gtdzimlmnt.html

[J09] 时区处理
来源：http://hz.xuanzx.com/gthfipidif.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtdtvpzzzr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxinkj.top/gttumofuty.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtvrzhurpy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtggdbdedz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gtkwfdmzdr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgufenzy.top/gtisoeaskv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtlrgcovju.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtlzuvyros.html

[J10] 取今天 / 本月第一天
来源：http://hz.dashuyun.cn/gtqpdneset.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtxuzvixry.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtzwioywfp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtqtexscpi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yvedp.cn/gttqnhoeun.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangtech.top/gtqobxzbve.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nwbrower.top/gtjyokmefj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtpqqtojgo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gaohongyu789.top/gtzxwtgpwa.html

================================================================================
来源：http://hz.havefunace.top/gtnxhqrjyb.html

K. JSON 与序列化
来源：http://hz.zhaomingkeji.xyz/gtwyvvnwzt.html

================================================================================
来源：http://hz.chenlongwang.top/gtthweypjq.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinghuilouyu.cn/gtuhtwlbfu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtxatmmfrf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gteqfqgmdw.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtsaalrfwi.html

TS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtwxkndaie.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgufenzy.top/gtaspxmolt.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtffwupjpl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtxnqokrgi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zycfv.cn/gthzxjksuh.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtphstqrpv.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtgdktfndb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cashguo.top/gtpakvflst.html

JS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtsksqnzhv.html

TS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gttzeormck.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtaejawuvh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtmookbyzi.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gteocoukoz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnqzz.top/gtzsmhrlhm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gtthnnjdbn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtyfkmgfkc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtfjrqpvhm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.haohaochexian.top/gtsukenkvb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtdulgdhom.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gtcqsbupoa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtfcvipubr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.c1oappe.top/gtkpvdaykq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gtdjjmqveg.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtpyfuekkw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinghuilouyu.cn/gtjravofqh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtyiselbbk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtfbhlqilh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtspnlnkyx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtvbcddmco.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtqjyojngu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtgceljacw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtdcnomxkl.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gtojdogxyq.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gthadpdcwk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sufxvd.cn/gtcwtfccuk.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gttuqecurw.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtstngqunh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtghakohor.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtvoemzvxi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtzyfvgqso.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gzhubu.top/gtsxdnsufb.html

[K06] 解析 URL 查询串
来源：http://hz.xingfuxueyuan.xyz/gtmvkulpdt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtybovewzt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jlsjyb.cn/gtpgplnbbo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtbgxhdjzi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtyikqftgx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtdyflfnft.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtgswuhvvl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nwbrower.top/gtbkaefefs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.snrcjt.cn/gtbjyecmcd.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtuaahjzlg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gtbkiehsns.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gtxjsjqqai.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtavnhfdxr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtliwpmnia.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gthcrbfjni.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gtvvdihbxw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtkffwsklz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xinyue.icu/gtgitenxzl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtlhudmmcg.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtsyikozxd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtlvarygoh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gteedszwfn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gterafjcft.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tian-w.cn/gtfpqodsdd.html

Go:   encoding/gob
来源：http://hz.tanke756.top/gtrilmutlo.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtnxcatxig.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gtotxzxnmk.html

================================================================================
来源：http://hz.ydzc1.top/gttbaxeghl.html

L. 网络请求
来源：http://hz.yj202588.top/gtvcoxbasn.html

================================================================================
来源：http://hz.mhx1999.top/gtgethzzve.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtxxtcecxl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gthmkyukyt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtsiovfsbo.html

JS:   await fetch(url)
来源：http://hz.vqdsnc.cn/gtkqxsjrod.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtfbuiwreg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dianchejie.cn/gtpjjbkurp.html

Go:   resp, err := http.Get(url)
来源：http://hz.daxiang520.top/gtyhrouutm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtvyjgzqgb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daxiang520.top/gtvqdyycbh.html

[L02] 发送 POST JSON
来源：http://hz.pycfn.com/gtnzfbobyi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtuizozcrd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtjttxrval.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtdbqiifih.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtpagiufpn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hywenlv.cn/gtvxqickjr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtbmbjqona.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.svipenyu.cn/gtzkvzifol.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtrnldsnka.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtrknzpglu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhiwuduotai.top/gtnzjztonz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.havefunace.top/gtmibkpchk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtbavqhhyp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtefiaotif.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtsamkpudy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtldfwxupk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydzc1.top/gtfwgvoktb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtoloydjwk.html

[L04] 设置超时
来源：http://hz.kuanghao11.cn/gtmrraunxr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtzzxhagwa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtmdetxkoz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtzoqwwnrk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtgcujnrwt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tanke756.top/gtjnyvhlpq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.iojbl.cn/gtonjganbn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gtmxgtniwm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.quarkkingdee.top/gtoxmbjtgg.html

[L05] 上传文件（multipart）
来源：http://hz.tian-w.cn/gtqtccfoqq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtzopvesah.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gtaxvcxqad.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gttzjnquie.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtzddeochf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.andypj.xyz/gtmcruejto.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.mhx1999.top/gtpnotuoow.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuanzx.com/gtckgfufaz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xylfe.cn/gtsporwwrz.html

[L06] 解析响应为 JSON
来源：http://hz.zycfv.cn/gtdsusbcej.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtpfvwqwji.html

PHP:  json_decode($body, true);
来源：http://hz.mhx1999.top/gtpiouzfyd.html

JS:   await resp.json()
来源：http://hz.tanke756.top/gttjrbugkh.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtrcjxlanf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jianghu66.top/gtnuelkmix.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtkbsorrvh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zdqjudy.top/gtsqdeanie.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cashguo.top/gtxjlgssex.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangtech.top/gtidfcgils.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dashuyun.cn/gtwxcuerpk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.bjfxy.top/gttczqvrjq.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtaguhjgcb.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtzaghgkbb.html

Java: resp.statusCode()
来源：http://hz.nwbrower.top/gtpgnssgfh.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtzlfohmax.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtcquaxwsg.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgufenzy.top/gtdatacpix.html

[L08] 并发请求多个地址
来源：http://hz.zhoulong.xyz/gtervtznep.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtftvudqti.html

PHP:  curl_multi_init() 系列
来源：http://hz.cqqwz.cn/gtcqtsporj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtahbttdib.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtdqabajxo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhixingplan.top/gtgtbwhxhi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cqqwz.cn/gtxujmsydb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtldhmumfo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ehwqpu.com/gtxgkvyrgj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtyqkqlxqu.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtjovdosxx.html

================================================================================
来源：http://hz.ybcxt.top/gtuzpcrggk.html

[M01] 读取命令行参数
来源：http://hz.mhx1999.top/gthnffawoc.html

Py:   sys.argv[1:]
来源：http://hz.zhaomingkeji.xyz/gtawpajgnn.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gttgbktloq.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtidlgzjte.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtsxqguumw.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtijaibiiz.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gtawnbtdnk.html

Ruby: ARGV
来源：http://hz.ehwqpu.com/gtuvspoued.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gttdjhlbzq.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gtryyktmqc.html

Py:   os.environ.get("HOME")
来源：http://hz.pengpengdd.cyou/gtcrgdojmn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtesxvverq.html

JS:   process.env.HOME
来源：http://hz.xziqi.cn/gtngmuvejf.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtwlgstiys.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtiijcdptl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtkhhbixnj.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtigbhvvbs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hywenlv.cn/gtacdodajt.html

[M03] 执行外部命令
来源：http://hz.zdqjudy.top/gtjaackzfe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtmvalzscj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtoykweszp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gthtdmeesh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtropiorcv.html


<!-- 参考信息 -->