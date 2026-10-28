代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gzhubu.top/gtasecguzc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gthafwxpdq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtfstlxexf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxuanxn.top/gtcducpjhy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jyoumei.cn/gtebgcwnhh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtdggrabid.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gtdwolswbd.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtmvxsdmbm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.haohaochexian.top/gtlyrukocq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gogol.net.cn/gtikainebp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtmwucgqvl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtlllatron.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gzhubu.top/gtjbwnueuf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.bjfxy.top/gtkdlvuxdd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtqduswalu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.52xcode.cn/gtabmngsmu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtfcsifjft.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtylipesdr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtytgusgxr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtrxtjtipb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtitjcpgse.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guannengcc.top/gtofzijjwl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.andypj.xyz/gtuilbtqtd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuxming.cn/gtakgsdyxa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtxbtjkvsn.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtlpmiyscf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtjseguyxn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtgrmrzszq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.redwolf501.top/gtaqrbpciz.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtwoqnlqzb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtcwpceqba.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cucudq.cn/gtqolkornv.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtdwryxpti.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fengsongda.top/gtgpibgdea.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtglfkbqcu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtwucvpbfw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtkdhnadrd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtpjqyakrk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtnposmyzx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtaajwpkgh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangdashe.top/gtnkxdzqmm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuxming.cn/gtxzwqdafu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtalkmlwgn.html

================================================================================
来源：http://hz.tian-w.cn/gtseskbfyt.html

J. 日期与时间
来源：http://hz.meibo888.top/gtokabyoig.html

================================================================================
来源：http://hz.chenlongwang.top/gtgglruobr.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtwygjctiv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gzhubu.top/gtnmlvjqms.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtzeqmokuk.html

JS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gthartegmb.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtfbvujugn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cucudq.cn/gtzkiknogp.html

Go:   time.Now()
来源：http://hz.316326.xyz/gtskfuhqgm.html

Ruby: Time.now
来源：http://hz.zhengqikj.top/gtrjkjoqvr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gzhubu.top/gtfpufxrsh.html

[J02] 格式化输出
来源：http://hz.yj202588.top/gtngfjqmhc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtkzxrfzwc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtrnqnufwr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtjgyczfdr.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtvvtwupeg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtalnszeny.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenzaomai.com/gtduxrnaph.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtnnmakopm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtwwwgxtuo.html

[J03] 字符串解析为日期
来源：http://hz.havefunace.top/gtarjsktyq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gteiwecsof.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gtqbplrtud.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtaasvcvuk.html

TS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtcfhpqtwy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtmpbeakgz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtakcoqrgd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtobvsrket.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yongpay.top/gtlxmokdap.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtwlfmvwew.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangtech.top/gtirndylnh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtlefilqwt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtujfbrdbo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtlxjkjxro.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shzxlz.cn/gtvqfjrrcq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtaugdujgb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtkzdumchk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtjyuikqgk.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtqstwkzww.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtsiqspkjq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtlgagpimx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtxmxfewgm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtvmiytcjw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtrclbwoyg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gtmlycqlpe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.mhx1999.top/gtnbsoljmd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtttersurd.html

[J06] 计算两时间之差
来源：http://hz.quarkkingdee.top/gtzqlfqwyu.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258.top/gtodjbycep.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gteaicxzap.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gttacvpoda.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtqmqpvzji.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtkflpfqln.html

Go:   end.Sub(start).Hours()
来源：http://hz.yvedp.cn/gtdlsixygs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtqvbczwvd.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtzzuyayyt.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtyelocuqp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtvutyjgsy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daria6918.cn/gtcilpiotn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtpqegcqar.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtpilwxvtg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangkeji.top/gtnuingawo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cashguo.top/gtohcbrenb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtqihwytlf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtnceycbiw.html

[J08] 提取年月日与星期
来源：http://hz.sweek.top/gtjglnwgbb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gtiyfyygnl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenlongwang.top/gthohtidvb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtpxxlaeab.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtcdncdkfg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtdlmbpmvo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sysykeji.top/gtezyfhlgc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.havefunace.top/gtdndjilmc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtslhrjjgk.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtvruiznbf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jyoumei.cn/gtctrxhaby.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtwgycmynh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtdhwgynuj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtkhqtxhmm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gtsfosvcwz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtdgbhrrqw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtnuxznfni.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sxryk.cn/gtjcethpqb.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gttkvauyvr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtdzzrzrmi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gteqoyhlft.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fzhhl.top/gtfppxlnvw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gttjxqzjsb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenzaomai.com/gtdemktuwv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtsjyfbbdx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhaomingkeji.xyz/gtzsuchgdm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtqkmgnusw.html

================================================================================
来源：http://hz.birdmap.top/gtwdxntbdy.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gtibphozqt.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtlsvbyexq.html

[K01] 对象转 JSON 字符串
来源：http://hz.haohaochexian.top/gtavjgxdxy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtsvscjael.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtlquyperc.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtgmobbqsk.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtixcylvxz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtpvfhiwds.html

Go:   json.Marshal(obj)
来源：http://hz.yj202588.top/gtvrgabyjv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gtvwchxdeh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtrhaheoas.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gtmztmbfvn.html

Py:   json.loads(s)
来源：http://hz.cucudq.cn/gtgoxmhvzi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.andypj.xyz/gthukybwgf.html

JS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtvobsltez.html

TS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtszfbdvar.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daria6918.cn/gthjrcfqyo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gttuhuheok.html

Ruby: JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtasitpnyd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtzqigjttd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tian-w.cn/gturnkqrrq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtafhfgjkj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtqeeidicg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtriljaghb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtwgjsjwwu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtgpqhglvu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtunsfevea.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtskrzuxhm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtgqmlmubb.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtygwbooak.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinghuilouyu.cn/gtotixasyd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hywenlv.cn/gtetzzhlsb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtywzewelj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtayczotpf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtgehqjjrc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtahazrfak.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gtkfrdtarh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtxbhoijjh.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gttddsmgme.html

Py:   copy.deepcopy(obj)
来源：http://hz.tanke756.top/gttmuwlffz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gttikerhbv.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtfqlerfhi.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtigjoszwc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guannengcc.top/gtcdcgiwxy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtqtximlvr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtnulwvgmf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nwbrower.top/gtofugmcqy.html

[K06] 解析 URL 查询串
来源：http://hz.pycfn.com/gtfbzjtmbj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtgdtziaae.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtvdmmtksj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gthgnvbiyz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtzymzfryb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtwfdhnvcg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtlsmpgqdi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gtkubkdrhy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtypfvyunz.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtfziotvnn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtfajyxozr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yonumen.top/gtohysvbrl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtdmhuvtlx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtaruwlqhx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtclkehhcj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtrungdhnf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gtmitsxkzf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtpnzmszoe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtizpvuqno.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtgotlbkiq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gthvoburzj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtjxzzfhsi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtrmremegj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtdhnkxglo.html

Go:   encoding/gob
来源：http://hz.mhx1999.top/gtifimpujv.html

Ruby: Marshal.dump(obj)
来源：http://hz.pycfn.com/gtoxvniwcy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtuvamftju.html

================================================================================
来源：http://hz.ybcxt.top/gtdwnzpspy.html

L. 网络请求
来源：http://hz.yvedp.cn/gtqzffcqfb.html

================================================================================
来源：http://hz.dashuyun.cn/gtmdlallay.html

[L01] 发送 GET 请求
来源：http://hz.daxiang520.top/gtlgcvhzfa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.snrcjt.cn/gtzbdbtahd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtqyoemnkd.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtimqsbcpm.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gttvrkxuxr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tanke756.top/gtemdtbkkn.html

Go:   resp, err := http.Get(url)
来源：http://hz.fzhhl.top/gtatmoggwm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhengqikj.top/gtexlswziv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtgnvuodou.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtekoxlnxj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangdashe.top/gtblhretqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtpkvgknoh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtsabxpawy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtffxetipm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtpofydzdw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jlsjyb.cn/gtjsllmaca.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sweek.top/gtvycnltev.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ppjwa.cn/gtnnjmyahy.html

[L03] 设置自定义请求头
来源：http://hz.chenzaomai.com/gtctdqsqkk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gttmbfzuxk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sweek.top/gtaihdomkh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtlscryrrz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtnmybqjqc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtwxhrdeao.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtqtoxpdnd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtasjatjuq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtxrlmwapd.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtvudoahly.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zycfv.cn/gtrfijdkyd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gtpxppqrgq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtzxrappdq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtnpjkvazr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dianchejie.cn/gtxyfzoygu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtindbiotr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtghrwiznu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtxhturaff.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtslkyplkw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtpjourrdc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtfiqylcqf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtkasftwci.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtlyjqiuki.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cashguo.top/gtorquuxwm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtjyluywkh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yonumen.top/gtkbsdzqxr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtmjxpaxby.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gtnksuhzle.html

Py:   resp.json()
来源：http://hz.tianlin.xyz/gtugjnwtuz.html

PHP:  json_decode($body, true);
来源：http://hz.xylfe.cn/gtjeacccav.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtebruusfx.html

TS:   await resp.json()
来源：http://hz.yuxming.cn/gtjdiojkll.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gtwmsgbboh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gtreokcura.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtokyhbdvc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cdnleiting.top/gtwqgitbxf.html

[L07] 处理 HTTP 状态码
来源：http://hz.gzhubu.top/gtanpejiog.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sysykeji.top/gtlwbusorm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gtprtatrwe.html

JS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtigzxpoiq.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtqvsmhmbk.html

Java: resp.statusCode()
来源：http://hz.chenjidiqi.icu/gtpdovqlzc.html

Go:   resp.StatusCode
来源：http://hz.cucudq.cn/gtyqwamrgy.html

Ruby: resp.code.to_i
来源：http://hz.zhengqikj.top/gtrlkzcnqe.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtplonubzh.html

[L08] 并发请求多个地址
来源：http://hz.yj202588.top/gtmbnvmpnl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtfertnupx.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtfqdupvya.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtztotunci.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtehexmgiy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtsltirtsh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtqoaxswha.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jiagoushi.top/gthsgehzyr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtpmluyore.html

================================================================================
来源：http://hz.hammf.cn/gtxvvskbmr.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangkeji.top/gtiuqlaoel.html

================================================================================
来源：http://hz.yj20258888.top/gtbonfdukr.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtjtcbzyrh.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gtznprlxxn.html

PHP:  $argv;  $argc;
来源：http://hz.ivvv.top/gthouumaxs.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtaytvyksl.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtgatecccs.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gtjxhtilja.html

Go:   os.Args[1:]
来源：http://hz.jinqigufen.top/gtpsvkmxlt.html

Ruby: ARGV
来源：http://hz.yj202588.top/gtvgavqmdf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtylirduas.html

[M02] 读取环境变量
来源：http://hz.hywenlv.cn/gtmkhcmyai.html

Py:   os.environ.get("HOME")
来源：http://hz.shuidangran.top/gtaqlpcybw.html


<!-- 参考信息 -->