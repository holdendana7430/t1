代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenlongwang.top/gtnwqbsmfo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtiviitsfd.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtcyeymevt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxinkj.top/gttkxlpwsj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.bjfxy.top/gtengtwpvi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtwzhqlbux.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtnthystwd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gtccmvzzzo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgufenzy.top/gtqlwmqfre.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tian-w.cn/gtybgpsrez.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtxuetmmle.html

[I05] 按正则拆分
来源：http://hz.snrcjt.cn/gtkwtcvwhi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gtsxufnwij.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuanzhike.top/gthmxvdyzs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtcdjrytfd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtcgclrkty.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gaohongyu789.top/gtprqarxhs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shangyingyoupin.top/gtgnzelyly.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtkfyyqgur.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtbbrspqvv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtipgcwlqu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtdmexnxbn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtshplfgdo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtyfrudwjm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtqrsnmita.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtzfvmfobl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gtzlefsocu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuetiantiany.cn/gtgtjjgbhy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtbuonmbby.html

[I07] 忽略大小写与多行模式
来源：http://hz.daria6918.cn/gteujabgzm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258.top/gtmfgwfedy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgfzy.top/gttgefuyvs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gtpdgtqwgp.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtzzngqouz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yanxiufei.cn/gtssfjunnx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhoulong.xyz/gtlcznbyde.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtlgcxzxrb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtttnugqmq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtsygvvyjm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtmvoijysq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tian-w.cn/gtczicfkef.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtucjafuky.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtyzbgnjdk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydzc1.top/gtxwzxetcw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtcrwboisj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.andypj.xyz/gtlngvzzrs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gteiiecvzn.html

================================================================================
来源：http://hz.yj202588.top/gtyxxwcfwc.html

J. 日期与时间
来源：http://hz.chenlongwang.top/gtecdwitlo.html

================================================================================
来源：http://hz.9152youxi.cn/gtjijyfalc.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtrcfynowf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangshuangyany.cn/gtnetjfojy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gtezsldyto.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtsjbbmkar.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtbnxocrzz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtjvnxgcfr.html

Go:   time.Now()
来源：http://hz.gogol.net.cn/gtnreultjw.html

Ruby: Time.now
来源：http://hz.wangshuangyany.cn/gtjlhelzhe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtfhsmfufv.html

[J02] 格式化输出
来源：http://hz.ehwqpu.com/gtfiunpgyv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtitnjqqgi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtlwrwebec.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigufen.top/gtftgooxbk.html

TS:   d.toISOString()
来源：http://hz.svipenyu.cn/gtekybiqhv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtuwtkalzb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cdnleiting.top/gtbuesznfp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtamihdcah.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtaqbrxayp.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtouimetjo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtznevxkck.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gtojjilsjv.html

JS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtoxerczcf.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtxplpbnzz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtrvyoowef.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ivvv.top/gtuopzeguo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gthxcppird.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtsxdrtaov.html

[J04] 时间戳与日期互转
来源：http://hz.c1oappe.top/gtthmqrmtp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gttlahrxtr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gttpecgcrz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.vqdsnc.cn/gtfmsoakwb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yangfankeji.com/gtlftozfcy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gzhubu.top/gtiehcykgs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtcdoxegsp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daria6918.cn/gttcavruhe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtjczeojkq.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtsyyixxhs.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtcklmsdwz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258888.top/gthtcucogf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtshjuyxmj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtoppscxyd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuanzx.com/gtabytwmmf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtgxfqiask.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gtdzxljcdc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jianghu66.top/gtruyghzyf.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtoidzagxh.html

Py:   (end - start).total_seconds()
来源：http://hz.316326.xyz/gteccdmkob.html

PHP:  $end->diff($start)->days;
来源：http://hz.snrcjt.cn/gtgmfxqvks.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgfzy.top/gtqqewuinu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tianlin.xyz/gtqqtdmfxu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtznsnepyp.html

Go:   end.Sub(start).Hours()
来源：http://hz.jlsjyb.cn/gtjgjwgoat.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ehwqpu.com/gtiqoamdsy.html

C#:   (end - start).TotalSeconds
来源：http://hz.gotoacloud.top/gtlzivwpuf.html

[J07] 比较两个日期
来源：http://hz.kuanghao11.cn/gtaxgzzsun.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtmhojjlbb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gturngxgrp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtxqczxeeq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtagpzccim.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cheryme.top/gtylvbyjxa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtquafnmfo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtcjoyhcdq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtmvqndqnf.html

[J08] 提取年月日与星期
来源：http://hz.jqgufenzy.top/gtrjxgurrx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jianghu66.top/gtmsgnnzzj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtdxhotevr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuanzhike.top/gtmwrjzcaj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtsmpdwlfw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtvrinqajh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.0kj1m.cn/gtburszjqd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gtkstndtns.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.0kj1m.cn/gtnosieqcz.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtexlrwghw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuanzhike.top/gtpjqqajih.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.bjfxy.top/gtxbzjbydb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtcymjmgnk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtugxlkljc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtjswbagry.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yuxming.cn/gtmrnrrjyy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gttbiaihqf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtiyobuxdx.html

[J10] 取今天 / 本月第一天
来源：http://hz.gotoacloud.top/gtkhfxonfm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtjuvdfqda.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xylfe.cn/gtmateyqff.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghu66.top/gtxjpiytso.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gtqseiezir.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtqqltxogg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtirmouwms.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aibaodan.cn/gtkeyiposo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.316326.xyz/gtweizqfzl.html

================================================================================
来源：http://hz.hywenlv.cn/gtfsgmtwgm.html

K. JSON 与序列化
来源：http://hz.zhaomingkeji.xyz/gtzzapzwxy.html

================================================================================
来源：http://hz.svipenyu.cn/gtiddowmwx.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtmapiqmnr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtocqhvfwu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtmifotzhw.html

JS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtpnhshcda.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtwyjxaphb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ppjwa.cn/gtpxjfbzua.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtanqjatlk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yueranfly.top/gtpzouswte.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tianlin.xyz/gtknqcbzzs.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtkpmoivgn.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtmvrzrcbn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtvxpmyyeq.html

JS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtbwmuodts.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gthdgkhbxh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtehtuibwd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtemdsmuqe.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtsejkvzjf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtywzsugwl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ehwqpu.com/gtlcxkaveq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtfqqzzegv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtimyxgzan.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtjfoeehjc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtgfnjjxex.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gtjccdsjbg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhongyouzk.top/gtqxjypdlf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtidrfqebs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gtgtlxkdzh.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtwahthmkp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtwecpeqal.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtfgjieuoo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtzgjugwvo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtshsfvtxn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtbgkgaupz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtitmrftff.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sufxvd.cn/gtfifdgsbf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yanxiufei.cn/gtmtcfvnax.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtheseoipl.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtlxtmuffr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtydquuqwa.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtqfizylvu.html

TS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtggklpnah.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.snrcjt.cn/gtjiajbnps.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtbrgsikgu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtyasesfla.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tian-w.cn/gthjzxhqmz.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gtjtougyox.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtugdpchhe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.bjfxy.top/gtzsoyqxvu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtykwgtakj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtesniarnu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gtmdluvmwc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gttoraxixz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gogol.net.cn/gtmbfdmmwu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gtiptpuxmj.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtairbaynx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gteqsqyucz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtvrcvyuov.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtbakenmch.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtjhdgvifg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtkpuqowqs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtasfvaglv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jianghu66.top/gtneeerljv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gtjhedabse.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gtzvcdpukd.html

Py:   pickle.dumps(obj)
来源：http://hz.vqdsnc.cn/gtgmcdwsvh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gtnqtcyani.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtjwfqopqf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtvswwtxzc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtyfgavyen.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtfqrgsjpm.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtoouoscef.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hammf.cn/gtcircqwio.html

================================================================================
来源：http://hz.yueranfly.top/gtqwxrscas.html

L. 网络请求
来源：http://hz.yj20258.top/gtkkwhqwwv.html

================================================================================
来源：http://hz.zycfv.cn/gtsrtgvaul.html

[L01] 发送 GET 请求
来源：http://hz.9152youxi.cn/gtzmpiicdq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.snrcjt.cn/gtndmhnkwa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tanke756.top/gturjhljys.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtqooprlft.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtuqppiene.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtqmnocsru.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtphzvbmoo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangdashe.top/gtpocessde.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fengsongda.top/gtrhvavkdw.html

[L02] 发送 POST JSON
来源：http://hz.feifeiyinyue.top/gtrykxmubu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tianlin.xyz/gtrmczuolh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258888.top/gtmisdfdhy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtspeujyub.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtqboyzoio.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aizwys.cn/gtioueefcp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtwwjmozjf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.iojbl.cn/gthwuzuato.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenzaomai.com/gtfrvqvxvl.html

[L03] 设置自定义请求头
来源：http://hz.jianghu66.top/gtnjzktxsz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtrdchdurc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtdodrakzw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtcqmbgywx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gtferjqatt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhoulong.xyz/gtzujocsfv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtcoawkvtv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yongpay.top/gtmzwfmvjg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daria6918.cn/gtoztnhzqg.html

[L04] 设置超时
来源：http://hz.zycfv.cn/gttymgfcvc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtihgdlvxn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gtcdmdyhgp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtqzdzzthn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gttooupxgg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtuumodjtg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.redwolf501.top/gtcehkymkc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fengsongda.top/gtuozdwnze.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtkiklmpdw.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtrbeympju.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtvliyjmxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nwbrower.top/gtvpqurfdm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtkjtpqivf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gtqpkprgfe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cashguo.top/gtawfnzzpx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhongyouzk.top/gtjkhgixwj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtadipybfh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shzxlz.cn/gtckehxngc.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtmskvweoj.html

Py:   resp.json()
来源：http://hz.gzhubu.top/gtaonovnex.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtljagqvke.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtucuuzogw.html

TS:   await resp.json()
来源：http://hz.nanxinkj.top/gtbfmrypox.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tianlin.xyz/gthrojhevv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shzxlz.cn/gtrtngkqww.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtqohkrpvi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gthrtllkcz.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtxvuvplzn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtpqasxcuh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cashguo.top/gtbersvctq.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtbwhiyiua.html

TS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtouvkirlq.html

Java: resp.statusCode()
来源：http://hz.0kj1m.cn/gtknaswnrx.html

Go:   resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtrvqgcjnk.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtylxpsgzg.html

C#:   (int)resp.StatusCode
来源：http://hz.yangfankeji.com/gtkgxerlxm.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtjpjqugpj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtviwzvjjz.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinyuanbaomall.cn/gtoswpgyzm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtcivkvfca.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtawfwxjcd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.52xcode.cn/gtircdoopn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.svipenyu.cn/gtbhsouqgk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pengpengdd.cyou/gtnuedjezc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtbivcdule.html

================================================================================
来源：http://hz.tanke756.top/gtiqypujcx.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gtfwxfbmzo.html

================================================================================
来源：http://hz.jiagoushi.top/gtacdkktdn.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtgrwqclna.html

Py:   sys.argv[1:]
来源：http://hz.fengsongda.top/gtefpdrljz.html

PHP:  $argv;  $argc;
来源：http://hz.hfpthk.cn/gtorrluxix.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtrtayljft.html

TS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtorwpmadw.html

Java: args 数组（main 方法参数）
来源：http://hz.cucudq.cn/gtongzqybf.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtdwocfyqg.html


<!-- 参考信息 -->