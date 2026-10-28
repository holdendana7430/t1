代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtxhxdjatg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pengpengdd.cyou/gtdlojlqwk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtkyxeixur.html

Ruby: s.scan(/\d+/)
来源：http://hz.9152youxi.cn/gtriidaohl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenlongwang.top/gtevgfykeg.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtzrezajsy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtyqmrdfdn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtpwseymon.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yongpay.top/gtkkiuvyuk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.c1oappe.top/gtdcjhlsjg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtmdvncstt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yueranfly.top/gthhvrlqqf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gtrokgcwdg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.9152youxi.cn/gthbqlbwii.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gtsbbtaxuh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gtjzwnfxtw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtvrojvpvh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtqybgzcrx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gthlpynbgi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aizwys.cn/gtthudyoae.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gthscfjhhw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydjk.org.cn/gtazzydidm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtaqrxugap.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gtuyteruec.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gttvwkjzgq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtmvjbsjhq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtriwslago.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtvtzgtcud.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aibaodan.cn/gtoiiwrwtt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtsotnrplk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtdjxcedfm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinghuilouyu.cn/gtfqsbyoen.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ywan-chungtsiang.top/gtfpkebbhh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtpvqxqjlb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhaomingkeji.xyz/gttlredgif.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtaivroofh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtqknupnac.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gtrshbrtwh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtvewcjvbz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hywenlv.cn/gtzfxmzrsg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtpstumsav.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtbdkduitr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtbdadhely.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtwqjwizyy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.9152youxi.cn/gteqjgrscc.html

TS:   /error/gim
来源：http://hz.ehwqpu.com/gtxacitmut.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtopcostac.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258888.top/gtmdwmoyqi.html

Ruby: s.scan(/error/i)
来源：http://hz.0kj1m.cn/gtlkbkozsf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtuczmbfql.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.quarkkingdee.top/gtsrxnfkme.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zycfv.cn/gtdjeltejz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtderskzvi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtunwkaudb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtbvynngte.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtqgfjzhxj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhixingplan.top/gtqhfgcydk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daxiang520.top/gtbceexszt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fzhhl.top/gtlvtmcnud.html

================================================================================
来源：http://hz.wangdashe.top/gtoqncydui.html

J. 日期与时间
来源：http://hz.9152youxi.cn/gtzhzopuxn.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtfcmibqjd.html

[J01] 获取当前时间
来源：http://hz.tian-w.cn/gtfnjmtnly.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sysykeji.top/gticiahkdd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtcdnfivvx.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtmetoacsc.html

TS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtwmursabp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtysdqpmtw.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtmfylqimv.html

Ruby: Time.now
来源：http://hz.aizwys.cn/gtiukwxrhe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtonqovzhd.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gtmxqyirki.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtpczoiqyz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtiknazqgk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxinkj.top/gthcwocklc.html

TS:   d.toISOString()
来源：http://hz.0kj1m.cn/gtigmpgjyu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtxhpznxhb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yongpay.top/gtfbyiumwd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtjaegvyeg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cheryme.top/gtmsqiokci.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gtxvfdxpdm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.meibo888.top/gtljcorndy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtmtumqbsj.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gttqqhpbnc.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtpqpxlbqi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtumhqxgsk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtruembgkc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtbozynddb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sxryk.cn/gtlyrplqde.html

[J04] 时间戳与日期互转
来源：http://hz.zhijiandao.cn/gtdnwtlsou.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtvlvazkgy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.bjfxy.top/gtcwosbhgx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xylfe.cn/gtpvbcfqvq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sysykeji.top/gtdvcdyufu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtsdbbjpxb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhiwuduotai.top/gtqykwqhkb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jyoumei.cn/gtwkjvqnax.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gthgwxeofk.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtpwuovqqz.html

Py:   now + timedelta(days=7)
来源：http://hz.sxryk.cn/gtbicttrpq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yongpay.top/gtwycpffmv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtyrsdoylj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtztmgschs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtmwcjrknh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuanzhike.top/gtcgewvvfh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yonumen.top/gtqqopudxq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258888.top/gtgfxyakab.html

[J06] 计算两时间之差
来源：http://hz.yongpay.top/gttkdbgfnh.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gtaefyogph.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuanzx.com/gtswowlxal.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtatmbiihn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gtzrdsrswn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtfbjjzksm.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtyuwlzeik.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gtdeehcbav.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gtynytkanm.html

[J07] 比较两个日期
来源：http://hz.yongpay.top/gtmppypnhl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtjgtmpwft.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydzc1.top/gtmcccawzy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtqlfeewwz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtcmjxafug.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guannengcc.top/gtvxrgjrnm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtbknxmcgd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtdgacigkt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtsmelrflz.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gtkeokvvvt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtndwobppw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtmchjqmjn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtkdwjbdxk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtsezyiwhc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aizwys.cn/gtzocwvtpo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtsmtmvovv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydjk.org.cn/gtmjnuakmr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtsvuxaces.html

[J09] 时区处理
来源：http://hz.dianchejie.cn/gtinnmddaf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangdashe.top/gtkioqmyxk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.havefunace.top/gtowgnfubi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtqxlmbkae.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtsnolgdts.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtidbladrq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gttxfqkjlh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gteabxjtsb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yongpay.top/gtcibtzksy.html

[J10] 取今天 / 本月第一天
来源：http://hz.shanyushiyangtech.top/gteawsjwlk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtatoqhvtm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtfrnyrukw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtksztlmsg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtygguzmnj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtpbrizuic.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.52xcode.cn/gtkcbvzpzz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtrwwlvszo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ehwqpu.com/gtjqovmqga.html

================================================================================
来源：http://hz.guannengcc.top/gtyuscfsvs.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtmsqrljvp.html

================================================================================
来源：http://hz.zhijiandao.cn/gtyatuhebx.html

[K01] 对象转 JSON 字符串
来源：http://hz.c1oappe.top/gtdqwvnndh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtikfcsiyq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtavyyswqo.html

JS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtuqhbpnkt.html

TS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtnoiiqsut.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ppjwa.cn/gtdcjjiykn.html

Go:   json.Marshal(obj)
来源：http://hz.cdnleiting.top/gtanrwguhf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jianghu66.top/gtopxcvoiq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtllyvtixf.html

[K02] JSON 字符串转对象
来源：http://hz.nanxinkj.top/gtpzqdoeme.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtpgbpkwhr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.svipenyu.cn/gtdwcphuxs.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtjkokgung.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gthgyltfiu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtrmopvyei.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtfguzrfmo.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtpwawqheh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtlezqatdg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtncgguojv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.meibo888.top/gteuwqyudg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtwrlwfvbe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtvaxmhvca.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtkwquurht.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aibaodan.cn/gtxabkidpg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gttvpflaoi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hongshengwenyu.top/gtirpzuisa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cashguo.top/gtjjuotugg.html

[K04] 读取 JSON 文件
来源：http://hz.redwolf501.top/gtgmkeuzqc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gtxrukvjvn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.meibo888.top/gtjnlxhtrz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtjdbebpod.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtdprmmpgo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dashuyun.cn/gtjgftsymn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtjkymwema.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daria6918.cn/gtzmimzopr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sweek.top/gtjhnnssge.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtynwhrouw.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtyvxfrhzv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gtqkhzhhyd.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtysntvkwj.html

TS:   structuredClone(obj)
来源：http://hz.cheryme.top/gtavhxfdhd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gtkgcusxez.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.svipenyu.cn/gtcmnxtmuw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtvtnbxnlj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtimdusoom.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtmglctqyc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yvedp.cn/gtgejktmgv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangshuangyany.cn/gtxlgjcqnh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtdvumsolj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtouogzkrf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtmllklmqr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtlyzqqlvp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtfvigqxxx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtopasilfm.html

[K07] 进制转换
来源：http://hz.hongshengwenyu.top/gtoyfakylm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxinkj.top/gtdvjuhvaz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.dianchejie.cn/gttfkcaavy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtruslwtwl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gttkgvgeeb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtvcjwfegl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtfvjtzoib.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yanxiufei.cn/gttkjbhyop.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtbectbgqz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.c1oappe.top/gtamzqqwpv.html

Py:   pickle.dumps(obj)
来源：http://hz.gzhubu.top/gtlnzdqxlx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtphaxpdes.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtpueeqdki.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtdatbdqjm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gtobfwfmvk.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtzoqosjfm.html

Ruby: Marshal.dump(obj)
来源：http://hz.sweek.top/gtdavqomnr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtzixlacvc.html

================================================================================
来源：http://hz.xinyue.icu/gtnczdoyea.html

L. 网络请求
来源：http://hz.ywan-chungtsiang.top/gtvbvrudhx.html

================================================================================
来源：http://hz.sweek.top/gtyckcyzbq.html

[L01] 发送 GET 请求
来源：http://hz.gotoacloud.top/gtccsxbxmh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gtecmzjbqx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gtfssthjtf.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtmdcbstax.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtapoblmko.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtgsirbdmz.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtzcecfmma.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtsecvabpn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.snrcjt.cn/gtfkusjsdp.html

[L02] 发送 POST JSON
来源：http://hz.yvedp.cn/gthvscnxyf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.meibo888.top/gtusnylxlk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtiqzyamuu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtwnpjjwkr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtyckzncid.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.redwolf501.top/gtmyrhixst.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj20258888.top/gtltcmtmvs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sweek.top/gtudhjtqzw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258.top/gtaryzjmpl.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtuejeuriv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gtbnrfigpk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.havefunace.top/gtlgkizrvr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtmpitanby.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtzsvoglod.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtipoepiha.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtrqkklasr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtvetvndoj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtomsepvws.html

[L04] 设置超时
来源：http://hz.jianghu66.top/gtprcykwem.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gtrnfqwwex.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtspskdenu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtyfoqvwua.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtjcoyopyg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtrhwzelce.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dashuyun.cn/gtpplllosx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ywan-chungtsiang.top/gtzhftgfig.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtuapwdixt.html

[L05] 上传文件（multipart）
来源：http://hz.9152youxi.cn/gtdygdkpbh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtigylmzrv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gthfvtylwa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtemvryfys.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtlidikwxz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dashuyun.cn/gtdztsgdfa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gtvtnptmwc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtxbrfvekc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cashguo.top/gtckvbeizs.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtbiqpwsvd.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtemdydtyd.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gtyqqwxzqa.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtjvbgghdu.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gttmjizaaz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtcycwykrd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtddzrotse.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gtnswqdmvs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yonumen.top/gtlopkrfve.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtvhexbstj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtxavwkiib.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.svipenyu.cn/gtdeanclft.html

JS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gttvuwsinl.html

TS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtsvlawfac.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gtjpdejhuq.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gteoymrnrc.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangkeji.top/gtkgdsrpdv.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtsuhrrgqv.html

[L08] 并发请求多个地址
来源：http://hz.svipenyu.cn/gtbwggplja.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtsmarclcd.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangshuangyany.cn/gtqepsaiug.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtadrjaudy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtuotbrgvh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtqncyrfgo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj202588.top/gthcydhyqf.html


<!-- 参考信息 -->