代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtfhrvacsj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtbehjetxs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtegskmorc.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtvezgejui.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtdjcitnjv.html

[I03] 提取捕获分组
来源：http://hz.jiagoushi.top/gtqgjpfivk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gtzskwvqsg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yvedp.cn/gtwqcdyjei.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ybcxt.top/gtasdibrjx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ybcxt.top/gthdijkzuu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hywenlv.cn/gtkyhpycpq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtixhfuzra.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtxqmgnnjr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gttqbhgfka.html

[I04] 正则替换
来源：http://hz.chenjidiqi.icu/gtatbcvbtd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gttuapklbs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtdqpeflvm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtxgoeyoaq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtdxlajiov.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtqyqpvvkw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtaypcvwej.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtwauwpcty.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hywenlv.cn/gtajnpxkwq.html

[I05] 按正则拆分
来源：http://hz.jqgufenzy.top/gtzpqxwurg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtfcsrlvmm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenzaomai.com/gtcbyudciw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtqrnqegjv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtuqyezdsf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ehwqpu.com/gtodidsate.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtdaqhyrwx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtshutxksf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sxryk.cn/gtjrvticuk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gtlrhfghqh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtzkrboruv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinqigufen.top/gtizmashrq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtlvmbpyby.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtmczymqnr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxuanxn.top/gtylnqdojp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gttpbhowdu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtjvcbegpy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtbcwtkocf.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangshuangyany.cn/gtwezygrnp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhoulong.xyz/gtduujhgpj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtesdrtfrv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtjtbvzcoa.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtgzmbftqo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtpbyfpeya.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtryutmqyu.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtdwbrowlf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shzxlz.cn/gttyhoaeit.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtmshfwvte.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daxiang520.top/gtzravevzt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shzxlz.cn/gteozqjene.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtjfilgbxv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydzc1.top/gtmaylphfd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtjcrvradh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nwbrower.top/gtukzutjgw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gthwpaytcv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtegntlbdl.html

================================================================================
来源：http://hz.tian-w.cn/gtamwuuqkz.html

J. 日期与时间
来源：http://hz.shzxlz.cn/gtyycvrvnc.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjhfmlvdp.html

[J01] 获取当前时间
来源：http://hz.9152youxi.cn/gttwsddmnz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sufxvd.cn/gtzdqccaql.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtupvlvvno.html

JS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtgmmftrcp.html

TS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtmdtpvzkg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtlhwvvkks.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtrzdwdtts.html

Ruby: Time.now
来源：http://hz.chenjidiqi.icu/gtckdombex.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.andypj.xyz/gtsquicurc.html

[J02] 格式化输出
来源：http://hz.chenjidiqi.icu/gtjgtbqttk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtjwmxwllt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtncazgvai.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtclrcjgpx.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtwevygdph.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gteauujuto.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gtwrjjbjdk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtqlurnepc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtcefkvkyp.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtysrbafez.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jianghu66.top/gtxceaiqoy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtbqctrwcq.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtfjgbghwz.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtllezpiww.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtxubkyhmy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtvteunxqq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtmkmemtnv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigufen.top/gtqokogaiw.html

[J04] 时间戳与日期互转
来源：http://hz.ppjwa.cn/gtqonrrpcd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnqzz.top/gtxyduxcll.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gteoohpwnd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangtech.top/gthpdypcpp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtroywyynx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtuzrbayjo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtwbhbiwxg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.andypj.xyz/gtcjoxkldn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtbafyzeok.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtoazewoih.html

Py:   now + timedelta(days=7)
来源：http://hz.zhongyouzk.top/gtzrfyzlcv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtrihacotm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtcjjvysfu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtmdayootj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtsokhpzbd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yueranfly.top/gtinumtjuz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangtech.top/gtcdjgckoq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtelmjsvrb.html

[J06] 计算两时间之差
来源：http://hz.yuanzhike.top/gtnpppuwme.html

Py:   (end - start).total_seconds()
来源：http://hz.bjfxy.top/gtzwxxkdde.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gtvjosgjch.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtxyebatyx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtibhlzcro.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhijiandao.cn/gtqddyzmyy.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtkdzyqllt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fzhhl.top/gtrjxbtsdz.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtohuxuaxk.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gtaouprewz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtcsaaosmv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtflmgvkqg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtyttffmxd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtkeelpqar.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtrkbyrwbq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtnmxfoiyk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtqfbllapl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtozqakxqr.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtkjmonnoq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtxulharsa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aibaodan.cn/gtivhcxjiy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yvedp.cn/gtlzxxkeil.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtzdkfdmlh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtfrrgogxf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258888.top/gtjbiwampo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ybcxt.top/gttrgrsuzy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258888.top/gtssvrviny.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtphmfsntt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jianghu66.top/gtojlbexea.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtwqshojuj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtzhtaltbt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gthmilvxxb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gaohongyu789.top/gtlhqmzaxg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangkeji.top/gtxoactqoe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtxryeomla.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtgrrxohpk.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtrtstbfeh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gtlvdczfkg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtwrhuvvtc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gttmzklbpn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tian-w.cn/gtcikuggry.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtgimpvktc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xylfe.cn/gtlyesclaw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigufen.top/gtvsrzpdts.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gtrvsevnye.html

================================================================================
来源：http://hz.hammf.cn/gtobweymrd.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gtuwvqijly.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjsdmpyvf.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxinkj.top/gtfmyfeyvn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtwfztfkzk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gteufujgsc.html

JS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtvftkznqh.html

TS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gttmhgdluv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cheryme.top/gtasmyfchx.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtwprchnvf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnqzz.top/gthezybygn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pengpengdd.cyou/gtlcvmdypu.html

[K02] JSON 字符串转对象
来源：http://hz.nanxinkj.top/gtuhfadlui.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gttjefgsyy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gtmzlxismy.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtxxggdnwl.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtvdszflvk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtxupqarci.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtsadepbsw.html

Ruby: JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtcoinxkiq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhixingplan.top/gtlcxgqfdp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtpygoygvt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtzuoqprbm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtevvcjooe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtqqojfgvv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtsrsrtkyf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhoulong.xyz/gtrzpqklju.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hysaishi.cn/gtcajunsie.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gthmyorjqh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtjuhymrzt.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtojqgkrxa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cucudq.cn/gtdreqnzkn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuanzhike.top/gtkujzdoyd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtuebydbwv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtjvpebzej.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtfmrfwohg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gteqfyyzmv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258888.top/gtiamsqasl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gtvgejmejq.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtmuzhxswy.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gttbezjqia.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtwattgfvv.html

JS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtrysglkhm.html

TS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtjvqavgoq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtxgmgjyod.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtftkjejos.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.snrcjt.cn/gtgkmosmkw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tanke756.top/gtuhlwwiqr.html

[K06] 解析 URL 查询串
来源：http://hz.ydzc1.top/gtfwrusaug.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtysigqxqn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yonumen.top/gtnkijdpwm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtstajstvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtyjqaezgm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.vqdsnc.cn/gtqubzrxhz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ppjwa.cn/gttrzcppbk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gtynlxvlvl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xylfe.cn/gthlajguna.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtilijjqmc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtjnwuynoe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.smart0.xyz/gtygxxwhjw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtkiyishuo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtvfufbmpk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pycfn.com/gtpjdrlbdx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gtltjjakeg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gtacsncmgw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fzhhl.top/gtzopdwjpm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhongyouzk.top/gtnwidciig.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gtxfzjielx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtnrxuodpa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtbkjzkncl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtxgtucpdx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtfdjbcynn.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtznxstoim.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtbadqthtn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yongpay.top/gtecomcbmj.html

================================================================================
来源：http://hz.zdqjudy.top/gtkidldcpn.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtmlcdnpwl.html

================================================================================
来源：http://hz.52xcode.cn/gtcrfbmaed.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtrzxgsbid.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtcclygtda.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gtgyuuddnr.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gttgbeertn.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtddyaiskr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jyoumei.cn/gtkofampxx.html

Go:   resp, err := http.Get(url)
来源：http://hz.xingfuxueyuan.xyz/gtygnifybf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gtbkpfwglv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sysykeji.top/gtyirameyz.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtlgizwckz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.pycfn.com/gtgckzhacr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtqtayzlwe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtnfzfkylb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtkrhexwjv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj202588.top/gtreypafxu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.iojbl.cn/gtgxkznyzk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gtdxovktfv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yueranfly.top/gtihrashgg.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtinxxdsrw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtruxbglki.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gtscsolywv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtdqbuccbq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtakwyrxkx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zycfv.cn/gtvxddfrfg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtvorjolph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tianlin.xyz/gtxyqucnxm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtzplsoype.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtwbdlpias.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shangyingyoupin.top/gtgumywdia.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jianghu66.top/gtdnqncdnw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtulfkvxmz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gthpufqqpw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtowxzgvye.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnxiangtu.top/gtwcbuocmv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sufxvd.cn/gtmeibxkot.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gtnjmguakr.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtmzvilypw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gtgzmvbicx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sysykeji.top/gtsconbvyg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtvipgjxzs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtvglhokts.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtaxhuxkwd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj20258888.top/gtimmlpmuu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.kuanghao11.cn/gtszgjdjau.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtabpjjnrx.html

[L06] 解析响应为 JSON
来源：http://hz.sysykeji.top/gtzglysgic.html

Py:   resp.json()
来源：http://hz.gaohongyu789.top/gtqswfmrhs.html

PHP:  json_decode($body, true);
来源：http://hz.mhx1999.top/gtnbjiijtp.html

JS:   await resp.json()
来源：http://hz.cqqwz.cn/gtjoxpyjrl.html

TS:   await resp.json()
来源：http://hz.pycfn.com/gtycdeyoov.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgfzy.top/gtytllagzm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.quarkkingdee.top/gtxnuylnbm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtqwyqolnz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtzrrposjw.html

[L07] 处理 HTTP 状态码
来源：http://hz.guowangkeji.top/gtldaczvfw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gogol.net.cn/gtwpzvuies.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtkhdjlhga.html

JS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtpdbfnlsk.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtgrlfukxz.html

Java: resp.statusCode()
来源：http://hz.nwbrower.top/gtafzzqmtk.html

Go:   resp.StatusCode
来源：http://hz.snrcjt.cn/gtijwuxlvx.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtvqtoeleo.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gthdococcj.html

[L08] 并发请求多个地址
来源：http://hz.kuanghao11.cn/gtpbnvnswv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtcguhsgci.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtbzagigcc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtmfttyqrt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtvtoninkm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtrxmzkiin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pengpengdd.cyou/gtvyvusqfw.html


<!-- 参考信息 -->