代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigufen.top/gtgmfwcqlq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtqcggswjk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtwfcstvdv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnxiangtu.top/gtzncydgpc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hfpthk.cn/gtmorbydng.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gtykxdajli.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtnhcpeowb.html

[I05] 按正则拆分
来源：http://hz.fengsongda.top/gtiwmbtkcz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtzucrflqg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shangyingyoupin.top/gtuwvakdks.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtlmyindtt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtdqvmggpn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gzhubu.top/gtfavrvgmg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gtbngxekev.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtnxbvpkrk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtszawfvba.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenlongwang.top/gtzxgxavwh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtfbbqdzli.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinghuilouyu.cn/gtmnhmpcua.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtmecpptkk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtacyzfihh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenzaomai.com/gtbakvcayo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.iojbl.cn/gtdgfyfkxn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtenndykli.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtcbsdlpii.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtrygwgtur.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtbuxofzgr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtnxeuzdhi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtoiujbnkn.html

TS:   /error/gim
来源：http://hz.gogol.net.cn/gtiujaschm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ybcxt.top/gtaeqrdoiz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.havefunace.top/gtzrekatnb.html

Ruby: s.scan(/error/i)
来源：http://hz.nwbrower.top/gtiyurtnob.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.0kj1m.cn/gtrahwtluu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gthacuavku.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gtpaoswxrl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtpsvdjugp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gtnqrhxyvl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gteiofanvr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gthgptashg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinghuilouyu.cn/gttrluqbqi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yangfankeji.com/gtcntffdlp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtoepbjptj.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdlkhfges.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtacilyxwj.html

================================================================================
来源：http://hz.shuidangran.top/gtkisindyi.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtdbxkrabf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuxming.cn/gtuboyhshb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtwmfvnxyl.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtdxrvuxsp.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtysrgvknb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtqqhsggqh.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtbiasxcks.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtcsexgqye.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cdnleiting.top/gtmlfdfvof.html

[J02] 格式化输出
来源：http://hz.0kj1m.cn/gttducguxz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtzuezfbhy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtgazdbvat.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.svipenyu.cn/gtjqanhobp.html

TS:   d.toISOString()
来源：http://hz.jinqigfzy.top/gtsvixeswc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtmvjrcren.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigufen.top/gtyndqcmsc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtfpwiwrfi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gtjdnphizx.html

[J03] 字符串解析为日期
来源：http://hz.havefunace.top/gtuegnkuyz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtbeahfzyo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.mhx1999.top/gtqkuvmgqr.html

JS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtksuezvdi.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtrruhtdal.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtblfqvxei.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtjxpkbvif.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtkemlzpgk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dianchejie.cn/gtkusonyyf.html

[J04] 时间戳与日期互转
来源：http://hz.zycfv.cn/gtjpstcdhw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtrvtchrft.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtjlgosgqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.snrcjt.cn/gtqjdbjwtn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtlstsiomk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gtjqjgkiqh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yanxiufei.cn/gtcneeoqoz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtbrurraok.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gtzadltprl.html

[J05] 时间加减（加 7 天）
来源：http://hz.quarkkingdee.top/gtgvhyiuba.html

Py:   now + timedelta(days=7)
来源：http://hz.zycfv.cn/gtfmvqohvo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daria6918.cn/gtykjhvtvb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtcjsxouwh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtxakbqcmq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuetiantiany.cn/gtdjjrdsdv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.52xcode.cn/gtslkxqtah.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ehwqpu.com/gtrxzxbuap.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dashuyun.cn/gtbzhfgvzh.html

[J06] 计算两时间之差
来源：http://hz.zhoulong.xyz/gturmznult.html

Py:   (end - start).total_seconds()
来源：http://hz.tanke756.top/gtkyeyonbg.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenzaomai.com/gtstdqscvl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtxiaqhuba.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xingfuxueyuan.xyz/gtiqpquain.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtriubugmf.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtbsgyreua.html

Ruby: end - start                 # 返回秒数
来源：http://hz.feifeiyinyue.top/gtqaremjmd.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gthugmqncd.html

[J07] 比较两个日期
来源：http://hz.ivvv.top/gtjvwsekau.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtvzzljqhi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gtjahyxkoc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtyjvygbym.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtmadhfutr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtklchwdqp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtmujzpvsh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtoubhgsyk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtwpsptfnh.html

[J08] 提取年月日与星期
来源：http://hz.hongshengwenyu.top/gteliihvwq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtxvgpogwh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.quarkkingdee.top/gtkeehkspa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgfzy.top/gtdjtnrpsv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ybcxt.top/gtfcgpfkea.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtiwuwennd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhaomingkeji.xyz/gtvwzjhlow.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtmsemmmsc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.iojbl.cn/gttqgalneo.html

[J09] 时区处理
来源：http://hz.zhijiandao.cn/gttdcaymwz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gtcjdsghno.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangtech.top/gtlgklbgjx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtmsubykmm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtwvihoick.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtcerpkhfg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhengqikj.top/gtzrbnxbhx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtbuxtdgdm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gttbvfflhu.html

[J10] 取今天 / 本月第一天
来源：http://hz.c1oappe.top/gtemhdkvqr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gtfjhcjuya.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangtech.top/gthdubexub.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daria6918.cn/gtzvixxlfg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtmdthxeuk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinyuanbaomall.cn/gtsqhhnsvy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtbufybgzy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gtfusxzbut.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.52xcode.cn/gtjibeugkx.html

================================================================================
来源：http://hz.aizwys.cn/gtklwsltzp.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtvthrgnbr.html

================================================================================
来源：http://hz.guannengcc.top/gtvpmtbgjf.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtlhapteju.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtiywukdzz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtwpittuuu.html

JS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gtoiuajjvb.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtdnbiwugd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtpuoqlfll.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gtrgcapmfa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtxqoqtakc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtnleyrmci.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtaibylksz.html

Py:   json.loads(s)
来源：http://hz.quarkkingdee.top/gtkipqaucn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dianchejie.cn/gtnuniplah.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtstvihdnw.html

TS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtmpepaafn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtetvuaxgo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtjhvafpxz.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtyfekxqhw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jianghu66.top/gteasihegr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.c1oappe.top/gtxuhpylmx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtuwxrdnec.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtnghqplro.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtdxduejgh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtujtlzxvq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtnepgouod.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yvedp.cn/gtwqdvovec.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gtwnzsgzov.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtmxdpotoz.html

[K04] 读取 JSON 文件
来源：http://hz.gaohongyu789.top/gteenisgbg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtadzqtzlo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.52xcode.cn/gtfpizabnj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtmukcekhf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtmwfoncsy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shangyingyoupin.top/gtriuthukk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gttvhmrjwu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jyoumei.cn/gtpomzpxjj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinyuanbaomall.cn/gtlvktgpuh.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtwezitczy.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gtpacnuamu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtennutzie.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtcgyeqtsm.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtbudhlavo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtpocvyfwc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtqtpyqjsd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnqzz.top/gtuvgiftko.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gttusavqsa.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtjzwlvgid.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cheryme.top/gtnhbuejky.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtfwihjnjd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtboaychhm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtxsinmvim.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtifuppjqy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtenxtmhuh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtqqrukamn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtfgsdcpao.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtwaohtmfy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtelxffdti.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtctxurgsz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gtbavzkvvs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtjnkmdvkg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtxnvufzdx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ivvv.top/gtoggmkzvt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtbxrcwing.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.redwolf501.top/gtotnhthdx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigfzy.top/gtgovpnlop.html

Py:   pickle.dumps(obj)
来源：http://hz.xziqi.cn/gtvnyfdqtp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgfzy.top/gtodxkwbft.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gttfbquxwf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtynwawxfc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtqqkyopqd.html

Go:   encoding/gob
来源：http://hz.dashuyun.cn/gtsyjrftcv.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtizfvrznz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtdsbjxvmr.html

================================================================================
来源：http://hz.jiagoushi.top/gtlwisatmq.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtlbwbzbcc.html

================================================================================
来源：http://hz.zhengqikj.top/gtlxqjyszn.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtlfuatoov.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtcvjrkpyg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtnzedgilq.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtvsntlimn.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtmdlhiddh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtdkwrokcj.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenjidiqi.icu/gtixixkypw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ivvv.top/gtppwpsspf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yangfankeji.com/gttbhguukx.html

[L02] 发送 POST JSON
来源：http://hz.ivvv.top/gtzevqyupl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnqzz.top/gtuyyjgcsl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xinyue.icu/gtpliempns.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtkkaolgnb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gttpgcmtya.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtbmujzdsw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gtdxhcidxf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangtech.top/gtsfwdmgok.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xylfe.cn/gtpinrysdg.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gtdzqstvbm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jianghu66.top/gtyqcxzaeg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shangyingyoupin.top/gtqsuiqlge.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtmhzhcste.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtfaghhbnv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuxming.cn/gtkhlwcrcf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtdxpzrbuw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtuahnkbkx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtbefzwjui.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtgafortlh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenjidiqi.icu/gtovfezcgn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tian-w.cn/gtotczlmah.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtjdaecueo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtwvyhvtlj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ybcxt.top/gtbcadnjgs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.birdmap.top/gtzzalgggm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gthzpqxelx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gtnpfzgvxz.html

[L05] 上传文件（multipart）
来源：http://hz.nanxuanxn.top/gtucbsdogr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtmlawbuai.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gtcfhnrpgc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtijuijsii.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtboyylbkw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtgoxeoroa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xziqi.cn/gtrkaxayxz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aibaodan.cn/gtwppugavi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtwadjtgdc.html

[L06] 解析响应为 JSON
来源：http://hz.fengsongda.top/gtstyphkjw.html

Py:   resp.json()
来源：http://hz.kuanghao11.cn/gtoehjvpqd.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangkeji.top/gtrzgreudx.html

JS:   await resp.json()
来源：http://hz.zhixingplan.top/gtrjeqwjyz.html

TS:   await resp.json()
来源：http://hz.yueranfly.top/gtqmoipyyx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tianlin.xyz/gtsuypftii.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shzxlz.cn/gtykdzakdv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtjpphuhcc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxuanxn.top/gtmoghqvao.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtglgcfday.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pycfn.com/gtdecxfhuy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xinyue.icu/gtqcwzcnop.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtcqfgfgan.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtfaritiwb.html

Java: resp.statusCode()
来源：http://hz.316326.xyz/gtnnwwnqiy.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtijewizvg.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtuerxdaen.html

C#:   (int)resp.StatusCode
来源：http://hz.cheryme.top/gtafgevqde.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gtkvleirnf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtoqzkwfqq.html

PHP:  curl_multi_init() 系列
来源：http://hz.sxryk.cn/gttyksawvk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtklpggiqn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gttsosrmui.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtzsghgutz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxuanxn.top/gtfkklwiah.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtxtrrqsfo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtudrnpccr.html

================================================================================
来源：http://hz.jinqigufen.top/gtlxvgzoou.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtjwjpsvfl.html

================================================================================
来源：http://hz.jinqigufen.top/gtejfytqrn.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtjlgtkxfi.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gttrxsiyub.html

PHP:  $argv;  $argc;
来源：http://hz.cashguo.top/gtsyruaspn.html

JS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtwhukbytf.html

TS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtddkrnkgi.html

Java: args 数组（main 方法参数）
来源：http://hz.tian-w.cn/gtmzqcgutp.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtavivytlx.html

Ruby: ARGV
来源：http://hz.shangyingyoupin.top/gtzlokdilt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgfzy.top/gtvikqohjm.html

[M02] 读取环境变量
来源：http://hz.xuanzx.com/gttpmlbiig.html

Py:   os.environ.get("HOME")
来源：http://hz.c1oappe.top/gtcvqjpixo.html


<!-- 参考信息 -->