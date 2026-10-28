代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnqzz.top/gtxdxugxhr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtcixignak.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtwekgrona.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydjk.org.cn/gttnqczmvm.html

[I02] 提取所有匹配
来源：http://hz.zhongyouzk.top/gttziohbfw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtgzbgjzkp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gthzgmijvb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ywan-chungtsiang.top/gttfyhwwks.html

TS:   s.match(/\d+/g)
来源：http://hz.aibaodan.cn/gtmwajbtsg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtoojeuplb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fengsongda.top/gtuzcktwek.html

Ruby: s.scan(/\d+/)
来源：http://hz.pycfn.com/gttggrogto.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenjidiqi.icu/gtbedmikzc.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtbqfkcsoy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jianghu66.top/gttuqlambq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtcbocburq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jianghu66.top/gtqgwncwga.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtnvissgcg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gtvzufegvf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtrmszceps.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gtfakerxbk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gttktchgce.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtrkfsqahw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtohrhzjnl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shangyingyoupin.top/gtpfimcbri.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtkviikutx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtgklitdks.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtsubajfvz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtcckejlta.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtmofudtfh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yonumen.top/gthewttsqj.html

[I05] 按正则拆分
来源：http://hz.svipenyu.cn/gttrykkezz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daria6918.cn/gthwpzyvnb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtqdbxpppj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtxnfgmsjd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtgmlgphjb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gtbnqgijns.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gtteauymlf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtwqdriqrg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtfxfgnshy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtelspnduz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtyswgztfi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxuanxn.top/gtwyiaucrf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtmwvombih.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtyynvuyti.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guowangkeji.top/gtzoxjrixx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtbkdrtefk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258888.top/gtxvbhwfbv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gthlhabdtl.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtwrcsipwp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gtmvfespmy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuetiantiany.cn/gtyzcwargp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.0kj1m.cn/gtlaplrbfb.html

TS:   /error/gim
来源：http://hz.ydzc1.top/gtfaajvtzr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gtontoxzdb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gteakwtwmw.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtyxjuemjw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxinkj.top/gtwzqruufa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtrijcbztv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gogol.net.cn/gtcpxgqksj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtbmsmvhdk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtmqqdreml.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtpmmfqhwc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtxlwrvbzf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gthoabseai.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhaomingkeji.xyz/gtdvosboco.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtxjcmctxp.html

================================================================================
来源：http://hz.xylfe.cn/gtnaiyvkps.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtnpwmhhsk.html

================================================================================
来源：http://hz.9152youxi.cn/gtjefawvhg.html

[J01] 获取当前时间
来源：http://hz.wangshuangyany.cn/gttczkhrxv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtgcrypato.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtlwjbomwo.html

JS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtthyhtinx.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtrkpqzcux.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgfzy.top/gtvtlpqjoa.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtpdcedixx.html

Ruby: Time.now
来源：http://hz.hnxiangtu.top/gthawpmibs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pycfn.com/gtfzpfgwbu.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtzncoqhqk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtstdztyvq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtfbirexxu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgufenzy.top/gtfhyvneql.html

TS:   d.toISOString()
来源：http://hz.yuxming.cn/gtrbyjbgkx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtbcmtofjc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hammf.cn/gtnzusoezg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtxqvjzmtp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtbwsthsts.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtvnumobuc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jiagoushi.top/gtnjtzvvoj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtxdzlalqr.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtwazmpgov.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtilhgyykw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtnbfmhydr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gttepynado.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj202588.top/gtzjdjgwex.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yongpay.top/gttoiuxdwr.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtkzzvxbwc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tanke756.top/gtyqxjnnoc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.9152youxi.cn/gtbesremkf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zycfv.cn/gtksoqibzn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtrajnnaik.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gtpbfkxccq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gtfrirxpyl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxuanxn.top/gtmrusbkws.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtlmgszbdz.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gteqzmymmo.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtcohxusio.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtgipfqnhv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtospahnyq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gtpkjrenbr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtpdeivddw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guowangkeji.top/gtxvabryys.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yanxiufei.cn/gtnssxuvfj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtidngsuui.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtywwuqnsn.html

Py:   (end - start).total_seconds()
来源：http://hz.sxryk.cn/gtteuqhczl.html

PHP:  $end->diff($start)->days;
来源：http://hz.0kj1m.cn/gtyywebyxc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ppjwa.cn/gtsgijntgi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yongpay.top/gtfliakbch.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xziqi.cn/gtnlepxsgp.html

Go:   end.Sub(start).Hours()
来源：http://hz.guowangkeji.top/gtzrnwtecr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gtzjkjyjho.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtheeroojk.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gtfvhosrov.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtexavuyiw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gotoacloud.top/gtvjzhwfsb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtoqyztbzg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gthyvinemq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtablqvbyo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.9152youxi.cn/gtzxzsvyye.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtktkcutfx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtpwuahoyr.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtrvzmixxg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gtrcculkpo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtrdjeszst.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.9152youxi.cn/gtpzcyoras.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtkcokzutn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtxqnrzcsu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yvedp.cn/gtgjjaefct.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gthswykijz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gtxmkkyuis.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtymdmoybh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangshuangyany.cn/gtsuxrhinc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtcnrylyri.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gttrjtjzrx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtrpqtsmet.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gtkspfpgem.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sxryk.cn/gtvebncylz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtixeekzkj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenjidiqi.icu/gtglitmocr.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtjhmsrruz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtxpmkkjyb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shzxlz.cn/gtwpwuwwlw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnqzz.top/gtffauzlxi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtxvbxkqqb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtpbimfiqe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtbzuufqsd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fzhhl.top/gtnkjijryt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fzhhl.top/gtbmshmzgy.html

================================================================================
来源：http://hz.yvedp.cn/gtiqmyovwp.html

K. JSON 与序列化
来源：http://hz.fengsongda.top/gtzgpszrsq.html

================================================================================
来源：http://hz.zdqjudy.top/gtcerkgoyg.html

[K01] 对象转 JSON 字符串
来源：http://hz.meibo888.top/gtfiemrqnn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gttsdjxveq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtewopwtlt.html

JS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtnlfxqcwu.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtoyezlhvg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.redwolf501.top/gtkfepyppy.html

Go:   json.Marshal(obj)
来源：http://hz.sufxvd.cn/gtdryiktgq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ivvv.top/gtmdhsphjs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtqrdkfavl.html

[K02] JSON 字符串转对象
来源：http://hz.xuetiantiany.cn/gthvpaifqd.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtfgkasted.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtduzjswvr.html

JS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtbqcamfjb.html

TS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gthzuhdqli.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtahvfsfyd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtiaddivem.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtynezklvd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dianchejie.cn/gtsxqkjjty.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtqpahwkax.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtgzuzhivv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtxawwbkey.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gthezhctbi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtxcqbvijd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydzc1.top/gtqqssvitl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtcbtuqgxv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtpspfczzq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gthubonlkn.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtoloyhoor.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.316326.xyz/gtiqrkdkyc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhongyouzk.top/gtbdaedydl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtzzpgrtka.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtirmgajln.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtwjmthjih.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtxdbcqcrf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhixingplan.top/gtdykhlqob.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtjedkmaup.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtmmuycntr.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtigmvlcoi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fengsongda.top/gtwtggogvp.html

JS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtgqdownaa.html

TS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtpnhojnlg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtlmoqicki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtjvdueqvv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gtklqjyesf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtnscxkzeq.html

[K06] 解析 URL 查询串
来源：http://hz.sweek.top/gtmnvimmud.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtyhwoirno.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.andypj.xyz/gtkmovbivr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtqlmcdfrp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtzqffycaj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gttcnvqmxw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtcsjsvmyg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgfzy.top/gtcqrlmazz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gtibbnvltz.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gteyseibfa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtaiyycpdq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gtlhzcojjv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gthuhmqqwb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtketakvam.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtotrnpooo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gtorjkooyy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yvedp.cn/gtvdtsydjp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtfvemldtl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daxiang520.top/gtspmnslxl.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtmbtytlga.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.mhx1999.top/gtkjuahuic.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtzjrqgzmj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtbahoeuqd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gteoinbzxq.html

Go:   encoding/gob
来源：http://hz.52xcode.cn/gtwwpbznlr.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gthmckzumw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuanzhike.top/gtylunwqai.html

================================================================================
来源：http://hz.yueranfly.top/gtoqypduxd.html

L. 网络请求
来源：http://hz.cucudq.cn/gtcyxefhed.html

================================================================================
来源：http://hz.jinqigfzy.top/gtuedoidif.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtibqhoqoc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ybcxt.top/gtaexlqlxy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtfthvlrrk.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtqgvwpzxn.html

TS:   await fetch(url)
来源：http://hz.hammf.cn/gtoufbloij.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhengqikj.top/gthncdvtss.html

Go:   resp, err := http.Get(url)
来源：http://hz.havefunace.top/gttqbgnzpg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtgusscecg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtdgnwkagp.html

[L02] 发送 POST JSON
来源：http://hz.jiagoushi.top/gtjdlaqdug.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtdottxhkz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinyuanbaomall.cn/gtbzvgfyfa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtzobplobj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtnvqbjkgv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.316326.xyz/gtdgmlynud.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtngafffmx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gttvbklznr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnxiangtu.top/gtwzrrqjfi.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtmzfarjxr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.bjfxy.top/gtyqndauon.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtzvdczypx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtcdgpbvwq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtswbxsbkb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gaohongyu789.top/gtqxuxmitd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jianghu66.top/gtwxenmecn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.andypj.xyz/gtiurxmeiz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtezicrztc.html

[L04] 设置超时
来源：http://hz.cashguo.top/gtpgjlgvxt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtllifvsux.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hammf.cn/gtvleebvsr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtvdbltwcj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtjfxjvehk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtzojhbodq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zdqjudy.top/gtcxupfewj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtmavijywj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtzaiwcvpt.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gtrmbvepjw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hywenlv.cn/gtzhiijknf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aibaodan.cn/gtoerfevcc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtjywrsflt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtyrlisqez.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xingfuxueyuan.xyz/gtkalovvju.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gtrlagwrxh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtabinvodl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dashuyun.cn/gtnddtlkpd.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gttlxcjjtn.html

Py:   resp.json()
来源：http://hz.wangdashe.top/gtrmzzcths.html

PHP:  json_decode($body, true);
来源：http://hz.xziqi.cn/gtqxhkaxyo.html

JS:   await resp.json()
来源：http://hz.tianlin.xyz/gteztcoysw.html

TS:   await resp.json()
来源：http://hz.bjfxy.top/gtjnybajvj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.kuanghao11.cn/gtasbfubzt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.mhx1999.top/gtxweqywgb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtoepvprvb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangkeji.top/gtutbucamp.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gtjearkokf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtjtpxpkrp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtzgguyofq.html

JS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtqsulnykz.html

TS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtpjokqbjq.html

Java: resp.statusCode()
来源：http://hz.hnxiangtu.top/gtqpsxjfjk.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtbrlfdvux.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gtnzsteqdo.html


<!-- 参考信息 -->