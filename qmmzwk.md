代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gtaxjrxjtn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtqdwnlhfh.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtxtwtglxn.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gthpmwilhn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tanke756.top/gtlydkotfr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtzsmkkavf.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtgxmawmpc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtkfeqiuzx.html

[I02] 提取所有匹配
来源：http://hz.ywan-chungtsiang.top/gtevripgpu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtaxiqxouf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gaohongyu789.top/gtsbzzhhjq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxuanxn.top/gtvfzodjsh.html

TS:   s.match(/\d+/g)
来源：http://hz.zhoulong.xyz/gtwbvnodwr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nwbrower.top/gtiqxjvrqk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhiwuduotai.top/gtkfhankew.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gtuihzxyga.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hysaishi.cn/gtbphlhpku.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtxiecvujs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgufenzy.top/gtldzfyuiw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ybcxt.top/gtieohbxhr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tianlin.xyz/gtmygcwfco.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtsezrjmdn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yonumen.top/gtcjebtlza.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtllwwmjnv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtkwxeykrr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigufen.top/gtolgqouvk.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtalwdsify.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtscypxxzm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xingfuxueyuan.xyz/gtsdziuept.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtbogkpnhe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtywfpbwsx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtpyospjuo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinqigfzy.top/gtxvedznmx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinghuilouyu.cn/gtzprntfww.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtiwcafdot.html

[I05] 按正则拆分
来源：http://hz.zhixingplan.top/gtmarkndlj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gttiwovilr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgfzy.top/gtvumryjga.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtofzugnzw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtambneopg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhijiandao.cn/gtnfbkrajo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtxexevfgc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtdiwquvpd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shuidangran.top/gtryjfkcqe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cheryme.top/gtcbpferni.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtdpdqlenu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinqigufen.top/gtqdagmjmb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtvsollxky.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtrrqmztjc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.meibo888.top/gtgltwqcah.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gtqgirfzjm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aizwys.cn/gttzbvrpzo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtpmkrezrf.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtaaumzwqs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtfrezqpwt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yanxiufei.cn/gtxpmpgpdn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnqzz.top/gtabdkkjbi.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gthpnmavqk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtkhuhtbmm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtcvbyodyk.html

Ruby: s.scan(/error/i)
来源：http://hz.andypj.xyz/gtyomumbyq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shuidangran.top/gtlaljeauh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhoulong.xyz/gtxsxpkams.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtgcnogxiu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gtxkqefklk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtqzyxrewi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtndiyjdco.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtqsfqonza.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daria6918.cn/gtnicpiuub.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fzhhl.top/gtzgetagdd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.smart0.xyz/gtkqazxkqh.html

================================================================================
来源：http://hz.iojbl.cn/gtlnwroupd.html

J. 日期与时间
来源：http://hz.yueranfly.top/gtbuebnpus.html

================================================================================
来源：http://hz.vqdsnc.cn/gtglicsmmf.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gthnduwioo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtpdsigkfb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtxzpqbcpq.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtmqxakhxf.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtqcpeimkp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtfztqmtrp.html

Go:   time.Now()
来源：http://hz.sysykeji.top/gtncugmxgv.html

Ruby: Time.now
来源：http://hz.pycfn.com/gthzpkrqzy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtfdpeyohe.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtdajicegd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtjqspmyzi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtbanksvpf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gtrueivfvy.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtljlcnzrj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pycfn.com/gtrbjulmok.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fzhhl.top/gtamipnbmv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtvszrpcuo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtoumpsjku.html

[J03] 字符串解析为日期
来源：http://hz.jinghuilouyu.cn/gttviqunsn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtxvdughtu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtumqnnjgv.html

JS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtbzlglfvw.html

TS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtwjvihyzu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtambbnumi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtjnebcswk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtfihwagyh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangtech.top/gtqncilmwb.html

[J04] 时间戳与日期互转
来源：http://hz.andypj.xyz/gtgakxspja.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yanxiufei.cn/gtymtwyudq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.kuanghao11.cn/gtmfnbpqoj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuanzx.com/gtsnjgylik.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.meibo888.top/gtqmrnccdt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhixingplan.top/gtvjbdjnbi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtybzapxhk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtzlocdurq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gtfrpedvol.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgfzy.top/gtabywfqdn.html

Py:   now + timedelta(days=7)
来源：http://hz.hammf.cn/gtnevlubcg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtqnjbcbxi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtckwayamj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtmimgeuaf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yueranfly.top/gtoqhpemsn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gtkyvmckfn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gtwjkywcht.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtilepayly.html

[J06] 计算两时间之差
来源：http://hz.hongshengwenyu.top/gtqqdbqwvg.html

Py:   (end - start).total_seconds()
来源：http://hz.gaohongyu789.top/gtydenjhte.html

PHP:  $end->diff($start)->days;
来源：http://hz.snrcjt.cn/gtvxyjoygo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gtyyouzwrn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hammf.cn/gtflbcntns.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtksrujvzb.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtugrkxdaq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jianghu66.top/gtofjotiec.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtdjybhrby.html

[J07] 比较两个日期
来源：http://hz.vqdsnc.cn/gthwxirxdk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtdzrzbifo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtczkwaike.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gtlcvflilk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtoscumjbr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shzxlz.cn/gtlxpvxuwk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhijiandao.cn/gtqheiiuby.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtaghzsafv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtvvndoyaq.html

[J08] 提取年月日与星期
来源：http://hz.yuanzhike.top/gtmuxlqnxt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ybcxt.top/gtfkvupjas.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.52xcode.cn/gtfvgosjgx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.0kj1m.cn/gtsbgtasgu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gtkwwmjmza.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtpvivyicb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.andypj.xyz/gtkkpkjbox.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.9152youxi.cn/gtyjdaqxly.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gtpqnzljkn.html

[J09] 时区处理
来源：http://hz.aizwys.cn/gtkwinskmw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenjidiqi.icu/gtkiudsukv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtmqllgmcf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtysdknfcf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtuovbcjdo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hfpthk.cn/gtjvkovipw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shzxlz.cn/gtxuwwqqnz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cashguo.top/gtzuqmweya.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gthriftify.html

[J10] 取今天 / 本月第一天
来源：http://hz.cdnleiting.top/gtzdxsiyep.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dianchejie.cn/gtkbdpgjis.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.meibo888.top/gtosliobdj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtuatbgdmx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtbflfaaow.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtvefbpnfi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gtgrvztpwj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtzeukkmrn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtrdxlqfwz.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtndqqirrf.html

K. JSON 与序列化
来源：http://hz.daria6918.cn/gtcwpynpes.html

================================================================================
来源：http://hz.jianghu66.top/gtjnozprhc.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtbqmcefrh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtffwqmtcq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtdkwogefn.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtalarxmnl.html

TS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtwgxxnszv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ivvv.top/gtbaczgfgk.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtygylxgjo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yangfankeji.com/gtfpycyzyt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gtaaxjskqt.html

[K02] JSON 字符串转对象
来源：http://hz.zycfv.cn/gtzvfqxeqn.html

Py:   json.loads(s)
来源：http://hz.sweek.top/gtkbimwzdb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tianlin.xyz/gtcwoxmggp.html

JS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtzwdpmnyu.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtstyhigcu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtwpwgenso.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtjajdrkny.html

Ruby: JSON.parse(s)
来源：http://hz.dianchejie.cn/gtjffnbifc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ywan-chungtsiang.top/gtpjvberii.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtvgmcqcmw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtvaowizzn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gthtoxnemx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtmmipupeu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtfzxxrgqh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gttliroyxx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtaewlisbx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtueonjxwz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gteuwxwqcx.html

[K04] 读取 JSON 文件
来源：http://hz.iojbl.cn/gtrncyptxc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aizwys.cn/gtwvmlthel.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtmwxovnuf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtxfigbywv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtorqopetm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.feifeiyinyue.top/gtezsqfdcz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gthswscgqw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tianlin.xyz/gtsivcdfgu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gtrzvqelbt.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtxlzvqgnp.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtgwqdlany.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gthbqiputp.html

JS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtjvcewbqs.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtkdajwunx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtkmptzrhv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtqfduawnl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtpqwvxpuw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtdrgatmxk.html

[K06] 解析 URL 查询串
来源：http://hz.zhengqikj.top/gtkmcvsgki.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gtleldhipd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtmhtfnemc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gtbeiheufp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtsntgnupw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhixingplan.top/gtfrlyhrxz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtdbdfaipl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtdgfhigyc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gteujfrqfv.html

[K07] 进制转换
来源：http://hz.cashguo.top/gtmgpdjbed.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gotoacloud.top/gtqcxroflz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtztbifbno.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtktvntejd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtbkupgsam.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtohzgqznx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj202588.top/gtmrempruj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gtvohmbkhr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhijiandao.cn/gtcwgkbitn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtudcfcroi.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gttbygdhvx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtkykvwdvp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gttabmylmf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtyxmicxrv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtithzoqdw.html

Go:   encoding/gob
来源：http://hz.gogol.net.cn/gtvpaahkef.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gtgaxbxpaw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhengqikj.top/gtxikvnmgy.html

================================================================================
来源：http://hz.yangfankeji.com/gtwtvdtjje.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtxxkokjnm.html

================================================================================
来源：http://hz.chenlongwang.top/gtchvtqwuw.html

[L01] 发送 GET 请求
来源：http://hz.shzxlz.cn/gtwgkokuwz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtxuednzgg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtwzrersco.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtwsorzynz.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtqpkrrusy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jiagoushi.top/gtreecnyca.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtunolfgbi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daxiang520.top/gtohpncsab.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtfumgekje.html

[L02] 发送 POST JSON
来源：http://hz.zhiwuduotai.top/gtnewnyqgw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.svipenyu.cn/gtvezbcmjf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nwbrower.top/gtngprjmcs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtmjhsqhti.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtfjfgpqbb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtrbclfjht.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtacjxlubn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtqxnnikaj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtljvjbdoz.html

[L03] 设置自定义请求头
来源：http://hz.bjfxy.top/gtuatctpnn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydzc1.top/gtyhvdjxep.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtzpzcjopw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gturwtxlou.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtmjybbxku.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cheryme.top/gtzmheppnl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtbfkdqlcz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgufenzy.top/gtovfivhpy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtsvqadmyc.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gteymeheix.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sysykeji.top/gtqrzggcvw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ivvv.top/gtonhlflvw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtmhqtggux.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtgdjsqxys.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.wangdashe.top/gtcrzxkfml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtfothrwhi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinghuilouyu.cn/gthtinfszg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gtdzyjmuhi.html

[L05] 上传文件（multipart）
来源：http://hz.mhx1999.top/gtsxphkhwj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.iojbl.cn/gtjujxztvm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtrorbjgdx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gthnlemgkz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtfqjqunoa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuanzhike.top/gtivxvuyet.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtnkyvqdnx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gtgkkojswy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtatyhmhdm.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtzpjuapxb.html

Py:   resp.json()
来源：http://hz.zhongyouzk.top/gtiuignnuh.html

PHP:  json_decode($body, true);
来源：http://hz.ppjwa.cn/gttlfnuijq.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtitryoakg.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtyggacxhy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtsariminn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nwbrower.top/gtsqjkoyrw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.havefunace.top/gtfmqanayd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtlmzzgpgs.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnqzz.top/gttyjlagqy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258.top/gtuwxoepaq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtipkqyawa.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtfkhcrqbs.html


<!-- 参考信息 -->