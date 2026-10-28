代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ppjwa.cn/gtupjdqnmu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gtfktzjiic.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtdnxlesdj.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtodkevyyc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtvuawcnnt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtpsuaqmrp.html

Ruby: s.match?(/\d+/)
来源：http://hz.gaohongyu789.top/gthjazyseq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yueranfly.top/gtcuvwipnh.html

[I02] 提取所有匹配
来源：http://hz.svipenyu.cn/gtbufuxizi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cucudq.cn/gtmfvcsfar.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtpvfwiwzn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yanxiufei.cn/gtecvprpqj.html

TS:   s.match(/\d+/g)
来源：http://hz.gogol.net.cn/gtlpzhxznw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtgakhkjfd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fengsongda.top/gtyhoqtxdu.html

Ruby: s.scan(/\d+/)
来源：http://hz.9152youxi.cn/gtafcacnnj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.dianchejie.cn/gtpajyktca.html

[I03] 提取捕获分组
来源：http://hz.ydjk.org.cn/gtbikjpwff.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jiagoushi.top/gtkxifgxcx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gtbeqsswft.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhoulong.xyz/gtmstvhqmw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtgudzldzx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtasicarga.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtudvrfxkh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtkedqtaos.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.bjfxy.top/gtsawnxuhx.html

[I04] 正则替换
来源：http://hz.ehwqpu.com/gtsvwdraca.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigufen.top/gtldukrouf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtlnwilkls.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtsasdpgbt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtuqbqedqe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sufxvd.cn/gtmknzgmvz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtspatqcbf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuxming.cn/gtlbaticbf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtmdulioeu.html

[I05] 按正则拆分
来源：http://hz.yangfankeji.com/gthnykyrli.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gtqmdrgjqc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guannengcc.top/gtviifswub.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtvnckhfiq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtsgkkjzqv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhengqikj.top/gtoxzpdljt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.mhx1999.top/gtzczzrdsy.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtqxhnccam.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yonumen.top/gtjrnqxvng.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.bjfxy.top/gtddlecuvf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gthuqgjssm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtkwaqndcs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtcwehvdud.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtdlxvszcv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shangyingyoupin.top/gtdpzbutlk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtcirqgpgw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtzbdywzoz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtfucouwgw.html

[I07] 忽略大小写与多行模式
来源：http://hz.sysykeji.top/gtmylnyjmm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hywenlv.cn/gtjewzspgy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gtcrldijxv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.birdmap.top/gtxrngimol.html

TS:   /error/gim
来源：http://hz.snrcjt.cn/gtfpqmeffo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aizwys.cn/gtlbndqrrg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.andypj.xyz/gtvbphjxks.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtucuuttma.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhoulong.xyz/gtwosgikrr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtjzlqtwth.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenlongwang.top/gthzpjzzkl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jiagoushi.top/gtrmlzgych.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtiarnmbep.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtlztitbqn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258.top/gtylypyubj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangdashe.top/gtllciqlop.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtkknqylok.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.iojbl.cn/gthpmvzyul.html

================================================================================
来源：http://hz.cheryme.top/gtbtpqbkhs.html

J. 日期与时间
来源：http://hz.cqqwz.cn/gtfgiielzi.html

================================================================================
来源：http://hz.chenzaomai.com/gtwbjkecif.html

[J01] 获取当前时间
来源：http://hz.yj202588.top/gtdvuyyaym.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yangfankeji.com/gtanxqomzq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtmuwbsrwu.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtubtfrbsb.html

TS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtvbbyhwuo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtfqbynssp.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtrjnvuppg.html

Ruby: Time.now
来源：http://hz.zhijiandao.cn/gtodnatfkl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtytdluegv.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtwolimrkw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtlkzzfuar.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gtvgvqmqut.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtcitykfan.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtqbmkljop.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtxiipsqeh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cdnleiting.top/gtldouzgkt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtoagzzlqj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ybcxt.top/gtgqrnxjel.html

[J03] 字符串解析为日期
来源：http://hz.cdnleiting.top/gtixckqzlg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gthavjscqq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shangyingyoupin.top/gtnwihnktq.html

JS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtliiqtnjo.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtkriprflm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtapzgbucd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.redwolf501.top/gtjaawtrqv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtoffejknq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hywenlv.cn/gtzpdigfyk.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gttqzpxsve.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yonumen.top/gtowjziany.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtoxoxcrhr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cucudq.cn/gtqliezrzp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ywan-chungtsiang.top/gtrvtnwaec.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gtqnfucugl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtcqplmbpa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtmhoczywn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gteqkxntjw.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtqopziqkg.html

Py:   now + timedelta(days=7)
来源：http://hz.zhixingplan.top/gtzjtevgcq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gthsqppxzt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtyjewpyne.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtognvkutt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fengsongda.top/gtzoznsfkt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtbmyucgcq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.vqdsnc.cn/gtxtadzgua.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tian-w.cn/gtyukuohgu.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gtddpujmkn.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtvcrehhcl.html

PHP:  $end->diff($start)->days;
来源：http://hz.yanxiufei.cn/gthvruqolr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daxiang520.top/gtoinzpkhf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gtbxncvwbe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gtemsjcpdv.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtcuuatmna.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gthmxmzrwf.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtjqnjgrtj.html

[J07] 比较两个日期
来源：http://hz.9152youxi.cn/gtvvwgtvwj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtjhxxsnja.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtkgzcdojf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtwwbecsuo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtcrkamwrn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.vqdsnc.cn/gtbpuzoeyk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dianchejie.cn/gtkikutcyw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtduehofwj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtbpjsuonr.html

[J08] 提取年月日与星期
来源：http://hz.sysykeji.top/gtgctqlkek.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.andypj.xyz/gtrjkmvkkb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtdiheznca.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtemblskuw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtqqbhbaic.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtzjbdeirc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtvgfosjpu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtrrpzhqcm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtycfbewrq.html

[J09] 时区处理
来源：http://hz.havefunace.top/gthlngrkeg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtsezeqcbp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtmxxxdesl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtxluijlex.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtaxvgaufw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenzaomai.com/gtxntmlqjo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtnygpxnol.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.smart0.xyz/gtoeuzdkop.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xinyue.icu/gtnmkujxot.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtzwayvzhq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnxiangtu.top/gtuafkjvmj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gtumfooytg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.haohaochexian.top/gtetwnlyqq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtgnenzfcp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gttrutozjg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.smart0.xyz/gtygenpvlz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtgrtdzjbb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.iojbl.cn/gtxgvzgsze.html

================================================================================
来源：http://hz.guowangkeji.top/gtdutzdxsx.html

K. JSON 与序列化
来源：http://hz.tianlin.xyz/gtgfdahtfl.html

================================================================================
来源：http://hz.smart0.xyz/gtfoobuzij.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtxjulgtts.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtlrmlggom.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nwbrower.top/gtpzmbrpcd.html

JS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtnwzhybhm.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtkrvubtxi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtbphvnmos.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtygohijwi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fzhhl.top/gtabawvwhh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gzhubu.top/gtsnmrbejz.html

[K02] JSON 字符串转对象
来源：http://hz.zhiwuduotai.top/gtldigffeo.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gttcesotqt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtynajscwz.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtnmfxruzm.html

TS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtkvndhvdg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtyxtgvpyy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtoehlojwy.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtulnughum.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgufenzy.top/gtrocaeien.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.iojbl.cn/gtmuuzusbl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtbxlfnwjt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtdscplcly.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtyleceley.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtmpqoujsd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydzc1.top/gtingadguv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtbgihucun.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daxiang520.top/gtamgxhxbq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gtepwstbon.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtuyisvyih.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangdashe.top/gtvivsaopl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtxyyrpssp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtmfuwzanp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtguwmsvjr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258.top/gtosikgtil.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gttkcsngyv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zdqjudy.top/gtpxeitoly.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gtjjwbrusj.html

[K05] 深拷贝对象
来源：http://hz.yanxiufei.cn/gtslouqzgv.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtwfbxcxjx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xinyue.icu/gtppdghxze.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gteqxhfwvf.html

TS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtjwxvbelj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinyuanbaomall.cn/gtjsaqavkh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jiagoushi.top/gtxnvoosui.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtxbaacdtz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gthtinltrz.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gtiaksbfdq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258.top/gtnafxqrpo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtisojsohs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtsotasbin.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtlsptnnet.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhiwuduotai.top/gtxasuicry.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sweek.top/gtlyuazsrx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.quarkkingdee.top/gtyukzqeom.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtkardwdab.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtwecjahkq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gthogurhdg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.snrcjt.cn/gtxhrezjev.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtghojcels.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtvgkalffn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtoafdgyri.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtguaroggs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydjk.org.cn/gthfdphgzx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtbtwvqfga.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtsevspaih.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtedypzcpx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtzxtnvsfo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtjhbcehvm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtvzjgzvdx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtdsnobzdm.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtyovqzxaz.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtrycjsfex.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtffzrhaji.html

================================================================================
来源：http://hz.jqgufenzy.top/gtyzoghfiu.html

L. 网络请求
来源：http://hz.sysykeji.top/gtrxbmdgcf.html

================================================================================
来源：http://hz.chenlongwang.top/gtdzscclrs.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtfeuadooj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangtech.top/gtqxguuhtk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtzpdztkbm.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtiydahkul.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtcawljicx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuanzhike.top/gtfpsqsult.html

Go:   resp, err := http.Get(url)
来源：http://hz.hammf.cn/gthhfxwmtd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj202588.top/gtafcpacuu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jiagoushi.top/gtieohezda.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtgmfyesxq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtxjbitnik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.quarkkingdee.top/gtictdfnqv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtblidwrxy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtrorpytdv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cdnleiting.top/gtiodsowpb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtgwloeonb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtstrfimdo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gtxigkblgv.html

[L03] 设置自定义请求头
来源：http://hz.xinyue.icu/gtwxgnhhtg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gtxcpnyrlr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuxming.cn/gtvylnooot.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtscxeltna.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtzfzewqdc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aibaodan.cn/gtszgexqnq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtmjprvxow.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtqldkmnsr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gteeximjum.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtdoattams.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtxhjdimlf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtzyfdwqqp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtmvfozsnd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtwudavdlf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtsxghdvoq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.bjfxy.top/gtidcvbbfy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtlfvmqbna.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtcxeelgdu.html

[L05] 上传文件（multipart）
来源：http://hz.redwolf501.top/gtehlpxmhl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtdqrnqwnw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gtthemzltb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtwjdtsolr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtpmdcenkq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtmbdpsvle.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ehwqpu.com/gtmlrtxaxt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtrykzvnmz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangtech.top/gtxqkvrkqk.html

[L06] 解析响应为 JSON
来源：http://hz.316326.xyz/gtjvuwxtps.html

Py:   resp.json()
来源：http://hz.yonumen.top/gttpfhyhyd.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gttimcqyso.html

JS:   await resp.json()
来源：http://hz.ehwqpu.com/gthitdekfy.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtuahlabam.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gthnwfpuzh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gtwnarxgvw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ybcxt.top/gtdgvkzphx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gtaferbati.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtvctcqefj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtebonmosf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigfzy.top/gtmegxgpsq.html

JS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtjgqqymfk.html


<!-- 参考信息 -->