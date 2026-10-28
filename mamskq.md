代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtfqkzdtsy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtgcfcggcb.html

JS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtjvlmboal.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtbrgrkxkt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yangfankeji.com/gtoxnbwkyf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daria6918.cn/gtrfbiyfvb.html

Ruby: s.match?(/\d+/)
来源：http://hz.sysykeji.top/gtiditlont.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.redwolf501.top/gtuhtlmiis.html

[I02] 提取所有匹配
来源：http://hz.chenlongwang.top/gtmutgnnzo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtbwwsdcat.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtjucxkoqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guannengcc.top/gtawzecjrh.html

TS:   s.match(/\d+/g)
来源：http://hz.ywan-chungtsiang.top/gtcpdwliux.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gogol.net.cn/gtckuyiqhb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnqzz.top/gtflwbtexi.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtbtgdlzxu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gzhubu.top/gtdmegdwtw.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gthkmbsexv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnqzz.top/gtmirrgrrq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangshuangyany.cn/gtfixwexdi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.0kj1m.cn/gtmnfqvwcb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gthjnaixyw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtkuaiuopu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtnxlbozoy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtywzpptfu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.9152youxi.cn/gtgahukdpv.html

[I04] 正则替换
来源：http://hz.pengpengdd.cyou/gtozhcwdyb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtpbsvnepg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtsmdeyycc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtanrgwbjv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtaqixfrhm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtvyzzafhv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtabkyqdnq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinyuanbaomall.cn/gtulgjjbbq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtkilxhmhg.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtlykfhpuo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gtexgrtlmp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtraivjffn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtycxsqatg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtqyafsgoq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tanke756.top/gtttfrcbgr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxinkj.top/gtyvyyhder.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtjmrxjunf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtpntwsmui.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guowangkeji.top/gtulamwlwb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtpqztdsei.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinyuanbaomall.cn/gtnnzuwloh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gttubplfrz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtfngxacbw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtjnpeokhq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxuanxn.top/gtstyogijv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtatlupkfh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtrkqyncir.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtayhvdyss.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtibmigknw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtxqyqeajk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtoannrkqc.html

TS:   /error/gim
来源：http://hz.ybcxt.top/gtzrzumqnw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ivvv.top/gtbwuiwbpj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenjidiqi.icu/gtukfhjnwx.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtvkvbdexn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtbginexob.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gtiaaxtous.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtivuisgod.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258.top/gteeikemdh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtqitsdavi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtgkcyxgbw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtdtmgbpjx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.birdmap.top/gtgngbagqd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gaohongyu789.top/gtyguqzkus.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtigvrputo.html

================================================================================
来源：http://hz.tanke756.top/gtgeiyjjkh.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtvpwvpqbx.html

================================================================================
来源：http://hz.ppjwa.cn/gtbilcrick.html

[J01] 获取当前时间
来源：http://hz.52xcode.cn/gtpyovmliw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gtgmbafqea.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtygebjewx.html

JS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtrlnhtbqo.html

TS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtrasepgtv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtnodywgzw.html

Go:   time.Now()
来源：http://hz.ivvv.top/gtrkvejgrn.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtvdnkcfvz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtxljfouev.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gtukhswtmi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtgkxghctc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtbmknojbb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydjk.org.cn/gtbihjmymq.html

TS:   d.toISOString()
来源：http://hz.aibaodan.cn/gtvphmpbul.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtjcyxzzgt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtmfgzewwd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtlfbrezyb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtovuxtpev.html

[J03] 字符串解析为日期
来源：http://hz.ppjwa.cn/gtjmazxqdi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtrsxskojj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jianghu66.top/gthwnrtrqh.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtyubxjypa.html

TS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtekepoobs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtuqtsoyks.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.vqdsnc.cn/gtfoukgeve.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtvecibarr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.feifeiyinyue.top/gtmkmrkugu.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtljephflv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gttpsspyku.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gtmhvjxsuj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtqisyqhms.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daxiang520.top/gtkmivsqxn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenzaomai.com/gtzrxodftw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtbczipyjr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tian-w.cn/gtzpxzzfse.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuxming.cn/gtxcbxmhck.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtgtfiiqbq.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtugvigmky.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gaohongyu789.top/gtlqdsdbyx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtrdpunhmc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtrfdspsqc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gaohongyu789.top/gtmxauxxhe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigfzy.top/gtxxkrlzyd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gtmsenkuqg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtqzzudtii.html

[J06] 计算两时间之差
来源：http://hz.fengsongda.top/gthlpixdhd.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtqnipfttb.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtphvkmubm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtqmaadoxq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtxbjlhbnp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtmlfiobgf.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtqjsrbtzk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shangyingyoupin.top/gtpvatxxsu.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gthiiktbob.html

[J07] 比较两个日期
来源：http://hz.quarkkingdee.top/gtzgrsqvfk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtakhmgzkw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gtxdzljqhh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtrcobvuth.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtuhchqyad.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtbucpolgu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aibaodan.cn/gtbbpfgyqa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtcukvdeyj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtytqbktms.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtymnusbpi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtidvvklbr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.0kj1m.cn/gthxorryrx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.andypj.xyz/gthqiuyrja.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gthuljpjgg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gthdzpmsvi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.52xcode.cn/gtpgkuvqam.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gtkcqldgfm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hysaishi.cn/gtmkncutdp.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtcplivyha.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gthtvjjlqi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtyjgockrk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtzptmdvxv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtvsbhbokl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.mhx1999.top/gtfjljvfzx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ivvv.top/gteuwoidtq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtzbmqfvhv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jlsjyb.cn/gtxrhplhpt.html

[J10] 取今天 / 本月第一天
来源：http://hz.bjfxy.top/gtegkedvqv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtwxdssadm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gtgzttcyww.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtgmldcktc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtbfnwzqeq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.birdmap.top/gteumdplri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtlenufbtn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.havefunace.top/gtkidrrlof.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gtjtmkhqjt.html

================================================================================
来源：http://hz.yueranfly.top/gtzzcoosyr.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtuhbbtync.html

================================================================================
来源：http://hz.nanxinkj.top/gtvqklepvm.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtwpkdgwin.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtlyybacbj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtxvwnozke.html

JS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtbtymbffa.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtavyoohbc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtcmacegii.html

Go:   json.Marshal(obj)
来源：http://hz.xingfuxueyuan.xyz/gtmgpdxmld.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtmjvfibsd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhixingplan.top/gtvtxbsita.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtojcrdemo.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gttdnggqvj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daria6918.cn/gtnutybirz.html

JS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtydfzlplv.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtnlvahgec.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtzyevqtnk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtlcqdwith.html

Ruby: JSON.parse(s)
来源：http://hz.9152youxi.cn/gtwmlsrtel.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtwowqgrfz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.c1oappe.top/gtvguzxufw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtclphakrk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtcdqelsvz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtsxlqkflo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtcemoomoz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtdeevczvy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtwwzzzjhn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtmqhdduvj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jyoumei.cn/gtoamwplmb.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gttttkbhkz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtqtcboiiy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtjztowrnv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gttoefwztt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtcrnugqfw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtgjjtdstd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtvspukgev.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.snrcjt.cn/gtosobsact.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtxdbidmwj.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gtysrjdado.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtspnwsfaa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gtsktzxlnt.html

JS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtbwsholph.html

TS:   structuredClone(obj)
来源：http://hz.zhengqikj.top/gtkitvplxp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gttibolvtq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangkeji.top/gtgwdkknmi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.vqdsnc.cn/gttfxrcyal.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhixingplan.top/gtuxkhgvav.html

[K06] 解析 URL 查询串
来源：http://hz.zdqjudy.top/gtlwuhaobw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gteurpmwfs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gthzxtcuaq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtbwecwkgc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtmlffwqia.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtthkvdctz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gtmdbgxtwc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gthtbtacgp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xziqi.cn/gtlmfsevkd.html

[K07] 进制转换
来源：http://hz.snrcjt.cn/gtsrmyeoik.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zycfv.cn/gtykrxchvt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtnwxjekgv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtxhayveco.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtwqexkkrn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtoqlkunwp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.quarkkingdee.top/gtwbagcmgr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gtoelbqqau.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtroajmhxt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtxaagjjog.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtlitmbalu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fzhhl.top/gtikduchvr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtehzvywse.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtkciaoror.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtseasekwx.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gtwygdpvjx.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhiwuduotai.top/gtfsddavgg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtzudvnkuo.html

================================================================================
来源：http://hz.cashguo.top/gtkfdbopjp.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtyhhkcddr.html

================================================================================
来源：http://hz.dashuyun.cn/gtikfhesqk.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtxhiupfqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtgxjkaidz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtgynlbpuv.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gtwaimlkwj.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtgcwmvabi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gzhubu.top/gteupiajdf.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinyuanbaomall.cn/gtezilumdy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgfzy.top/gtazoymurr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtxbjmrvpx.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtjwdjnasp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sufxvd.cn/gtuixsdvfv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhixingplan.top/gtubckatbz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtoywattco.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtduubkyvw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtkccgmqhf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jyoumei.cn/gtfdaudilq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cdnleiting.top/gtdgqryrlm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtjqqgoftv.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gtskhrswyl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgfzy.top/gtxwyoqyrt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cheryme.top/gtmmxbbhvu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtqtkkeypa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtowncqruc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtobslfahp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aizwys.cn/gtzwoqvgsf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gtwemwrhfp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtrwfnisbm.html

[L04] 设置超时
来源：http://hz.sxryk.cn/gtvzdijhza.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhengqikj.top/gtftbqflhw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gtrbwhnfed.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtmniwwzvn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtirvjljlt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gttfivjvdh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nwbrower.top/gtxputodgr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hywenlv.cn/gtwvktrmoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtqwdcxnsr.html

[L05] 上传文件（multipart）
来源：http://hz.ybcxt.top/gtxebowrox.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtxsyjjhal.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sweek.top/gtiupiwavl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtueejmhcx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtyiqbnnby.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnxiangtu.top/gtchczjfpq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hammf.cn/gtgcjgtlgz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tianlin.xyz/gtdbghkyjg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ybcxt.top/gtfrqranvg.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gtyhkwagsq.html

Py:   resp.json()
来源：http://hz.hnxiangtu.top/gtdvkjjrfw.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtjrorfvgl.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtmzrorqeg.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtevageprz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtvdnccswx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigufen.top/gthorydhuu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.dianchejie.cn/gtvmjerffe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtsgkgfolz.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtwigfrrta.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gtvlizpjks.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtrhjfydqz.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtkgbighou.html


<!-- 参考信息 -->