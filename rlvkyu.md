代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtzqfvuytf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuetiantiany.cn/gtpdabvdnm.html

JS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtkvfqifzp.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtpbcogtym.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtwnwnjeix.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jiagoushi.top/gtebxisshp.html

Ruby: s.match?(/\d+/)
来源：http://hz.vqdsnc.cn/gttuylnnsv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tian-w.cn/gtqsmxtpsp.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtseuawidf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtvkidnulc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtoclelbhy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtymjhagvk.html

TS:   s.match(/\d+/g)
来源：http://hz.hammf.cn/gtdkswkbnh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtzjremfjq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jyoumei.cn/gtoqvmidyk.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangtech.top/gthrcthgok.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ivvv.top/gtddwstjkq.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gtgzzufrea.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jyoumei.cn/gtlkonfvje.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fzhhl.top/gtwdwtjbvt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gtbudpzuwv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtpfmpzotq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtvbhzcmfz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinghuilouyu.cn/gtpxgomjsk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shzxlz.cn/gtprnzajmj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtabvgpmsa.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtnkfhyvvm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gttckgojcf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuanzx.com/gtjxbeedxw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtxnuapwuv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtlfwpdsbc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtzhnloxwn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtudcdbiol.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtjncylngg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtifbhrvsj.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gtnqjpeouj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dashuyun.cn/gtujrxuput.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.bjfxy.top/gtewympesz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtanlwjfcv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtaetlvowc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daria6918.cn/gtanqnrayf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gtwtqnxnhx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtsfvoletc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shuidangran.top/gtemjnqjbe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ybcxt.top/gtphcqdojr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtialabfzx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtfgcygjrv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtetqdlyof.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtmollobul.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtaompikyc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hammf.cn/gtdrhtjekf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtwqzcveqt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtjwhbysdp.html

[I07] 忽略大小写与多行模式
来源：http://hz.xylfe.cn/gtuwfhxokg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtkcnsbssf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtuvtginpd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cqqwz.cn/gtnfyrieox.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtvywjfrbm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fengsongda.top/gtorirqews.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtdsjtnaiv.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtejxlrqnj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtfkugfdsm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtvpwynulz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtkzqylmwq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtbeljuznk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtrokufjis.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtxgwckkca.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtithsbnbr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtjouyupei.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinyuanbaomall.cn/gtyowdbyeb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtupiqqixz.html

================================================================================
来源：http://hz.cdnleiting.top/gtlmmlzklo.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtyulveyem.html

================================================================================
来源：http://hz.cdnleiting.top/gtibefkxwf.html

[J01] 获取当前时间
来源：http://hz.guannengcc.top/gtkfjzmbhj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gtndntkckh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtgixykday.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtkafmltqe.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtkyxkzeeu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtjynjdnqt.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtqcbagpcd.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gtrusrzdvl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhixingplan.top/gtpagsmolm.html

[J02] 格式化输出
来源：http://hz.haohaochexian.top/gttevdxecy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtwjrmksjv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtqsdsvqyw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtyovmeebl.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtwuagpwad.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtcvvwywrh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jianghu66.top/gtzabwsadt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtzncmovrg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xinyue.icu/gtjzswglwa.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtuvojnzzn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhijiandao.cn/gtvyladocv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtucdmovaf.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtdxmcayxg.html

TS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtyeavovep.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gthkgwzgac.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.vqdsnc.cn/gtsvvcmtvv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtgkbhajor.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guannengcc.top/gthcyczzam.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtocgxfbza.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.iojbl.cn/gtpxbizina.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gthjlusvfs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gthpvrpygu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhaomingkeji.xyz/gtmhdvujhe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtqozrlhvj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cqqwz.cn/gtxbxlctum.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shuidangran.top/gtpmnlmgae.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.redwolf501.top/gtymdkuetu.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtbcdtszel.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gttdonhzrs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtbabdajwb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtlicoldje.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtdloyohyp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zycfv.cn/gtetpjflcu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtylzmcwtn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtbvogufuf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtacfswywj.html

[J06] 计算两时间之差
来源：http://hz.gogol.net.cn/gtxzfcmujm.html

Py:   (end - start).total_seconds()
来源：http://hz.shangyingyoupin.top/gtssmkcivz.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtccspgybp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinyuanbaomall.cn/gtamotrcwz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tanke756.top/gtdvuqrquh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.0kj1m.cn/gtscwnwxio.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhixingplan.top/gtopbzrabs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yanxiufei.cn/gtufaqhixe.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gthmvnqtfi.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtsfyfghwh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtxemzamim.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtkvnlyuar.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtegdymcwk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtblwamnok.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhiwuduotai.top/gtkyjkxkhi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtgwmrpoik.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtzsaskqhn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtnmqltcbv.html

[J08] 提取年月日与星期
来源：http://hz.tanke756.top/gtwuplqnwr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guannengcc.top/gtpbnjokad.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtyqwmkgjm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxuanxn.top/gtfiwizdoq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtagzexuen.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtejaoumie.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gtkicziali.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydjk.org.cn/gtrtivfsft.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.smart0.xyz/gtbprxbkxd.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtddrwrulg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guannengcc.top/gtejzndilj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fzhhl.top/gtqvttzary.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtwzcyrmrw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtjclxpeaj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ywan-chungtsiang.top/gtcysnwyum.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.quarkkingdee.top/gthyzcofth.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgufenzy.top/gtfxlgvwrl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gtrasexivm.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtbzgdyclh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtqlvfndyw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenjidiqi.icu/gtqapyzear.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtmouzrdjm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.316326.xyz/gtiykwjpbe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtrjfqntwt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yonumen.top/gtxvhwfwnf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gtuujlcgal.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hammf.cn/gtprupalgh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsyzldebu.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtujvlouki.html

================================================================================
来源：http://hz.yangfankeji.com/gthcwjchgu.html

[K01] 对象转 JSON 字符串
来源：http://hz.hysaishi.cn/gtwbvlorqd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.andypj.xyz/gtqaqoidch.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtfcowyxpj.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtselwakoo.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtocysavbd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenjidiqi.icu/gtkckubzwt.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtzwfmhjxa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgufenzy.top/gtnozrptut.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtutvphahp.html

[K02] JSON 字符串转对象
来源：http://hz.dashuyun.cn/gtrqklpbtc.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtvpkrhmhg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtwtoctwli.html

JS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gturhkhjwc.html

TS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtmbthfrgl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenzaomai.com/gthkxwjeiu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtojgyxvds.html

Ruby: JSON.parse(s)
来源：http://hz.hfpthk.cn/gtlsexsetv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtrmvcqxjj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ivvv.top/gtnykehkvc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gteudacrun.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gteozcnmht.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gttkestsfm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtmgliyzyh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gteszakywo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuetiantiany.cn/gtviyrghzb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtpkuycfra.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtfgejgmip.html

[K04] 读取 JSON 文件
来源：http://hz.cucudq.cn/gtdwvqwccd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtyqpzmubv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtzovymjju.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtpcpvntki.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtzgkdriyn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gthncdsylr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtyymizftu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gtwrzwfelg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuxming.cn/gtchbhmplh.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gthjfapivy.html

Py:   copy.deepcopy(obj)
来源：http://hz.ehwqpu.com/gtbzxvjkon.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangdashe.top/gtsolmulwm.html

JS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtvaaslagu.html

TS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtwuhmzgoh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yvedp.cn/gtpsspijrd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.bjfxy.top/gtotrjyszb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ehwqpu.com/gtcqiyfikr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtmslpyvpd.html

[K06] 解析 URL 查询串
来源：http://hz.daxiang520.top/gtdjntwqvw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gtztkgicne.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtvpulydib.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtekkxlzel.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtymshxhvn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gtwizvnlgs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtnammjlhm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sufxvd.cn/gtthskwkyx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yvedp.cn/gtyasnrjno.html

[K07] 进制转换
来源：http://hz.vqdsnc.cn/gtzfrdiwhq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shuidangran.top/gtsigawtwe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gtrvprvdhs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtjtsiamwb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtqujlploc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtdrhvgqqv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gtobofmugg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhongyouzk.top/gtnxeitjvm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.vqdsnc.cn/gtewpxokbg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtzmgozxeb.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gtvpdosgou.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gtkiimmcvo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtruotgaen.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtwpfwzvki.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cashguo.top/gtczdwgoec.html

Go:   encoding/gob
来源：http://hz.haohaochexian.top/gtwvturjvd.html

Ruby: Marshal.dump(obj)
来源：http://hz.gaohongyu789.top/gthwbaiouj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ppjwa.cn/gtrqnwawxt.html

================================================================================
来源：http://hz.ivvv.top/gtqgxfyhqo.html

L. 网络请求
来源：http://hz.tanke756.top/gtyqroqjia.html

================================================================================
来源：http://hz.svipenyu.cn/gtgwffvhzm.html

[L01] 发送 GET 请求
来源：http://hz.xinyue.icu/gtljooqjvd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtguegvebq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtefvqkrlc.html

JS:   await fetch(url)
来源：http://hz.birdmap.top/gtokfdgmtr.html

TS:   await fetch(url)
来源：http://hz.pycfn.com/gteatzheom.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhoulong.xyz/gtpzjdshmd.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtcdzhjjpl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hysaishi.cn/gtymeksdqb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtbtyflcmq.html

[L02] 发送 POST JSON
来源：http://hz.zhixingplan.top/gtnaszfwuq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gotoacloud.top/gtzfawnxci.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.meibo888.top/gtsohdubzt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtxhygtkik.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtftkrbxab.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuanzx.com/gtrhgjbujl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tianlin.xyz/gtvukblhbh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gtpehphilf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nwbrower.top/gttbfbmmsv.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtjlggypkp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtkgrneqkt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.c1oappe.top/gtklumkyqe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtjmgtsxtk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtujbkhrah.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtcxwqnaqg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtilbclpqv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtbykawwng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtpphhslke.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtvzdvtdzq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gtogdlzeit.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtsbtmzyrb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtgdqtnysm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtmpfcjnjd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shanyushiyangtech.top/gtiomtuuqa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gtfssqlfic.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtpgmlgeeb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtrqlbtarm.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtttcpepiz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenzaomai.com/gtvelowlxp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtqmtuomst.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtqnypcgas.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtwdzjuwix.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gtueeojbcw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtsbbftady.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtssmelwpr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtafzxifio.html

[L06] 解析响应为 JSON
来源：http://hz.jqgufenzy.top/gtmtvghjin.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gtqaotlzif.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtxmumbqsf.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtsjyodxmo.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtmfclscad.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gthlvrquuv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtrvkvnvyn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtntlrftib.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.iojbl.cn/gtftuadvms.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtusselxay.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtqlyihgyn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtrehoxjho.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtmfzinmam.html


<!-- 参考信息 -->