代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtbltadpkp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtegqlvctx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtxrvdyzwq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cashguo.top/gtoymbxors.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtcqaieyka.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gtdstblipu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtjnybuvpm.html

[I05] 按正则拆分
来源：http://hz.yangfankeji.com/gtyxilfbss.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pycfn.com/gtrgllfxgs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgfzy.top/gtptjdizqc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtxjlezaht.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gthvoiafuz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xingfuxueyuan.xyz/gtnznviyla.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shuidangran.top/gtrylzlfpn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtnwvbvsuh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtudwizvab.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtdmszfawz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtljypkgvp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shangyingyoupin.top/gtnlhprqqu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtbjmntfrs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gthgvmxsfu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sysykeji.top/gtqqbhfjcq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gtuvymzzez.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dashuyun.cn/gtoxocneuk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gturmwvinb.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtfbzvznav.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtsvdnludu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtacnmrlrf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pycfn.com/gtypzvwulf.html

TS:   /error/gim
来源：http://hz.tanke756.top/gtnuugxwlu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangtech.top/gtldoefuax.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.feifeiyinyue.top/gtlhymzbji.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gtlscpzupx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shuidangran.top/gtnkqubofa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtnvynblxj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtswbxrmtb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gttitamdky.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtwsccyzps.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtzyelprrj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gzhubu.top/gtvvdgakli.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cqqwz.cn/gtgwtmvazq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gttcffisje.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jianghu66.top/gtowydddiu.html

================================================================================
来源：http://hz.shzxlz.cn/gtzuywftki.html

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gtdjaukccx.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrctdvqmv.html

[J01] 获取当前时间
来源：http://hz.gotoacloud.top/gtemuafeke.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yvedp.cn/gtvcasopkr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gttcuthqhk.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtcteonwim.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gttcqyznzl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sufxvd.cn/gtkyysewzo.html

Go:   time.Now()
来源：http://hz.chenjidiqi.icu/gtzkydhwrd.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtieihjbfk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtvsrwcqau.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtztfqootw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtagrmdgvq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtsvhaocjm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtzpuxqkci.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtkqdbocmj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yongpay.top/gtrcxxskgh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtnaxpsqly.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtoxgdcase.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guannengcc.top/gtukyzneef.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtilpuzurx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtrpfbubpt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtudergkdc.html

JS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtdgrwjbpu.html

TS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtskgylmmv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtvwjkkvln.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtdwdnhfzm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtskaogcce.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gttkdzfizp.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258888.top/gtiwldmdgw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ybcxt.top/gtvpsvffta.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gtqytngwlc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dianchejie.cn/gtjwrejeiw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtdvziwfuq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gthcplnccf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnqzz.top/gtbffdanzd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtrtsuiddi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtsbbzowcy.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtjvxwixmh.html

Py:   now + timedelta(days=7)
来源：http://hz.xuetiantiany.cn/gtqdkevhrd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hammf.cn/gttzssvldo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gttvaglqxn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtlhbhnpxo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guannengcc.top/gtvdrkcvno.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigfzy.top/gtquysuoxv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fzhhl.top/gtkcbzvfrr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtscicwqtp.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtjfpmizrv.html

Py:   (end - start).total_seconds()
来源：http://hz.quarkkingdee.top/gthkzcrogr.html

PHP:  $end->diff($start)->days;
来源：http://hz.fengsongda.top/gtslrkdelp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtxjyogvzn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.meibo888.top/gtyvefchhs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtgrejdjfe.html

Go:   end.Sub(start).Hours()
来源：http://hz.nwbrower.top/gtrdsbmguz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gthavcjvzw.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gtnanvttfi.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gtxhpqxrzd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtqvtglxvg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtppiqiman.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtremyynut.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtcdbqecte.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.0kj1m.cn/gtuwhjbzyj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxuanxn.top/gtvoethswg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gttnskierc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtjxvqcyya.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gthrtxhyhx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtbqqydsxd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtjfagetus.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtwwzwjyme.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gttslahpou.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtgoonilhy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yangfankeji.com/gtrcmrsers.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtmsqhrpks.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gtzqmodrit.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtuventwyl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtgbcqxufg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shangyingyoupin.top/gtolbayxxp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtzsramvqs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtradfpvti.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gtjggwrnpe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtgctweolc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtgpxnlkhe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.mhx1999.top/gtthprozrp.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gtocnunfvo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daria6918.cn/gtaifqwvbk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nwbrower.top/gttigzbaza.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtesxtexpj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gttsvrcyzb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtkqkjgasl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtnghwgzbt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuetiantiany.cn/gtrpkqwxav.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtokxspjnt.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpkctubfi.html

K. JSON 与序列化
来源：http://hz.gotoacloud.top/gtnmajaxgh.html

================================================================================
来源：http://hz.hnqzz.top/gtgfrosdau.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenjidiqi.icu/gtgvkqztxy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtpgkzljnz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtmmyjsjrt.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtktrlflvf.html

TS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtjekbnhhk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pengpengdd.cyou/gtjwurxeuj.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtguntngwr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sysykeji.top/gtfdzlhoju.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtwamifohf.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtnvephftj.html

Py:   json.loads(s)
来源：http://hz.cashguo.top/gthdmpyzeb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.kuanghao11.cn/gtsmjdhjkq.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtjtitwdzl.html

TS:   JSON.parse(s)
来源：http://hz.hammf.cn/gtqygijwri.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtgdyivhym.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtihkrzubp.html

Ruby: JSON.parse(s)
来源：http://hz.hnqzz.top/gtscatzuhe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxinkj.top/gtjseogmmx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangshuangyany.cn/gthvgyzdjd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuanzx.com/gtoaarrdjm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtnmldjjtg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtbmrnzgca.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtjgbqhfsd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.redwolf501.top/gtnhkelogn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtdvfhjlbv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtlhuejrgd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtqswhivlf.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtooupvrzw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtseyswonv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuanzx.com/gtsffkvryl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtiryqcojj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gttdvmftgq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gtlfvfwztu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtucxjzfxb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.svipenyu.cn/gtljwrfqdb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtgvjxdkbu.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtmlwlkgzs.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtkwbpcclb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gtewztqfwd.html

JS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gthmkrvrxg.html

TS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtwxzhwccp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtvdqbpfil.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtucoflazj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jianghu66.top/gtmwdqssze.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tian-w.cn/gtfhygfbcs.html

[K06] 解析 URL 查询串
来源：http://hz.zhiwuduotai.top/gtzzcvrkus.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gtpwtawqfo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nwbrower.top/gtnswrqlpw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtudyqehfk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtvgcvlaxz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jianghu66.top/gtvwusrjhn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daria6918.cn/gtvefekbig.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtcgmkbtfh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtmjpsdefl.html

[K07] 进制转换
来源：http://hz.52xcode.cn/gturlkonqy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.bjfxy.top/gtpkstdnxx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.vqdsnc.cn/gtjywrzkso.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtqkzhmnjg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtkosatgrr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtlebjakjg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtjlzvczde.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinghuilouyu.cn/gtsgkgwpzy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtjraxeoou.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtsyreaejg.html

Py:   pickle.dumps(obj)
来源：http://hz.birdmap.top/gtqevlwuns.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gticyyyqit.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtpgqltqjc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtvjffneae.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.c1oappe.top/gtnlobnuhe.html

Go:   encoding/gob
来源：http://hz.ydzc1.top/gtkbqfgvtu.html

Ruby: Marshal.dump(obj)
来源：http://hz.iojbl.cn/gtaflluzht.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtvfiebavd.html

================================================================================
来源：http://hz.iojbl.cn/gtcwfqkjoa.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtjnzacqfd.html

================================================================================
来源：http://hz.mhx1999.top/gtvxolltur.html

[L01] 发送 GET 请求
来源：http://hz.smart0.xyz/gtqmaqjqwy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtyoouhurc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gzhubu.top/gtnhtuzday.html

JS:   await fetch(url)
来源：http://hz.ehwqpu.com/gtqeoqmmgl.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtgozgdoas.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtfjsyykyt.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtccaanmxq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtbhhkiitg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtdguwwuuh.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtgdejczmd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.birdmap.top/gtcgjicbjy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtlozqzzep.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtcptbcehi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtnukyshmi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gtffhvvdtv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zycfv.cn/gtfwikatud.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zycfv.cn/gtiwbvpgyj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yangfankeji.com/gtfcglyfgc.html

[L03] 设置自定义请求头
来源：http://hz.hfpthk.cn/gtbftbhgfd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtribyepdb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hysaishi.cn/gtuedxgwpy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtfsqtzptk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtgsfqbczh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtpbnafbpp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangdashe.top/gtchbvmzov.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtzwbpapop.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtjwabczax.html

[L04] 设置超时
来源：http://hz.jinghuilouyu.cn/gtefapolcy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtpozlomyd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtzpgmvyej.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtvpsvrgjf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtiljabqmt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtbvalfauk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtbqgaoyfn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtvfuvkfdt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gtgyvckbhu.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtpaasnpci.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtyyxtreqm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtcsuqiews.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gtkajidwwz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtbyeurtpq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gtahggfldf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gtibkqngxy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gtxycjoeri.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtvrinwtfz.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtobexmnkg.html

Py:   resp.json()
来源：http://hz.chenzaomai.com/gtnmdjsocl.html

PHP:  json_decode($body, true);
来源：http://hz.xziqi.cn/gtrkpmuoyz.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtgtaccdoo.html

TS:   await resp.json()
来源：http://hz.xylfe.cn/gtjlbocbhb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.havefunace.top/gtihwfytdl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangshuangyany.cn/gtfwhbkdvs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hongshengwenyu.top/gtxvxvyzsr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jianghu66.top/gtrlkmatby.html

[L07] 处理 HTTP 状态码
来源：http://hz.316326.xyz/gtxngfucrj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gtqeydznbk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cashguo.top/gtqivtvyup.html

JS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtzczziubg.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gturlvahek.html

Java: resp.statusCode()
来源：http://hz.jinqigfzy.top/gtenysptov.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtmmjuokde.html

Ruby: resp.code.to_i
来源：http://hz.yuanzhike.top/gtptbuxqsp.html

C#:   (int)resp.StatusCode
来源：http://hz.sxryk.cn/gthiejspih.html

[L08] 并发请求多个地址
来源：http://hz.zhixingplan.top/gtiseqkesv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nwbrower.top/gtwgubbskv.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtlmvrawzb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtbptlyjxu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtqoanrulz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtzhmbfisd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnqzz.top/gtdivwkhtq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtwbmqiiwy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ybcxt.top/gtfnmqbmar.html

================================================================================
来源：http://hz.dianchejie.cn/gtrbqsctjd.html

M. 命令行 / 进程 / 环境
来源：http://hz.svipenyu.cn/gtnsrdpgen.html

================================================================================
来源：http://hz.jyoumei.cn/gtvgafvibw.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gteyuqrfqp.html

Py:   sys.argv[1:]
来源：http://hz.jyoumei.cn/gtfksdugsz.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtkolirosw.html

JS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtyvmrxdxi.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtptfemzbe.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtwlzbvbap.html

Go:   os.Args[1:]
来源：http://hz.yj202588.top/gtombsvxyr.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtlxkmysak.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtmsvevqol.html

[M02] 读取环境变量
来源：http://hz.xziqi.cn/gtxgnvdcgv.html

Py:   os.environ.get("HOME")
来源：http://hz.bjfxy.top/gtkkiaiwdy.html


<!-- 参考信息 -->