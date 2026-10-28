代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenlongwang.top/gtkiwkpeti.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuxming.cn/gtfbkbxfce.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtqhyncgef.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtjvftbmug.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gtuaysjdsu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtqiisafkr.html

Ruby: s.match?(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtaulvkpjy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtpmmtyulo.html

[I02] 提取所有匹配
来源：http://hz.ehwqpu.com/gtddvlhgxe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtnjxhqfhu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtntcuihfh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtagpfswuz.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gthfwdtsls.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtpwgpzpgo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtdcqvjitn.html

Ruby: s.scan(/\d+/)
来源：http://hz.yanxiufei.cn/gtbucyzmta.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.havefunace.top/gtiofkpsyc.html

[I03] 提取捕获分组
来源：http://hz.hfpthk.cn/gtbrtbvdri.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gaohongyu789.top/gtbuflunve.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.bjfxy.top/gtpidjqgyq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtbypuyyer.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ehwqpu.com/gtqgyhevhb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gthdloznmr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtzulpgvhm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtucifnutn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cdnleiting.top/gtamqdydum.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtndgqnjzw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtybfizahm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aibaodan.cn/gtufqlxgzf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtihxjdoat.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtxijtgsir.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtxynhrugz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tianlin.xyz/gtjsxwoeim.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hongshengwenyu.top/gtsixyzbzj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigufen.top/gtfxwqvaao.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gtjdggogxq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangtech.top/gtacbmcngi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.9152youxi.cn/gtueuiupxw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gttfjmmlej.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtspftewvm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gtxfpudexz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gtytdoziqw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gthzauaqgq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gtqmtriuzd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yvedp.cn/gttyhudrfy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtbydpsbst.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cashguo.top/gtamikipml.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtoxgrnhcw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtqknjzkxm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sufxvd.cn/gtgtqiqrxb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtkjtodcuf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jiagoushi.top/gtvgtlrekf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtryeohpdc.html

[I07] 忽略大小写与多行模式
来源：http://hz.pycfn.com/gtfevecmhb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yangfankeji.com/gthfhtfpwu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gtxkuopmpt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gttpmhzljm.html

TS:   /error/gim
来源：http://hz.yj20258.top/gtmxqxbgav.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtjvnwqvfn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gtprebmyup.html

Ruby: s.scan(/error/i)
来源：http://hz.daxiang520.top/gtswiohgvk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgfzy.top/gtibjxhfct.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtoiaufnwl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtdzmozejn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtpnmfvrxf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtrmieldhl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtzrciribk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtblkbnzct.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtruasqwbd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtknewyfok.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtpcxyuobv.html

================================================================================
来源：http://hz.yongpay.top/gtjzrzduas.html

J. 日期与时间
来源：http://hz.wangdashe.top/gtkehcqaso.html

================================================================================
来源：http://hz.sysykeji.top/gtlmajjpvc.html

[J01] 获取当前时间
来源：http://hz.52xcode.cn/gtfuqejrcs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tanke756.top/gtjkgfggxa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtabpvxxyf.html

JS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gteajsybos.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gttgxlabve.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtlfsngbtx.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gtclayhyiu.html

Ruby: Time.now
来源：http://hz.pengpengdd.cyou/gtoesavnlm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.feifeiyinyue.top/gtzwfhsdzv.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtzucjpdgs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtrvvoujng.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtjevvxicq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aizwys.cn/gtridnhblw.html

TS:   d.toISOString()
来源：http://hz.316326.xyz/gtilxshmbe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtcjxohgoj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jianghu66.top/gtjurfzcem.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtjoxqfimm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.fzhhl.top/gtzebyycdh.html

[J03] 字符串解析为日期
来源：http://hz.iojbl.cn/gtqxacppmc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnxiangtu.top/gtgaiopjuc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtaxjgtprs.html

JS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtcldfbjtc.html

TS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtpnpchtyt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtvicopizw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtnsrjzpbg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtyracexuh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtulrxwnos.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtgxrrsyav.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj202588.top/gtucvqpobe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangdashe.top/gtyltxroxz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yangfankeji.com/gtnvvgqszr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtnktlcopd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gteeqaamvr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtanwlexbo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtfqkgjyld.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtufuejtwf.html

[J05] 时间加减（加 7 天）
来源：http://hz.mhx1999.top/gtggydquao.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtyybqyryu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinqigfzy.top/gtbiafjmgd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtyeqjnbbu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtppvjqkxk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gtgxxcmsqn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gtpfgcqqyh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtegyjswnd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yongpay.top/gtmpgnzcxs.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtotknrxhd.html

Py:   (end - start).total_seconds()
来源：http://hz.tianlin.xyz/gtuzovnpox.html

PHP:  $end->diff($start)->days;
来源：http://hz.kuanghao11.cn/gtpqyixenb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gthsbxtfji.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtqnxryqgc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shangyingyoupin.top/gtyybkppyu.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtmwoswkwk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtwlzcaczn.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtwwdopxnl.html

[J07] 比较两个日期
来源：http://hz.xuanzx.com/gtpbisntgt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtplphaohi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtvzrzjsjg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtxaltuflx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtpmtxiqsj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtrqjqsjyt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtkzuwgsfv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtnfrzyulj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtylkpixkd.html

[J08] 提取年月日与星期
来源：http://hz.ybcxt.top/gtczdlfgca.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtmwcsogns.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtlyhpqmgx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cdnleiting.top/gtkdkzaqqd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.snrcjt.cn/gtzpcjjiwx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.9152youxi.cn/gtmvhyvvni.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtwzjtoczl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtukznddrj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gteqabvswa.html

[J09] 时区处理
来源：http://hz.zhixingplan.top/gtaiukkpcw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gtxbtcusla.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gtliiyhoxq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtldiuwneu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtnrwfukgw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tian-w.cn/gtefgtsjzu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtxnlhvhhi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtohzdfuba.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gtdlitdigf.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuetiantiany.cn/gtmmifrvjj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtzliskscu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtatkoyfdm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtisdnkujh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtoebwuacg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtnfkitdhm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.daxiang520.top/gtmhphptof.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtylfzbion.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtawvahzmx.html

================================================================================
来源：http://hz.yanxiufei.cn/gthkiiywwc.html

K. JSON 与序列化
来源：http://hz.pengpengdd.cyou/gtsjgfylsn.html

================================================================================
来源：http://hz.haohaochexian.top/gtsassnryy.html

[K01] 对象转 JSON 字符串
来源：http://hz.52xcode.cn/gtbnpjyspf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuanzx.com/gtytzahlzz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtriepixfc.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtcieqzqii.html

TS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtykiyqkjm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangshuangyany.cn/gtubwanpzv.html

Go:   json.Marshal(obj)
来源：http://hz.chenlongwang.top/gtjyiqvqxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gzhubu.top/gtbgxcptxo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtihkmcsmx.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtmwvjhtcn.html

Py:   json.loads(s)
来源：http://hz.hnqzz.top/gtffpujcwn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtjmrxeaot.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtsykklqjz.html

TS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtwbdwobbg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhijiandao.cn/gtwprfkwje.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tianlin.xyz/gtxyalhtds.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtdqwidqtg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gtzyaslyxw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gtqvgxnwna.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuanzx.com/gtkbrhmsjg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtgqaorhub.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtndtckdmm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtevbkpqot.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtpurlczhq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuetiantiany.cn/gtytdkrocy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gttflxksua.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtdhsjtefw.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtndgvazhk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtfbzlhwff.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jyoumei.cn/gtdtmgxyaa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtexahpxff.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtsgdqmzmn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtcochlnnr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtorfzoucd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.52xcode.cn/gtasupqdhj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtedsmzxqw.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtgzlkvkpr.html

Py:   copy.deepcopy(obj)
来源：http://hz.pycfn.com/gtrpytltwz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtalurzhod.html

JS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtmlmdogau.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtclcgkeqh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtyihkkdey.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtzbbapwwg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fzhhl.top/gtamkpcqsd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtqkhijsve.html

[K06] 解析 URL 查询串
来源：http://hz.pycfn.com/gtlxjkeaem.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gtohgikkep.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtyaudczmg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtboqgxyzf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtdwwqffpx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtuildwiwc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtgpplopro.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtteoxbnvm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.316326.xyz/gttzyvgsai.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gtolmocbkx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gtwwfdfqbg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtxoqyistd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtrrnepcoo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtvwxiwckz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtinbxgmpb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhongyouzk.top/gtkbqpwtiy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuanzhike.top/gtajevsbwl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtzmjwawbs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gttmuljdah.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gtolsiyppt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.kuanghao11.cn/gttksenbra.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtriwbbyco.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtkbyxqsnb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtegdtnbrz.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtzvkewazt.html

Ruby: Marshal.dump(obj)
来源：http://hz.gaohongyu789.top/gteydztfhi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtsxftuhzu.html

================================================================================
来源：http://hz.dianchejie.cn/gtfhokxukm.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtvjebmdmh.html

================================================================================
来源：http://hz.aibaodan.cn/gtjdndnhnq.html

[L01] 发送 GET 请求
来源：http://hz.ehwqpu.com/gtobaofekh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gttwkeedjv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gtixuejceq.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gtvgruhigo.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gthfnupibw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtbelacksg.html

Go:   resp, err := http.Get(url)
来源：http://hz.haohaochexian.top/gtxnilkxjn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnqzz.top/gtjhsszryi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pycfn.com/gtalszvihp.html

[L02] 发送 POST JSON
来源：http://hz.daxiang520.top/gtyvawurel.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtlcvrbvvw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dashuyun.cn/gttvncspbq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtgwnazzoy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtmtnwuruf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtpdhjhxyl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtcbdhnclr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinghuilouyu.cn/gtnxgwskry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtkvuchlud.html

[L03] 设置自定义请求头
来源：http://hz.kuanghao11.cn/gtgrtmaitl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtjczyvsfp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtuhvzvgbo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gtwbbvlmxi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtzhhfxnjn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pycfn.com/gtlxyhksie.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xziqi.cn/gtncelbrrg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gttfqwzucw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtckksrmis.html

[L04] 设置超时
来源：http://hz.zdqjudy.top/gtsqxerbij.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxinkj.top/gtensjdbao.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hfpthk.cn/gtdxwuqcep.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtmqaibnru.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtnjhostsq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hammf.cn/gtodphkego.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtywwjlwrr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.svipenyu.cn/gteknhydti.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ppjwa.cn/gtcrkdyjpm.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gtrrkdbsrn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gtxmdqupfr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtclxjsbji.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtewxumrcv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtcqazyglp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtdqefabch.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.mhx1999.top/gtkbdavfjm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhoulong.xyz/gthrzmylyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnqzz.top/gttuwrqajl.html

[L06] 解析响应为 JSON
来源：http://hz.ydjk.org.cn/gtatytahzb.html

Py:   resp.json()
来源：http://hz.nanxuanxn.top/gthkywbsjh.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtwjnfhzeg.html

JS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtdbnoydnc.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtpolgqfey.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtpqdldohn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtaeggfjyi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtmrhzbrfg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zycfv.cn/gtgavphkdg.html

[L07] 处理 HTTP 状态码
来源：http://hz.yvedp.cn/gtumlgljns.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gtgxuctuen.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nwbrower.top/gttmsngkdc.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtfvriacia.html


<!-- 参考信息 -->