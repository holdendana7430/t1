代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gtbhlghoik.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtyqbwrwmu.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtynlzgauk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daria6918.cn/gtupchttso.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cdnleiting.top/gtutjtnews.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtsuoqowzj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtsstgqjvn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daria6918.cn/gtkvzphqyl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtbyljcnrz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jiagoushi.top/gtmqsdnkqf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtajblfkwx.html

[I05] 按正则拆分
来源：http://hz.meibo888.top/gthncsiebj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtlobacefp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgfzy.top/gtskddtnim.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtttnofxpv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtayjcclqq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhongyouzk.top/gtbqsbatrl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtsczghezo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtflpkmgre.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.dashuyun.cn/gtrvfphafh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydzc1.top/gtkvrtuwvx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtsrpkoeuf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ivvv.top/gtpmshyxmi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtwbgshmqw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtnfomxdzc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hysaishi.cn/gthmvcwxbp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtohmqgyps.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtpexkadgp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtowsxjerz.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtnodycmvp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangshuangyany.cn/gtzwvyjqzq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtnnirftnn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtwpfziowy.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtshblljgl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtukifqkzf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gthleaoosc.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtitlexkdb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtinhsxyut.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtqmbyuwlr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xziqi.cn/gtpjpbgxha.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shzxlz.cn/gtmxymtyee.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtlbyphoog.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gtqdrxymsr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtakoxhobj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jianghu66.top/gtuodbvsvg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yangfankeji.com/gtsttfskuc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtzjizyjtc.html

================================================================================
来源：http://hz.dashuyun.cn/gtwlqzkfpj.html

J. 日期与时间
来源：http://hz.quarkkingdee.top/gtexolcqqx.html

================================================================================
来源：http://hz.316326.xyz/gtvsnvzcem.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtzetfdikj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtnjjxkuft.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtzvtpeier.html

JS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtqaeojpbh.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gttcmxigxm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtunhcctnn.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtjuxajpsu.html

Ruby: Time.now
来源：http://hz.ivvv.top/gthovqimqy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dianchejie.cn/gtdsmjgttx.html

[J02] 格式化输出
来源：http://hz.gzhubu.top/gtujgexneu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtbyffyjrf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gthrtknymg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shuidangran.top/gtkrjaxgjn.html

TS:   d.toISOString()
来源：http://hz.sxryk.cn/gtvchsqpod.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhaomingkeji.xyz/gthqrhqvrk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daria6918.cn/gteuaqybiy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtwktosere.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gtwghygkkp.html

[J03] 字符串解析为日期
来源：http://hz.gzhubu.top/gtsqktdfvx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhixingplan.top/gtyxrmktgc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenzaomai.com/gtzjgrwkqy.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtvlhbljyp.html

TS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtthfcbbnk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtmziltozv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtngyzrqes.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtgscjwpfm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtwryfofxv.html

[J04] 时间戳与日期互转
来源：http://hz.daria6918.cn/gtnaaebvot.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtsquybpbt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gtfgbtkrsc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gttojadwug.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtiicodsnp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtnoxmgkxb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cheryme.top/gtwaudwvqw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gtycxihgxq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gtagnstaqw.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhengqikj.top/gtvytmwwgu.html

Py:   now + timedelta(days=7)
来源：http://hz.pycfn.com/gtzxbyetsu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnxiangtu.top/gtaxrfbgzq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtdgvhepui.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtxzlthrsf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgfzy.top/gtdjdkwesm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.mhx1999.top/gtthqmeyvg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ppjwa.cn/gtyhsrnicw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtqingvwfv.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtlwbcpbmm.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigufen.top/gtxkkpwcqx.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtukdldspj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtpfcjtmls.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tian-w.cn/gthmmxzeya.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhoulong.xyz/gtjgynbrgw.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtezjuoino.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gaohongyu789.top/gtcorwsdkb.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtkrlobjhk.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtpudqpyde.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtwqcpwmyj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dianchejie.cn/gtqyqbxbap.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtnyvnijxt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtyqegtzdn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtyhiwubry.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtiojvuhfs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtatanumgi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtvrviosyc.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtahaialzo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dianchejie.cn/gtvwwpmfxo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtyrrcqxfw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangtech.top/gtztptcbxk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tanke756.top/gtgwtoutbu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtyxrfxnbb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtkrqfblmp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtkowhggkn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtjonjuzep.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gttzozwrup.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gtlxztwsxg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gtvoyoalmm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtthwqacwy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtqmvpbfvt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.c1oappe.top/gtroyyoens.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtinwpgjif.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gthllmypfl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gtskloytpk.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtrgximiko.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jlsjyb.cn/gtnuktwacb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtawhfeque.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fzhhl.top/gtqtqkzbsx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtdniqcvll.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtfxtoghnt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hywenlv.cn/gtnmjjkrbv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtcaojbqht.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yonumen.top/gtgzzdflyr.html

================================================================================
来源：http://hz.sufxvd.cn/gtxjrbzttm.html

K. JSON 与序列化
来源：http://hz.zhijiandao.cn/gtjcyoyzlp.html

================================================================================
来源：http://hz.yj20258.top/gtecuazqec.html

[K01] 对象转 JSON 字符串
来源：http://hz.aibaodan.cn/gtxfsqqhgp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtkxyopfks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtuuckdprl.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtpdthjzar.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtokijcxof.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtpkjekscd.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtzxadkuvb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgufenzy.top/gtsvlcqfno.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gticbuwgdf.html

[K02] JSON 字符串转对象
来源：http://hz.haohaochexian.top/gtjrmubnob.html

Py:   json.loads(s)
来源：http://hz.zhengqikj.top/gtjdkkszoc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dianchejie.cn/gtrzzqstbf.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtedxkjqvv.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtxliuqmlz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtgwjlqcpk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gtzyyeoomu.html

Ruby: JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtexaslcdi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtuhmqtnip.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ehwqpu.com/gtcuserhud.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtwazkqxol.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtjotkweuj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtdfbodqrx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtwdiurxeh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jianghu66.top/gtaxdhtvmp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dashuyun.cn/gtlaqkreng.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtejyzlhze.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.redwolf501.top/gtegoojyqy.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtcneqzcli.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tian-w.cn/gtcruaayme.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtfikfqhix.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtmuopvglt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtbcfmiphv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gtmejruyuv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgfzy.top/gtvyottsbm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtdrjhymps.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtpjknpokj.html

[K05] 深拷贝对象
来源：http://hz.aizwys.cn/gtrnxjzvko.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtrgrfzuhu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnxiangtu.top/gtujfdpija.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtnpwtgula.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtqshjiizw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxuanxn.top/gtuomfbbpp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangdashe.top/gtqvkqaman.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangdashe.top/gtyikzbeih.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangshuangyany.cn/gtlarhcibv.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtbalxmopx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gthfklhnrg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hammf.cn/gtrmlyzlme.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtjqoyidos.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtvkuedsmc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtuffkiomj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sufxvd.cn/gtazzfwlwl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtgzklqqhy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.iojbl.cn/gtonfyxxcg.html

[K07] 进制转换
来源：http://hz.ybcxt.top/gthjzataug.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuxming.cn/gtdfuwhlxr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuanzx.com/gtdqcznvsg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtdxhrwpyd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtzrcvpoma.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtghmxtpmk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtxebfvrnt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtapritnoc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gthhajfeix.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guowangkeji.top/gtjwmsloub.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gthuglzsrp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtafpuidxv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtndgyqaan.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtveesgsqr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtvliaqagt.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gthdpleprh.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtcxgforli.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtzevvxtxw.html

================================================================================
来源：http://hz.fzhhl.top/gtgenbmgvn.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtcpnexklb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtaecngzyi.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gthlfgvnhd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtssbcjouu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtuyzzvfxb.html

JS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtwzodqwla.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtunhawunx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ybcxt.top/gtvvomrrto.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuxming.cn/gtofoqpmhk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtpxedllts.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhengqikj.top/gtgkxsxqrz.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtrinjjrly.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.9152youxi.cn/gtopmfaput.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gthovkfudt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtfczzgybc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtqbeitudu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtwzpzhjcc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtgpxkrjth.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ivvv.top/gtdqkhaall.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtnnzmnkiz.html

[L03] 设置自定义请求头
来源：http://hz.yanxiufei.cn/gthwcsbott.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xziqi.cn/gtaxxgesco.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.bjfxy.top/gtjxmzefgd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtauuhibhw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtlcxnrtcu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtnjlyyqkl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtaagzljxy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hongshengwenyu.top/gtanobcuvw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtozxiodqp.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtwhknoanp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.mhx1999.top/gtdlxpegoj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ehwqpu.com/gtmqgainmw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtfsulktqc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtrozfpret.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuxming.cn/gthzjkfvca.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtegpcmsap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtbqidackr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gtzijulvqy.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gtziqevbzf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jiagoushi.top/gtibhrgxwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenzaomai.com/gtkwncqarv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gttcpxqwjs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtoryxbypl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ppjwa.cn/gtdbaigucg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.316326.xyz/gtoisstxer.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtxaijfrbl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigfzy.top/gtnhmgmere.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtlllpqozy.html

Py:   resp.json()
来源：http://hz.zhongyouzk.top/gtwnkcpkyb.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtexcmvquh.html

JS:   await resp.json()
来源：http://hz.ydzc1.top/gthydrmpsn.html

TS:   await resp.json()
来源：http://hz.smart0.xyz/gtenlcdwwg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtubimwnro.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gtxeedvgmm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cashguo.top/gtgdaiucof.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenzaomai.com/gtsnnzeyuz.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtrwuwuuwk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hammf.cn/gtxfmfdlar.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gogol.net.cn/gtamiquxuf.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtzgbhzcxd.html

TS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtlyjquann.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtbacxdvhw.html

Go:   resp.StatusCode
来源：http://hz.jinyuanbaomall.cn/gtgoxdiume.html

Ruby: resp.code.to_i
来源：http://hz.guowangkeji.top/gtdnyxqrzv.html

C#:   (int)resp.StatusCode
来源：http://hz.316326.xyz/gtbjxmnhiq.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtqikxfomc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tanke756.top/gtntxbnzxt.html

PHP:  curl_multi_init() 系列
来源：http://hz.shuidangran.top/gtznvxcjpe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtkfjmkuog.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtbxqarpbx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigfzy.top/gtnlbszvqv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sufxvd.cn/gtivthexxp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ybcxt.top/gtgexvzhgb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtaruikotb.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtarjsbiyt.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gtxumnlutu.html

================================================================================
来源：http://hz.nanxinkj.top/gtdkjlzgdr.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtvsjmizig.html

Py:   sys.argv[1:]
来源：http://hz.hnxiangtu.top/gtitfxzlof.html

PHP:  $argv;  $argc;
来源：http://hz.yangfankeji.com/gtmepsawde.html

JS:   process.argv.slice(2)
来源：http://hz.ywan-chungtsiang.top/gtsjowlpmh.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtzvaxtfcu.html

Java: args 数组（main 方法参数）
来源：http://hz.guannengcc.top/gtyhfzbktv.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtekbajsff.html


<!-- 参考信息 -->