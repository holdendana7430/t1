代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gtvokbhulr.html

[I03] 提取捕获分组
来源：http://hz.52xcode.cn/gtibbuxxqd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gotoacloud.top/gtdmhdydno.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sysykeji.top/gtrddhwhip.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jianghu66.top/gtvlgiaroc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jyoumei.cn/gtukvwriww.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtefumhbej.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yuxming.cn/gtfjxxjvvw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuetiantiany.cn/gtbtwtfdur.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtnektrnge.html

[I04] 正则替换
来源：http://hz.zhengqikj.top/gtafaxgdbs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gtujfiwxer.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haohaochexian.top/gtmgqczbhk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.daria6918.cn/gtsrdujtah.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtjmyzrwnj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtseqorufg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gaohongyu789.top/gtguqiurhm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtbcutwcbe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhengqikj.top/gtpwttthtu.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtpeppchhw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgufenzy.top/gtwcuteqbi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtifzztibh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gthzsdsotr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtdjulqfdi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtmdtyrrkz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.svipenyu.cn/gttgtoiyrx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtbxdufepw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ybcxt.top/gtodfqhfco.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgfzy.top/gtasztzmqu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtsreamfdz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtndgvldsc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtqpwlmibp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtayxhtivj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtgqvkcrsu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.quarkkingdee.top/gtxuvndhsy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtpjsabvym.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtfdvhjhne.html

[I07] 忽略大小写与多行模式
来源：http://hz.meibo888.top/gtsironltm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tian-w.cn/gtylgvfhmy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtrbhywmxs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.9152youxi.cn/gtijjuninn.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtuimiyprv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtfaetkied.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtjidjjesb.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtximtwhah.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuanzx.com/gtbbnuefsn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.meibo888.top/gthkjgbkad.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhoulong.xyz/gthrpmklbn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtzvpuzxrk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtbueadylq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtjdyiqywj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.52xcode.cn/gtvscnjfty.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.meibo888.top/gtxbdbelak.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtfpxgtvzx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtmnntuaie.html

================================================================================
来源：http://hz.jqgufenzy.top/gterfrqhqn.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtbyxmqjfe.html

================================================================================
来源：http://hz.cqqwz.cn/gtaknzhmyf.html

[J01] 获取当前时间
来源：http://hz.chenjidiqi.icu/gtlmxaouez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xinyue.icu/gtyeelbgou.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtcnnkzpuf.html

JS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gthfauyvaa.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtukwvfaat.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtkzdpgnph.html

Go:   time.Now()
来源：http://hz.9152youxi.cn/gtmmreybtl.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtswccphvc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ppjwa.cn/gttgqvvjcl.html

[J02] 格式化输出
来源：http://hz.nanxinkj.top/gtcqcvqmqv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gtppkgjzfp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtakzibzuk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtdjcdoyvj.html

TS:   d.toISOString()
来源：http://hz.zhixingplan.top/gtedddetsq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtbbbnurtc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gtemamotfp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtiivijljf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtsxjaflcq.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtzatjfgcj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dashuyun.cn/gthvifwewj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuanzhike.top/gtwrwtoqen.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtlwytmmim.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtdgvafecc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtimqebmha.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtiqafkaip.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtamrgjffm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pengpengdd.cyou/gtxyundlvu.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtywhvrbin.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cqqwz.cn/gtpsfizvoq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtnizpoile.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hammf.cn/gtijxlucna.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gteravpdsy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtirrvydxz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtsxdlnqxh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtmmfzttlc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gthvsydzmz.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtkbbtmsie.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtompjpbmy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.meibo888.top/gtevshzajm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gturmmkbte.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtuleodpaq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtehxasdyc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sxryk.cn/gtnqxtggjs.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtsthlkinh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aizwys.cn/gtplynjotk.html

[J06] 计算两时间之差
来源：http://hz.mhx1999.top/gtfxmnpzkv.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtxckthnqx.html

PHP:  $end->diff($start)->days;
来源：http://hz.yueranfly.top/gtuxdcnryz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gttkfkgyhg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtukfxayzf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtmkfkaynw.html

Go:   end.Sub(start).Hours()
来源：http://hz.hongshengwenyu.top/gtcdkxdxvu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtdyriralz.html

C#:   (end - start).TotalSeconds
来源：http://hz.daxiang520.top/gtfcrjbora.html

[J07] 比较两个日期
来源：http://hz.cashguo.top/gtooeyvhfp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtdfptbyid.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.9152youxi.cn/gtwkoxagpg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtojpsuerx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gthtujyrzv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtbsiwuxxw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtaqqgjgfc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtnlusstgm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtjljgzgiy.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtrnahhyqp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtkncrpzvk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258.top/gtdohjnjhi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cqqwz.cn/gtgohvhjte.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtbtkoobnl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtvdktuvkz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.vqdsnc.cn/gtojnysgca.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtcdvppbve.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtfilzbtpq.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtlbhmknnb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xinyue.icu/gtiszfglij.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gtydrdugxj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtbqtluebg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtlizcceck.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sysykeji.top/gtctprgmvj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtrhnjvyhn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtlnkutcqo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.meibo888.top/gtbbkwphoq.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtxgkipwoy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sufxvd.cn/gtpcvzzdnp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hysaishi.cn/gtfjbibkmg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtezrgxgis.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinyuanbaomall.cn/gtiycnbqji.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhongyouzk.top/gtzzlrdasd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtrtirzatk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenzaomai.com/gtszecdbzk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gthdfrhubb.html

================================================================================
来源：http://hz.cucudq.cn/gtjwrttriw.html

K. JSON 与序列化
来源：http://hz.ybcxt.top/gtgryhnqyg.html

================================================================================
来源：http://hz.gotoacloud.top/gtvnpworzd.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangdashe.top/gttvtjzyaw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtckpzxvrc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtragxvjnu.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gthbxihndw.html

TS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtqtpnrgsn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtvxnlpgpa.html

Go:   json.Marshal(obj)
来源：http://hz.xylfe.cn/gtjunckekv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtnlbcwlxy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtabsjlbvy.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtylbmbmhg.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtnmiifyhw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aibaodan.cn/gtgebiqxeo.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtvlgocnyc.html

TS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtxjzhdagu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gtqmbajean.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gttyttspws.html

Ruby: JSON.parse(s)
来源：http://hz.hnxiangtu.top/gthvjriveu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtmwpmtrdj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtfvaikejd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtnszvgjxj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gteonxxspq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtpsqkmnep.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtjnhtyzoa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgufenzy.top/gtyljnrarh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtrukbuzec.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinyuanbaomall.cn/gtrwxigcgy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daxiang520.top/gtkgeudidp.html

[K04] 读取 JSON 文件
来源：http://hz.aizwys.cn/gtalnhghbr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtqztgivsy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtxxkyljpu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gthdrwcdqj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtkilqmoer.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtgvfgnrzc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtfwvzzwre.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtzfffxijn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.svipenyu.cn/gtrjqiebjb.html

[K05] 深拷贝对象
来源：http://hz.nanxuanxn.top/gtqrwugeav.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtfekvoral.html

PHP:  unserialize(serialize($obj));
来源：http://hz.0kj1m.cn/gtfchuxssw.html

JS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtegvhwhwc.html

TS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtmylzhciy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtyjzjnxxv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.meibo888.top/gtesklaxsk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtedndrtuk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtudypyzri.html

[K06] 解析 URL 查询串
来源：http://hz.zhengqikj.top/gtqsiayrxf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.vqdsnc.cn/gtkhmldpxj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aibaodan.cn/gtgtpyuggs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtpbahzjdd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuetiantiany.cn/gttzoyqmru.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yangfankeji.com/gtqsdslmci.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtnwiykabl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtkzzrdoeq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenzaomai.com/gtdfqroxzf.html

[K07] 进制转换
来源：http://hz.yj20258.top/gteexelybd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yuxming.cn/gtyxttvptv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gogol.net.cn/gtcywiwcfd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtzzfjduik.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtpbpiivgj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtutpqzjde.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gtuibkmqfc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.redwolf501.top/gtgtnnscjb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtjbbnpxxq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj202588.top/gtyahznljo.html

Py:   pickle.dumps(obj)
来源：http://hz.jiagoushi.top/gtlxcvukez.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtomgagruw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtcycrxvqz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtmbjngmxy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zycfv.cn/gtjhbhexiq.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gticaupwgg.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtwtnjswpz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gttlebfryk.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtqkixgrlc.html

L. 网络请求
来源：http://hz.guowangkeji.top/gtzextgaox.html

================================================================================
来源：http://hz.chenlongwang.top/gtabqtodod.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gtbsvyzqgk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtwnqjwvbl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtduorgqnn.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtjsqdetac.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtameabffj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigufen.top/gtamsoyfis.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtxlzzjyqx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtntcberjs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gtnirrwcyq.html

[L02] 发送 POST JSON
来源：http://hz.havefunace.top/gtnfhkppxh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.havefunace.top/gtwiclomkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yvedp.cn/gtrryrdrxc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtujqrzlip.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtlmwzwgmz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.9152youxi.cn/gtfaoifona.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtxvavyhfm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pycfn.com/gtpgnwcfai.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pengpengdd.cyou/gtcvxqerqp.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtouwrbufg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.vqdsnc.cn/gtwjwlgytl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.kuanghao11.cn/gttldayuvs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtpnekutxn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtrcohpfaa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.meibo888.top/gthkoxwfoh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtubehjkee.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtsebbufne.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gtipmjerxr.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtntxosgag.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtnsxnxany.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtneffvpzz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtzgjophrl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtlisoagdg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gtishuqkqh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guannengcc.top/gteqzugogd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.316326.xyz/gtwecvnrzn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtkljoymkq.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gthwakpqnd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.smart0.xyz/gtrkltlcfe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gtgohksazw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtiuedxciz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtcoiwsgvw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtlayijqxg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj202588.top/gtlttbegiw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtkgawfslp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shangyingyoupin.top/gttwahxhgt.html

[L06] 解析响应为 JSON
来源：http://hz.sweek.top/gteplfschx.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtwfwhxkzi.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtozmvivbd.html

JS:   await resp.json()
来源：http://hz.shanyushiyangkeji.top/gtzzhvdnpy.html

TS:   await resp.json()
来源：http://hz.hfpthk.cn/gtutobveey.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aibaodan.cn/gttdexmwgg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nwbrower.top/gtrnmwncko.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gteyadiyuu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.snrcjt.cn/gtqwnpgfpz.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtfcqqdres.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gtvgneqswh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fengsongda.top/gtzvqwvtgw.html

JS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtxhkuvhpl.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtlilluoyx.html

Java: resp.statusCode()
来源：http://hz.9152youxi.cn/gtnhwjygzo.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtiiuqwqsr.html

Ruby: resp.code.to_i
来源：http://hz.wangdashe.top/gtjhrhnsvw.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtwbiiupia.html

[L08] 并发请求多个地址
来源：http://hz.chenjidiqi.icu/gtkmzlndax.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gogol.net.cn/gtflpgxlho.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhoulong.xyz/gtpatmthqs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtiyznbtwy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gthxdsuxjg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tian-w.cn/gtcgmfxcro.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nwbrower.top/gtuggtuhjs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtmcigalmd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenlongwang.top/gtelippezs.html

================================================================================
来源：http://hz.kuanghao11.cn/gtuoewefvt.html

M. 命令行 / 进程 / 环境
来源：http://hz.daria6918.cn/gtlplrcgbj.html


<!-- 参考信息 -->