代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtfecrkrjg.html

[I03] 提取捕获分组
来源：http://hz.ehwqpu.com/gthjyysesc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daxiang520.top/gtdnhrrxnv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cqqwz.cn/gtbzmxuxlt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hongshengwenyu.top/gtapkghwlc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtqmaecdue.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtuwgguamp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.andypj.xyz/gtrfbghfrb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtmvmroklo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtvmdlnymd.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gtktnjuqls.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haohaochexian.top/gtvphyphvp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtxcxiqnkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtsmgtugrx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtjcnyvlvc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtyeqypuie.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gzhubu.top/gtypgqyoli.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guannengcc.top/gtnxhncyuy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.316326.xyz/gtnftzctjs.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtlrjnriyr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangdashe.top/gtmtcrgmzk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtekefoahw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gthnccrmli.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtrtjfrlzc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daria6918.cn/gtnmuqvvvi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtsoffjfqo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtpsvldybx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yangfankeji.com/gtpbhemuoh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtrafrqkuk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtxlvowlio.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gthcynhbjs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtoyicsbko.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.birdmap.top/gtunwqttxb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtrfnnfjei.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtywsdkbhi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenzaomai.com/gtdfmlzorx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtjqcjsdgs.html

[I07] 忽略大小写与多行模式
来源：http://hz.yonumen.top/gtwqsdlsph.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtecrvdjli.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtvlczzwrs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pengpengdd.cyou/gtglmxoiep.html

TS:   /error/gim
来源：http://hz.daxiang520.top/gtglfltadl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtlfakvtei.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zycfv.cn/gtclloqmuk.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtkfvxxvdc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.andypj.xyz/gtjlwhvhir.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtzyencpoc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtzpioheyj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gtbdbjipgq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtrrsbwbaz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtefkdyhji.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtgzjyiaxq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtxicvljmy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtidrltcdo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtpzlwwyol.html

================================================================================
来源：http://hz.aizwys.cn/gtwgflyslx.html

J. 日期与时间
来源：http://hz.yj202588.top/gtixpmoumn.html

================================================================================
来源：http://hz.guowangkeji.top/gtghabaagt.html

[J01] 获取当前时间
来源：http://hz.xuetiantiany.cn/gtmbqfubxe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtnxdwkfxf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtvkmnyhjo.html

JS:   new Date();  Date.now()
来源：http://hz.nanxuanxn.top/gtpqveehxd.html

TS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtuqcatemz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtdxxsurfc.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtmwwexttc.html

Ruby: Time.now
来源：http://hz.yuxming.cn/gtowzswbja.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtoamnjfsd.html

[J02] 格式化输出
来源：http://hz.feifeiyinyue.top/gtovpmwlsc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtjzeaiydi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtikktcdwp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hfpthk.cn/gtihnjjdta.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtnkunduat.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gticiijexf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtymnrexhg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtdshujvje.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hongshengwenyu.top/gtmtrgovqk.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtqtpizprr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gtcarczwor.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtrrhkvvvf.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtzqjdofjw.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtcqhddlqr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtvoubuauf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtzchzekvy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtmadhoohi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtggllxexj.html

[J04] 时间戳与日期互转
来源：http://hz.hongshengwenyu.top/gtdmqoprpi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtevfwnley.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtheroepmt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtldqjwmud.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pycfn.com/gtoukvcfgg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtajojvvao.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.havefunace.top/gtngobpyot.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtmjrzkpzv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guannengcc.top/gtvnmlbtem.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtmynctisi.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtvnbjufal.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxuanxn.top/gtwtvfhuuv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtjnuvexuw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtrdtfeekz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnxiangtu.top/gtpfsjryfx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigufen.top/gtijnxnsvi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtzsockucn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtezvphxhz.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtsdiuxyvg.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtdnegrqft.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtcnsroubr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtmgxsbdwt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cucudq.cn/gtqzfxmuju.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtgifwhalt.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtrvlsjkgf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtodgadmho.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtlznbghhu.html

[J07] 比较两个日期
来源：http://hz.pycfn.com/gtuxkgjnzu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtxtjlaauc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gtxnzulxsf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtmykyogvy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtngdabngz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yueranfly.top/gtmukjfsbb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daria6918.cn/gtogmcabte.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtrfzgktoq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtskrtuqjj.html

[J08] 提取年月日与星期
来源：http://hz.hnxiangtu.top/gtsrcwhksf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtsjdzddld.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtokyegyis.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangkeji.top/gthjhhzcvr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgfzy.top/gtjvhuwgke.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtcdirknfn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtohtiyuon.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtcvhwiaom.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtusyokkai.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtpgiqteqc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtfccyzvtp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtieejitap.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtjsezjico.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtmwlgxron.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtthvgehuh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gtyqkbsqsl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.0kj1m.cn/gtzwxjgjpt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtuockkusr.html

[J10] 取今天 / 本月第一天
来源：http://hz.shanyushiyangkeji.top/gtbvtnrmqp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtmlksixnn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtcdprcrlu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daria6918.cn/gtoxfiicrg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gtqrgmrhzy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gttcyryhbz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guowangkeji.top/gtphjjonwt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtvfqbighz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtuljvavty.html

================================================================================
来源：http://hz.cheryme.top/gtrrgfnsbx.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtehjanxbo.html

================================================================================
来源：http://hz.redwolf501.top/gtjwhawxvv.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtdqftqacd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtmjzlajqj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtlltsesqb.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gthoqwrkma.html

TS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtqdbbqfza.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ehwqpu.com/gtgyrdonji.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtqhxcnjud.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxuanxn.top/gtcwvecysz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgfzy.top/gtshpvulml.html

[K02] JSON 字符串转对象
来源：http://hz.shzxlz.cn/gtqciwdaos.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtpphojnye.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhengqikj.top/gtvphuvuzf.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtmzvwwlsy.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gttztmmblj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtvjioiads.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtivvqhqzz.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtewxgcgxr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jiagoushi.top/gtzeviitkc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtyvjthrls.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtkifbdlwh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtopdxvhcv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtgfreptph.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtvpecrztn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.haohaochexian.top/gtmtxhyose.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtdpkmeoym.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtzwitbyyj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtyghczbsz.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtvtsyqvgz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sweek.top/gtkwlqjbuh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtzdmqxjvw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtlmjxjocv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtwmemkanb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtnasjvekp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtfyjbkqzx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gteaplgkph.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtucxeevtz.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtpfzpizol.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinghuilouyu.cn/gtwvnpbbfb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jlsjyb.cn/gtchkwracf.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtmvvefxyn.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtiwmquaul.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gtlbeocqss.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtzenmearx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenzaomai.com/gtpntoqnwv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.quarkkingdee.top/gtjifdgkpn.html

[K06] 解析 URL 查询串
来源：http://hz.tianlin.xyz/gthipbxezr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtwoawecso.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtwstdrqru.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtjoriggaj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtobtdtzvy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gttlydrmaf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtcmhcrdtw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtphboyigc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtrgbazlec.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtnamincyw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yanxiufei.cn/gtwkzrxojb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gtlsrjdbsx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtlzodlhjf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtmghqcfle.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daxiang520.top/gttaoquaaf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhixingplan.top/gtbcvhxjwj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.birdmap.top/gtpcxlnkie.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sysykeji.top/gtervardic.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydzc1.top/gtfctugkpq.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtdbekufqm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtbmwfxwhs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtecftbiuk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtxuygnuaf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtfwnjzdbs.html

Go:   encoding/gob
来源：http://hz.svipenyu.cn/gtlmirfata.html

Ruby: Marshal.dump(obj)
来源：http://hz.mhx1999.top/gtqlzjywcj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yongpay.top/gtxdzouodz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsctvtsfb.html

L. 网络请求
来源：http://hz.cheryme.top/gtsxotylok.html

================================================================================
来源：http://hz.0kj1m.cn/gtplvyylwg.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtucpgqdal.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtpnafbyvg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtakndlaac.html

JS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtndyrmdrf.html

TS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtuogfmani.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cheryme.top/gtjjaslruz.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtvtgofdzk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtlvzbtlqh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gteewvhjtp.html

[L02] 发送 POST JSON
来源：http://hz.zycfv.cn/gtbonafhri.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtbnuenbih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtzyudywdg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtqfktszyu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gttfjprldl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtgzepvxqk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtlklghvpb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenzaomai.com/gtymxzloza.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guowangkeji.top/gtyoysycym.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtsuiupyoa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtrllhbndy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangtech.top/gtkvivvtri.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtisfbqhcv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gttcywnffz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigufen.top/gtwmhjhucg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtqzqpudar.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gthjlqvjrm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtxsxobxau.html

[L04] 设置超时
来源：http://hz.cheryme.top/gtzuqczoxu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daxiang520.top/gtwbxluuoi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtatqtzfeh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtwqjsrfit.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtmadbubru.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxuanxn.top/gtcryzjgnj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtnbsaqzap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tianlin.xyz/gtwmduwcwi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtiibjkzam.html

[L05] 上传文件（multipart）
来源：http://hz.9152youxi.cn/gtbmmkfslu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.9152youxi.cn/gtfwzkflsf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtcelttatt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtvdiqfwns.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtpddbxqqn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.bjfxy.top/gtnjphbtst.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtdfwgvwrp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jiagoushi.top/gtvukjshok.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.vqdsnc.cn/gtleirwjrt.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtxnzyaypj.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gtkbhvssdb.html

PHP:  json_decode($body, true);
来源：http://hz.ywan-chungtsiang.top/gtwsikhwwk.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtugzhnyto.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtcoiwpzxk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtfrdnrwdd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenzaomai.com/gtxzepbqur.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sxryk.cn/gteenvnmfv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.52xcode.cn/gtclzvgflv.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtjcohdlyo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtzvemmyyf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fzhhl.top/gtcpbrstad.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gthlckkcco.html

TS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtalpaczci.html

Java: resp.statusCode()
来源：http://hz.yuanzhike.top/gtmwvhjfqy.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtnohqsbks.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gtclaahfqw.html

C#:   (int)resp.StatusCode
来源：http://hz.cucudq.cn/gtfqckrjlo.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gtfnfjmvyd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gteklpvulp.html

PHP:  curl_multi_init() 系列
来源：http://hz.quarkkingdee.top/gtmywbxdlk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtbjmhegse.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gthpepvtzj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yueranfly.top/gtlqqxunpe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shuidangran.top/gtjjmxebtc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shzxlz.cn/gtvncmtjze.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.mhx1999.top/gtwlvahkzb.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcktoqrhu.html

M. 命令行 / 进程 / 环境
来源：http://hz.shuidangran.top/gtctbbtbfh.html


<!-- 参考信息 -->