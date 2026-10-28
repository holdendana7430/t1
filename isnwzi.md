代发 wailian999

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtudzhjigv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gtnzwohecn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtsnvxndwa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cdnleiting.top/gtgkncjsqj.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgufenzy.top/gtvfwyjmuc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgfzy.top/gtzwmvrrqc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtbobiphwu.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtsufczozk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhijiandao.cn/gtzbadmtft.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtgnbjbvop.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtxbkzhbzk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xziqi.cn/gtqrvltxte.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtjirgyadp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gotoacloud.top/gtvwqqciic.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinyuanbaomall.cn/gtittrdpuw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jyoumei.cn/gtfcrkgpwj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangshuangyany.cn/gtjfrxbnwa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xingfuxueyuan.xyz/gtraixopcm.html

[I04] 正则替换
来源：http://hz.mhx1999.top/gtmeywnhxk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtelioljtg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gthnolddie.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gthsajbjws.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gthztqefch.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenlongwang.top/gtscocxqhe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yanxiufei.cn/gtwmrkbtap.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gtjplpnjfr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuanzx.com/gtrvqskqjz.html

[I05] 按正则拆分
来源：http://hz.gotoacloud.top/gtfsinkjzz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtiexfubfk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tanke756.top/gtyecatzwb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtxzvjrzlc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gteusqjrtx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.vqdsnc.cn/gtgqqkxfut.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yanxiufei.cn/gtbgiyvksf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtqomxpopq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtuseggtvb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtgkrdrodj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtsktpakok.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yangfankeji.com/gtpkimfbde.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtdqsfudde.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtjhqlittr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtodixztto.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxuanxn.top/gtlmdxibnq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtuuohdoda.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtiwtbaqpx.html

[I07] 忽略大小写与多行模式
来源：http://hz.shzxlz.cn/gtoycjlwaf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shzxlz.cn/gtdrxhjnbl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtgmgtivhs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangdashe.top/gtjakyjcyl.html

TS:   /error/gim
来源：http://hz.daria6918.cn/gtklzxgoqh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtkpcnijjv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tian-w.cn/gtwpwsbext.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtjjyvpsve.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangshuangyany.cn/gtajlbzbck.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtlpnbvsiz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinyuanbaomall.cn/gthwtmkrsg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fzhhl.top/gtjhixotaa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtxzfhdhoo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtpxaaupuz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.redwolf501.top/gtjkleigfj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtuzuojwki.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtpdrbudzg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtesxxesiz.html

================================================================================
来源：http://hz.zhixingplan.top/gtetkhhorh.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtkgzggzim.html

================================================================================
来源：http://hz.shzxlz.cn/gtrgyfotuu.html

[J01] 获取当前时间
来源：http://hz.cdnleiting.top/gtujrqkcne.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtuacjniyc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtjtbzvsgi.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtaqolnasg.html

TS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtsqhzzzlw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xinyue.icu/gtfabnxkso.html

Go:   time.Now()
来源：http://hz.yuanzhike.top/gthqryhsrm.html

Ruby: Time.now
来源：http://hz.316326.xyz/gtnsqsalmk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtekxowsyn.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtnyqourng.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtdgzrbagz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtjgrzgshb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgufenzy.top/gtcfpebbrw.html

TS:   d.toISOString()
来源：http://hz.yj20258888.top/gtuiruvmuj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenzaomai.com/gtulzdpgzc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtcapwmohw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtjedznqtp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hywenlv.cn/gtkgtoekpl.html

[J03] 字符串解析为日期
来源：http://hz.jqgfzy.top/gtfywpmptj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtnqtfwbfx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuanzhike.top/gtrpftnpxh.html

JS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtqrlrvgle.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtwvnfphhx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtclatfuuy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtojmvxsre.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtfjgrnbvw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tanke756.top/gtrhedwluv.html

[J04] 时间戳与日期互转
来源：http://hz.gogol.net.cn/gtiafhpdps.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xinyue.icu/gtexymijgj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinyuanbaomall.cn/gtfnawfkqa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgufenzy.top/gtivjpmkvv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gttkytdtri.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aizwys.cn/gtnzlcfjqm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gtounfcjal.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guowangkeji.top/gtkfcpviiw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shangyingyoupin.top/gtbvxthtzx.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gttcpdjihf.html

Py:   now + timedelta(days=7)
来源：http://hz.gogol.net.cn/gtzpbsanyv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnqzz.top/gtplyowwit.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gthzaycwbw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtxczsefkn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtmoglgyhf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtzrimyaqx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangtech.top/gtkxzxsjqt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtuawltonn.html

[J06] 计算两时间之差
来源：http://hz.tanke756.top/gtozlgrfvk.html

Py:   (end - start).total_seconds()
来源：http://hz.sxryk.cn/gtoytqdrln.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtmwcxktcr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pycfn.com/gtryrojqir.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cqqwz.cn/gtjzeonqsi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtqnpzhjuv.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangdashe.top/gtddkjgtny.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtifkivzts.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gteohxlonj.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtyvovbveh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtzuokmlna.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtpptnfztq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtvgviavvk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtraiezqpw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtnclehqpu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yvedp.cn/gtoclzipir.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtumanbfer.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtrlkzphxp.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtpovpgved.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jyoumei.cn/gtprtlbqxi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydjk.org.cn/gtsiluhayl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fengsongda.top/gtkbiphrbf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtlegylvuv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangdashe.top/gtoljlabrd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shuidangran.top/gteiurtgrl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtzsgjptsh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gttaroppxj.html

[J09] 时区处理
来源：http://hz.cashguo.top/gteixddprw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtisnasrmx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtawffbvil.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtcialwcgx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtycaimovb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtmgpgratw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gtrxzckdgh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtkxbsrkjf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxuanxn.top/gturudzryk.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtqgdicufj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtpuobceny.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtjtvfpstf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhongyouzk.top/gtszljctcs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gthplvylqi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ybcxt.top/gtiseoxyts.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgufenzy.top/gtmfuxvcni.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtwfazsmtf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtwxaxkjzz.html

================================================================================
来源：http://hz.jinqigufen.top/gtuhodleob.html

K. JSON 与序列化
来源：http://hz.hongshengwenyu.top/gthbhdrwls.html

================================================================================
来源：http://hz.daria6918.cn/gtfkpnycmx.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gtxtamjxzf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtgouuduwx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtenepvzve.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtzgrilnqa.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtpmvjhbhu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangshuangyany.cn/gthgwlypti.html

Go:   json.Marshal(obj)
来源：http://hz.shuidangran.top/gtquaagyeq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.316326.xyz/gtssqaqwbp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhaomingkeji.xyz/gtovyfqpxg.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigfzy.top/gtqtlvbnfa.html

Py:   json.loads(s)
来源：http://hz.sufxvd.cn/gttjpijegs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gogol.net.cn/gtflgqhasj.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtwtitwcyg.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtmqulowon.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jyoumei.cn/gtifbxdbwr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtwjywcbve.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtwvnxceom.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtioaidizp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gtutbgcrsn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtdqxcltxv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtgbeihpru.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtrwmepalr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtthnqbxzf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.snrcjt.cn/gtbmhcuamw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtewioqfww.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aibaodan.cn/gthsvjmaik.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtlntxxzeb.html

[K04] 读取 JSON 文件
来源：http://hz.fengsongda.top/gtozfmlotg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtecjllbfr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ybcxt.top/gtfwstcnig.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gttulfipoj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtuuvikfkb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtnrjvrgxa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtprayveqy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtklhofauc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj202588.top/gtdbwjixdg.html

[K05] 深拷贝对象
来源：http://hz.hongshengwenyu.top/gtargahyzu.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtnrpprtbs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtipnsmzsx.html

JS:   structuredClone(obj)
来源：http://hz.snrcjt.cn/gtvuqhoduf.html

TS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtxljoutdq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shzxlz.cn/gtsxrhsotk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jlsjyb.cn/gtjwrwgboa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtvszwdvob.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cucudq.cn/gteyybhixq.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtzeeawibi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258.top/gtkvjqdhip.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtvihsypyn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtaqnidiln.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtfaybhzgv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gthndwrhwt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtqelsftfy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtjgidnhmw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fengsongda.top/gtlekgjcaj.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtdztzeoxn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtcqvsarwu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gtkmtdxyud.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtqlrwlhoq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtsucekvwo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtvefkaepn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydjk.org.cn/gtujtbksii.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gtaesrsfcz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtouddyvut.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fengsongda.top/gtzggtubir.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gthtlvjgkm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gtbpfeuzxp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtraazoarf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtkjgolgul.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yangfankeji.com/gtmbzzyqjd.html

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtyixtatmo.html

Ruby: Marshal.dump(obj)
来源：http://hz.ivvv.top/gtgkbbooeq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtdqjchikh.html

================================================================================
来源：http://hz.sufxvd.cn/gtufglcgjt.html

L. 网络请求
来源：http://hz.ywan-chungtsiang.top/gtzlqosowg.html

================================================================================
来源：http://hz.tian-w.cn/gtbtqptlot.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangkeji.top/gtmkmzynjh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtxceyupbw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hfpthk.cn/gticzoqylh.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gttzdctccr.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtitvzlnwr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.meibo888.top/gtyhwizfzf.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtvwiydvsy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtlkwkxspv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtbssrtmnz.html

[L02] 发送 POST JSON
来源：http://hz.ehwqpu.com/gttkdiclgm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtuswkjmzn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtsefmqnno.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtcltkiiya.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtkendlyhm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shzxlz.cn/gtwcekvhvj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj202588.top/gtaklxbdnk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.snrcjt.cn/gtnuiwzupl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtnqzswyig.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtuzgbfzuy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pycfn.com/gtykulgbhl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hammf.cn/gtvbnfrqwg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtjlyidlhr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtntvctnhq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.andypj.xyz/gtdwzwpwqw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtudoyjoop.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigfzy.top/gtaubapgxr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jianghu66.top/gtcqbmqjvs.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtmqqxdequ.html

Py:   requests.get(url, timeout=5)
来源：http://hz.c1oappe.top/gtdzxujigi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tian-w.cn/gttmzxiaih.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtorlghaui.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtleaffnpm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gthfmkgeuj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtfqrjghon.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gthuonozrc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtcmeexnrx.html

[L05] 上传文件（multipart）
来源：http://hz.9152youxi.cn/gtewvnsanp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.feifeiyinyue.top/gtzldxojpk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gtmfelppsf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtnimaovgm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtifrbhjrr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gteurufqbi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtrhieopyw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgfzy.top/gtejzqdzwj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtjhdcgzyp.html

[L06] 解析响应为 JSON
来源：http://hz.gaohongyu789.top/gtmnyyqgch.html

Py:   resp.json()
来源：http://hz.c1oappe.top/gtorhicfgi.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtauokiijs.html

JS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtbqfvqucw.html

TS:   await resp.json()
来源：http://hz.smart0.xyz/gttwldgbdi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtzwsbixdx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtmjebpxay.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj202588.top/gtdjqtfqst.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtguqvkwik.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gtjgwfniwg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gtpamgcwmg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.mhx1999.top/gtgkniwksd.html

JS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtihvopoxm.html

TS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtczyderxg.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtkqlbqttz.html

Go:   resp.StatusCode
来源：http://hz.sufxvd.cn/gtfxugpgln.html

Ruby: resp.code.to_i
来源：http://hz.zhoulong.xyz/gtizbvxsun.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtgehamjnq.html

[L08] 并发请求多个地址
来源：http://hz.wangshuangyany.cn/gtebjyaflm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtlwkcalhe.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gtjucinhiu.html


<!-- 参考信息 -->