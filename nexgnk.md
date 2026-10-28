代发 wailian999

================================================================================
来源：http://hz.sysykeji.top/gtaktnnuei.html

I. 正则表达式
来源：http://hz.hywenlv.cn/gtkwxpnvov.html

================================================================================
来源：http://hz.tianlin.xyz/gtutdgfzyp.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gtslyglytj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.quarkkingdee.top/gttdfmmyzb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtzfxjdzps.html

JS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtqonofylj.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtuolsgmdb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sxryk.cn/gtmwttrdgz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtgcknozir.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtqgbvsvuj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtwiamsuqt.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtprsheyxg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.0kj1m.cn/gtliwviata.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinyuanbaomall.cn/gtuoyliioz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtomhqsmcu.html

TS:   s.match(/\d+/g)
来源：http://hz.yanxiufei.cn/gtprkrmqow.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yanxiufei.cn/gtixeepyjn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtkfohqasr.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtpfafaamo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuetiantiany.cn/gtnhntyfvh.html

[I03] 提取捕获分组
来源：http://hz.cdnleiting.top/gtzmyfiklr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.52xcode.cn/gtqiguurxz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sxryk.cn/gtxyhhiucj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtdpfkskuo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ehwqpu.com/gtqjtrjvsd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guowangkeji.top/gtzxibsrkv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtsdeaaxku.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tanke756.top/gtfpgbiswj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtozvgxton.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtejoaaccn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daria6918.cn/gtvtjarpst.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtejlpbgnr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtagcuuhhq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtydapwrga.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gttipicneh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtnncnjpzb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtebirtlaa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dianchejie.cn/gtxhwfayft.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtiyvckajy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhaomingkeji.xyz/gtcwsdlery.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yonumen.top/gtdjwunglk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtgusoncpi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtbugphhoy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gtegfvaziw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yonumen.top/gttxnympcv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtvknmxuwm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.mhx1999.top/gtiacyuabc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gttsrpvtym.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtkmzptque.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtqouyighq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtaadnefzw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtidsiapbj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jiagoushi.top/gtilypflqg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtyxeumjrp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtoauylekf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtkogzvgxf.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhijiandao.cn/gtunwlkfhf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtfrylwhir.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yongpay.top/gtsgfhesot.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aibaodan.cn/gtguiaqtju.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtkzdjmyvk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gtijyflhsu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.havefunace.top/gtdqsefres.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gtqfcfbmrj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daxiang520.top/gtkcdfjidt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gttlcwekjl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258.top/gtvkmallea.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxuanxn.top/gteqykdnks.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtqykbibdx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtndhybqld.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenzaomai.com/gtwfymwxah.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtopjfqldk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtzrcvlpxz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtwlhdarln.html

================================================================================
来源：http://hz.hnqzz.top/gtryyyerct.html

J. 日期与时间
来源：http://hz.cheryme.top/gtoydjrtys.html

================================================================================
来源：http://hz.ivvv.top/gtpoztoukr.html

[J01] 获取当前时间
来源：http://hz.wangdashe.top/gtsynxcwcr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.0kj1m.cn/gtvqzymltw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtyqhgqwhc.html

JS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtpskhbyvs.html

TS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtpqiipawn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhaomingkeji.xyz/gtrwfxzqyc.html

Go:   time.Now()
来源：http://hz.gotoacloud.top/gtushsmnwr.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtvllwyysq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yonumen.top/gtmkgbdzxm.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtrekuiblb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtsskajkbt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtjmungvdx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtjznkketp.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtaeilsyvz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenjidiqi.icu/gtqfqdijcd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtdzgsfvci.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtmlabyuas.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtqgqaahyw.html

[J03] 字符串解析为日期
来源：http://hz.zhengqikj.top/gtcjoppdei.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtkypnqqtw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gtalnttwqg.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtvqerbeoh.html

TS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtttvonumy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gthdrpspfy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtsriimhem.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gttboqluni.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhaomingkeji.xyz/gtthrtakja.html

[J04] 时间戳与日期互转
来源：http://hz.hywenlv.cn/gtngujlctq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangshuangyany.cn/gtrludcidp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.kuanghao11.cn/gtvhtpfnrj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gthzmtwhgm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtmmaxxwyo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hongshengwenyu.top/gtsmmrugut.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shangyingyoupin.top/gtengoeutj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtkvtqylnj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gtepuavhpp.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtbnozqtty.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtsgplinip.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yangfankeji.com/gtvbrzzvcb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtvchfmqxa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gttcrjckpg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtzenjvorg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.andypj.xyz/gtroqbktub.html

Ruby: Time.now + 7 * 86400
来源：http://hz.vqdsnc.cn/gtvfgoycvg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ywan-chungtsiang.top/gtgfnlstyp.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtvnzchrel.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangtech.top/gtgoffpdrp.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtuuvbgvde.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtlzqkqjpw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guannengcc.top/gtiukmamtx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aizwys.cn/gtwuepliqk.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtewniituj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtdmqawpex.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtvewxzdzm.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtvnifalej.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtlotxcsgw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.9152youxi.cn/gtceqrnxmn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtwslklhdj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtwonyjbjl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.haohaochexian.top/gtlfjwacli.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtxvyyeexz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtnatatsid.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtppnjvcrq.html

[J08] 提取年月日与星期
来源：http://hz.xingfuxueyuan.xyz/gtcrzozclk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shuidangran.top/gtjerocele.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtaldhidcx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gtdohskbgh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtghicbrgu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.redwolf501.top/gtxktapqor.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtzsbhizci.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shzxlz.cn/gtdnapzlyo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtjkcgunfa.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtjnwwrksw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtnbbbsrik.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.svipenyu.cn/gtazrmfiws.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gtadppmqfp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtvlezzezm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gtiaogpdhc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jianghu66.top/gtjqragpvv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ywan-chungtsiang.top/gtulufdepc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xinyue.icu/gtnkmoiqmt.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtsgthrkjq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtercpyxzq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtysrxgaga.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gthxipaach.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhaomingkeji.xyz/gtwyloeelt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtgiotvbes.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtbaldnfft.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtiagrsaze.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gzhubu.top/gtrmtzmdrd.html

================================================================================
来源：http://hz.gaohongyu789.top/gtjlyagcfw.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gturjqnrpl.html

================================================================================
来源：http://hz.52xcode.cn/gtxpzwkzdq.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtdvzygwwb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtteziuguv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtshdpreqw.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtkxokkotd.html

TS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtkgcgmicj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydjk.org.cn/gtwssifbyy.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtmxbxbvtg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtqgfmmnvv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtoecbpgrq.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtfwlsxqnd.html

Py:   json.loads(s)
来源：http://hz.jqgufenzy.top/gtfglmwynj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ppjwa.cn/gtsksezcwg.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtrcskrffe.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtbsxanmce.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtyvuaynyz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gttffnqzht.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtyvwfdydc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jyoumei.cn/gtdpyvkecz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gteajmyqgt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.birdmap.top/gtmdkhivfe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtrqvhejdb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtbjvkjnjg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtoizkixvk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtwsvnrhzf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xinyue.icu/gtmjlxwvbd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigfzy.top/gtubbznrto.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtgqcqlaac.html

[K04] 读取 JSON 文件
来源：http://hz.ydzc1.top/gtrqokhjei.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtciubexaf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gttmektafw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtpvntonqm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtibitrpif.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gtiwlkauoe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtvznkcfqo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtzxopsvpb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gttsvqztyx.html

[K05] 深拷贝对象
来源：http://hz.hammf.cn/gtlbqcaqhj.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigufen.top/gtareoxbvc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtawmskkpl.html

JS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtuvevbbjz.html

TS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtlpgnkrfr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhixingplan.top/gtzpprybme.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pycfn.com/gttnkxnzyg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aibaodan.cn/gtitamqlwc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangshuangyany.cn/gtnoniwqhc.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gtxhlgwfxv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtpbcrinrm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydjk.org.cn/gtgjmzgoxs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtjrgnpqas.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtphwcvjsi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pengpengdd.cyou/gtkoupypnu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ehwqpu.com/gtwabmaxed.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtccurdbem.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gtvbqqzjez.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtgkhywepv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtheoeunqk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigfzy.top/gtcdpbkweg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtcjvvxsix.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtwftrnbss.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtbtufnlgk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cucudq.cn/gtbunuijuh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.0kj1m.cn/gtohlrlewg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangshuangyany.cn/gtsjzlnrrh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtqqzdmekd.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtxzlvtkee.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtdojfxsay.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtenevneyv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtcvwsikdj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gogol.net.cn/gtmmnpfysa.html

Go:   encoding/gob
来源：http://hz.xuanzx.com/gtotgcojao.html

Ruby: Marshal.dump(obj)
来源：http://hz.sweek.top/gteknmousg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gtzsywnedk.html

================================================================================
来源：http://hz.xylfe.cn/gtgdkkjjwn.html

L. 网络请求
来源：http://hz.bjfxy.top/gtquyufins.html

================================================================================
来源：http://hz.yj202588.top/gtqecpmphz.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtmklbxnpj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtghpmakdh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtqegdanyy.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtwpdvmtwx.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtzihfkqtm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtdpyxivcn.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangkeji.top/gtwcooxzus.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtzxmlfwir.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtibpgieoo.html

[L02] 发送 POST JSON
来源：http://hz.yonumen.top/gtixbwpzec.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yueranfly.top/gtnhiqnpvq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shangyingyoupin.top/gtchaoubmp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtmnnskhct.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtmxsjuced.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtzixtyekj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtnmcxrxyi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtqigvbpmo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtwgqaleik.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtlypjilsi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtnzjmcvoz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hysaishi.cn/gtgigrpvms.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtybyjedvt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtezqaqvml.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gthgpdsbsn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtocuwlljc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtbzbjwhva.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtjdhssuzy.html

[L04] 设置超时
来源：http://hz.shzxlz.cn/gtqfmtriin.html

Py:   requests.get(url, timeout=5)
来源：http://hz.snrcjt.cn/gtkvgjumir.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.52xcode.cn/gtncmnkxiw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtmikyhvue.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtzmssrcle.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangshuangyany.cn/gtfyvoraor.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhiwuduotai.top/gteajibzjm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gthxxfraev.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtybyxdpow.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtvyjtgyli.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sxryk.cn/gtkkghsxbd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sufxvd.cn/gtyzkwlrpc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gttlyhkrls.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtgbqmwuov.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydzc1.top/gtyqezqbee.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sufxvd.cn/gtprrlirfd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtebggvprc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtqkrblpui.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtgkjuqkip.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtzujpcagv.html

PHP:  json_decode($body, true);
来源：http://hz.52xcode.cn/gtdipoaijq.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtkewszvti.html

TS:   await resp.json()
来源：http://hz.cheryme.top/gtmldmhnvj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangtech.top/gtlniqmnsu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtlpnxkjch.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yvedp.cn/gtabcamvej.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xziqi.cn/gtezddgzbz.html


<!-- 参考信息 -->