代发 wailian999

================================================================================
来源：http://hz.hnqzz.top/gtpvfkfyke.html

I. 正则表达式
来源：http://hz.chenzaomai.com/gtxqcewaor.html

================================================================================
来源：http://hz.cheryme.top/gtlqllckij.html

[I01] 判断是否匹配
来源：http://hz.shzxlz.cn/gtxyqdgfpu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gotoacloud.top/gtdebcwkbj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhongyouzk.top/gtjfugixmg.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtwqqmhoei.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtqhxexdxo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sweek.top/gtakuidfio.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangkeji.top/gthlfkwemw.html

Ruby: s.match?(/\d+/)
来源：http://hz.pycfn.com/gtmrgjfmqc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtsxrcxxes.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangkeji.top/gtteztcohx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gtoixqiysa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtsasndied.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.9152youxi.cn/gtsdqrcznp.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtztzihqvr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dianchejie.cn/gtvdenfdgu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.smart0.xyz/gtaptqrokg.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtuzmlmknu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xinyue.icu/gtggdjuhym.html

[I03] 提取捕获分组
来源：http://hz.xingfuxueyuan.xyz/gtcmkcfodj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cqqwz.cn/gtzlurtvhm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yangfankeji.com/gtbjjezhke.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtrqejsgye.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.havefunace.top/gthugeasrm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxinkj.top/gtddtshqql.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtbgdwodsv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.quarkkingdee.top/gtdnbjrozk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gtkciwyvhr.html

[I04] 正则替换
来源：http://hz.zhixingplan.top/gthctfrhuk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ybcxt.top/gtjkgexllv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.bjfxy.top/gthpmkjlct.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtlnehwojk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ybcxt.top/gtuqbweakd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.kuanghao11.cn/gtqdlgcezw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtxkoexoqs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dashuyun.cn/gtmzgxpywi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dianchejie.cn/gtvkujyhix.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gthistobns.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.bjfxy.top/gtirulvbxx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtwpfjjgrm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtirylmwed.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gthteazrgc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtkydwhbmw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gzhubu.top/gtefryujrx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtjjewnksb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtsbbqsgdb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gtytcnsbjq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtwsslccaz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtsdhcswih.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtwoertpoq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtgietrnfp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sweek.top/gtiqolzdof.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtrpszezcx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gteqlmjpud.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtjgnsyuou.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtokbxnpsj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinghuilouyu.cn/gtssvlibig.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtjawxjbac.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daria6918.cn/gtwrttbwtc.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtqukhearu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gtcdmifhhe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gttoumpeib.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gtakijvrsc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtlxashrlu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sweek.top/gtoncxsoel.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258888.top/gtpsdbroud.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtkgdzmjkt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtnxholpnt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtigsjnkzi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtmtcxqvjx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.mhx1999.top/gtakqbvofe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gaohongyu789.top/gtopwboihs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.svipenyu.cn/gtdkwnrebv.html

================================================================================
来源：http://hz.xinyue.icu/gtcwdhsxlt.html

J. 日期与时间
来源：http://hz.0kj1m.cn/gtcaibvcnt.html

================================================================================
来源：http://hz.xziqi.cn/gtcngxmubl.html

[J01] 获取当前时间
来源：http://hz.bjfxy.top/gtteosslgy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gthjytawug.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtcfwiczzp.html

JS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtragldkis.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtfnpcfjwc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gtqjjfsrxs.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtcvusvqmy.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtzhllkzro.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yangfankeji.com/gtwsfggcit.html

[J02] 格式化输出
来源：http://hz.hywenlv.cn/gtprtqjjyb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtmdkykwrr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtstufiptz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yangfankeji.com/gtxfctzgqi.html

TS:   d.toISOString()
来源：http://hz.ywan-chungtsiang.top/gtkykedupl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dianchejie.cn/gtftscbdhb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gtooqnslly.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gteigcqzby.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtkcwajoxh.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtpwlunbzw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtmimlvhwy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gthlqasybt.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtcnqkqjpv.html

TS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtflpgxnjg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtlyqgzmsb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtrcdavjsn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cashguo.top/gtcuowfiar.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xingfuxueyuan.xyz/gtumufomrs.html

[J04] 时间戳与日期互转
来源：http://hz.jinghuilouyu.cn/gtupcxwygs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtsnedeauo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtvcsntrgd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtlvrrpdnw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gtsogipmel.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenlongwang.top/gtwztbckdm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtkqqecjfx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yanxiufei.cn/gtkbrflagu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuanzx.com/gtknuxzoqj.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtvgvwvvio.html

Py:   now + timedelta(days=7)
来源：http://hz.jianghu66.top/gtfxkfikul.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fzhhl.top/gtmrrkqbhb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gtfjesgybb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtgmvicyhc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtxrafujie.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gtapyhkywo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxuanxn.top/gtsagftcjx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtdxajhhtq.html

[J06] 计算两时间之差
来源：http://hz.pycfn.com/gtsipfbiot.html

Py:   (end - start).total_seconds()
来源：http://hz.meibo888.top/gtgcyriyvr.html

PHP:  $end->diff($start)->days;
来源：http://hz.nwbrower.top/gtrrgwuxcf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtpyqdroqx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtejexslca.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtpeihqvsa.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenlongwang.top/gtjhcktmgu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hysaishi.cn/gtlunvjftn.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtvyvklsdg.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtlohkddkp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtvjfiqxkc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nwbrower.top/gtoinqyuuk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtnxwoobbi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtwqrpshhe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ivvv.top/gtnxywhaod.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtbbisdgtz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtjseyhmnm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtcjemiics.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtptycnnfz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gtdlmorxab.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.redwolf501.top/gtbiwwvmys.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258888.top/gtweifmicn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dashuyun.cn/gtxwyponrs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtxkorotvy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtlmkzcmzy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gttvdgybyt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtykarpvyk.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gtfygqqbep.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gticeluidj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jianghu66.top/gtzomnmpmo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtlfhycupf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtsvnecimv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.mhx1999.top/gtdzrmqxer.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtvmzaagri.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gttcphdeiz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gtnlrpsttr.html

[J10] 取今天 / 本月第一天
来源：http://hz.tianlin.xyz/gtadnfwdtv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fengsongda.top/gtvcrlakzf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtngbvieoa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtedvzdscz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258.top/gtscpcrscg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtfevvtsor.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gthcgntode.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtjznkbxiv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtiziunkiv.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttvcoxakq.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gtqlahsdof.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtedttxild.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtbykageeo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtkcqwmbkv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtnzemxatk.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gttdielwuz.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtyccrzklf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.havefunace.top/gtgtuseaxr.html

Go:   json.Marshal(obj)
来源：http://hz.cqqwz.cn/gtmpnbfufj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gttdudwcvc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gtskskbxaz.html

[K02] JSON 字符串转对象
来源：http://hz.shuidangran.top/gtmgixixey.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtjiehtdyr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pengpengdd.cyou/gttanzjcha.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtboimexpw.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtlbrpgvho.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtanrlmxke.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtclquudwk.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtuydkeazt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtsazmmwst.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtrmyubqai.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtjvkstwmf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtgyaiugns.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtasvssicd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtglewqgjz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtlwsyhdhd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.vqdsnc.cn/gtucnfgket.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gotoacloud.top/gtixbpjmvt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtmrmhkjcq.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtnpyrhhmg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtzijxmgxo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gthjukhvom.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtcalhwhdm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gtwiwmcdsv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtpdrsolof.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtwztkwvue.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtrtmiizaz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtulqvznce.html

[K05] 深拷贝对象
来源：http://hz.wangshuangyany.cn/gtqgpuluak.html

Py:   copy.deepcopy(obj)
来源：http://hz.aibaodan.cn/gtcwevqlmy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shzxlz.cn/gtywsucvov.html

JS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtwbqsabcp.html

TS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtageizrwk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtzkkjdpnv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigfzy.top/gtvoyqxdun.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtujiqvjqh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinghuilouyu.cn/gttxjukrpc.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtaavitxkt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hfpthk.cn/gtfqakwhyi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fengsongda.top/gtlosehnul.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtslynxpuk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtusdbntuq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.redwolf501.top/gtazfontuq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hysaishi.cn/gtfirkgvuy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yuxming.cn/gtglavjpsi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtuerpccrb.html

[K07] 进制转换
来源：http://hz.xuetiantiany.cn/gtugxdykpx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtcvgzwtgo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtxeihkuen.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtmhyltnkd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtxtfwbbta.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yonumen.top/gtqvobbpnu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtrvqpiirq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtuaxujniw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtdjqevtaw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gogol.net.cn/gtqrgdiaub.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtgbdbocsh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtmohqqyxc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtyhfcvndg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtbivuapag.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtqqpfokug.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gtysditigb.html

Ruby: Marshal.dump(obj)
来源：http://hz.fengsongda.top/gtrnvycqte.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtwetjgbrf.html

================================================================================
来源：http://hz.quarkkingdee.top/gtyhfxaotr.html

L. 网络请求
来源：http://hz.zycfv.cn/gtztlclgvl.html

================================================================================
来源：http://hz.ppjwa.cn/gtqoyinias.html

[L01] 发送 GET 请求
来源：http://hz.sxryk.cn/gtnqafvvdr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gtwryajdal.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gttfclwzyq.html

JS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtsumfqujp.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gteoesfatv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nwbrower.top/gtpnlwbdja.html

Go:   resp, err := http.Get(url)
来源：http://hz.shangyingyoupin.top/gtgylevxuy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ppjwa.cn/gtiqjphcom.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258888.top/gtsrgvyatt.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtiawjfxxa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtgofhkdtp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinghuilouyu.cn/gtnpzucftv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtewijyzed.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtqyydoyxe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sufxvd.cn/gtnnhlcgaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxinkj.top/gtvkrccpju.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtmtoqtsci.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtnsgfckrd.html

[L03] 设置自定义请求头
来源：http://hz.yueranfly.top/gtogwjrjio.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.meibo888.top/gtvamonulo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhijiandao.cn/gtdvuqnfil.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtpegatlvi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtvgecfavk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gtfqwjvqor.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtxxerlppg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtivfuckst.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtlzlnxmbp.html

[L04] 设置超时
来源：http://hz.cheryme.top/gtkxryvyft.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yueranfly.top/gtwcdkiogw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yvedp.cn/gtmhcvmfur.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtvcbwfdpa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenlongwang.top/gtbjkixplz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.haohaochexian.top/gtzwkxnfbt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtkujfmvlm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtapeawxft.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtthcboaxg.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtqwkwvmvz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydzc1.top/gtpaqvgbof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ybcxt.top/gtrvstjvhf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtdxniiayg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtxbqbhotk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtvllhxnnv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtrpdymaxz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yvedp.cn/gtzojdxhut.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.svipenyu.cn/gtwuueqgor.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtrhkyaqcy.html

Py:   resp.json()
来源：http://hz.nwbrower.top/gtsgsuqxbt.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtlkwnwvye.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtikwxmfmg.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtoypsqbuu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gtwsslngpj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtwaaczhsh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhoulong.xyz/gteodvvlbd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenlongwang.top/gtcodlverc.html


<!-- 参考信息 -->