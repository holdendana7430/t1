代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.havefunace.top/gtkqskmcvo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtdntdfoco.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gtpqmhxios.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gtmhpkhfri.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.snrcjt.cn/gtkkgmqxal.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aibaodan.cn/gtasnzxles.html

[I04] 正则替换
来源：http://hz.aizwys.cn/gtggaypqnh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangkeji.top/gtkkcsyitn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gteaxvrmfx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtkxbbdxnw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtgksbukcs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtedgpzrfk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cheryme.top/gtecdzalpu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zycfv.cn/gtdjvptege.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtphjuolln.html

[I05] 按正则拆分
来源：http://hz.andypj.xyz/gtzgohjdci.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.haohaochexian.top/gtztbkvpzt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gtgqnupxxz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtrjlswpfo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtjibucsqy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtawmlssjf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtmlmkubqk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtkwhplygi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtfrdbxsxj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtqqdihymi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtmsygonjk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aibaodan.cn/gtibwnijin.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtseuvgepo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtoksollek.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtxexuhzsl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gtttkwfqvf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtnlgwhfjt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtbwpnhwcl.html

[I07] 忽略大小写与多行模式
来源：http://hz.jiagoushi.top/gtlwygyzsr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtbfldvfdo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtmonafghg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yongpay.top/gtufsfstab.html

TS:   /error/gim
来源：http://hz.cashguo.top/gthverxbbr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gtnqrjbbsb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtmkwulcwu.html

Ruby: s.scan(/error/i)
来源：http://hz.zycfv.cn/gtvbyzncvr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cheryme.top/gtjbnekeab.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuxming.cn/gtzlnuarki.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtqpqcbvws.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yueranfly.top/gtkltvkwlc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtodyyjpok.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtpeepzfup.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtvshnhtwv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtqnloeekt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtxnixehhv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gthlhzlofs.html

================================================================================
来源：http://hz.sweek.top/gtuqqsjvfn.html

J. 日期与时间
来源：http://hz.fzhhl.top/gtvkdhqoqq.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtaonxdkzf.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtkiyjmlas.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtahyqwreo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtoqtgmvoi.html

JS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtjxaxaouf.html

TS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtxsvjzupl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.bjfxy.top/gthdnqrzax.html

Go:   time.Now()
来源：http://hz.quarkkingdee.top/gtlegfatrn.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtczcosbdf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtvbajdbve.html

[J02] 格式化输出
来源：http://hz.shzxlz.cn/gtcvilapvm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtkvpkrnvj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtjwmfucuw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangtech.top/gtqgbooagr.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtufqmdsgz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jlsjyb.cn/gtpxjrtwhb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jiagoushi.top/gtdikmamem.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtrmqgmxle.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gthqtvnwww.html

[J03] 字符串解析为日期
来源：http://hz.fengsongda.top/gtlackjdgw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gtwogeigjf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.quarkkingdee.top/gtodryopmy.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtmquhyack.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtrojuorim.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtufbnceqo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.9152youxi.cn/gtlnoqmqwq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtnaefjolj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtplrsyzos.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtrcgbvrea.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtgsqwtlkn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jlsjyb.cn/gtwgfuihfm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xylfe.cn/gtpalrxonr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gthtbcikda.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gzhubu.top/gtixvnogju.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hfpthk.cn/gtcygalgsb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gthgzeiklt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gtgvdkgqwl.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtgfrkbkub.html

Py:   now + timedelta(days=7)
来源：http://hz.hywenlv.cn/gthtiohcyi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ivvv.top/gtolucagqv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtnxpiraxs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtuhespjvu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtrtgersqp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtcxdkrirr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtnvwyiwmq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtkkriofxp.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtguumayjg.html

Py:   (end - start).total_seconds()
来源：http://hz.zycfv.cn/gthuqszsuv.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtksnnpavi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tian-w.cn/gtdxmrygec.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtxtgeeqeu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtaspulemr.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtxhufwjxl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.feifeiyinyue.top/gtfwizoonw.html

C#:   (end - start).TotalSeconds
来源：http://hz.meibo888.top/gthrwphibr.html

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtsdyfduwb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtbvtqhcde.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtiokknkyk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtorwrcpah.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtdxipqibu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtrichfinh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jlsjyb.cn/gtfzkpcbcy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtffizlsgr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtdnvljouc.html

[J08] 提取年月日与星期
来源：http://hz.ywan-chungtsiang.top/gthyukjupk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yueranfly.top/gtqhlcntdr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hammf.cn/gtzxoapnmw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtgnohionh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtjfekwthy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtdfbpriqi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fzhhl.top/gtozbsuazf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shuidangran.top/gtutzuhefy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtgkurwolg.html

[J09] 时区处理
来源：http://hz.zhoulong.xyz/gtttpudonk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtzfsqelaw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hammf.cn/gtgxxgyxex.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtkgwadoii.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtyaxpjipj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sysykeji.top/gtebqfkybv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtleoatxqy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guannengcc.top/gtxdzhilbp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtzyspxvqm.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtepyjarsw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtjstvfiao.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhixingplan.top/gtwlejnppd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.0kj1m.cn/gtetskbjww.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gthgurgfcq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtzmihkara.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gtstjdnuym.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtutvusbmp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.iojbl.cn/gtsngovsii.html

================================================================================
来源：http://hz.wangdashe.top/gtndstorlc.html

K. JSON 与序列化
来源：http://hz.shanyushiyangtech.top/gtwerzxlbt.html

================================================================================
来源：http://hz.nwbrower.top/gtdamueimm.html

[K01] 对象转 JSON 字符串
来源：http://hz.meibo888.top/gtbsjvxlqk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtorgtndks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtuvxdwhfs.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtxijkvrrb.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtquautepo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gtdddyquws.html

Go:   json.Marshal(obj)
来源：http://hz.ehwqpu.com/gteahnfzbm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigufen.top/gteztydfcn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtyibrmysf.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtppomdetb.html

Py:   json.loads(s)
来源：http://hz.jqgufenzy.top/gtrubpdxuq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtixrgltek.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtbltgcbfo.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtdtlenven.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtgobbgwyi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gterfqporl.html

Ruby: JSON.parse(s)
来源：http://hz.yangfankeji.com/gtgwuvtsth.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gtwfmghhzw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtnsahletm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtawssujuk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtkveuttzm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtlarkjawq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtmbgqwsbt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.birdmap.top/gtlalethxu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zdqjudy.top/gtpjafugng.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zdqjudy.top/gteukoprfg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtazstzmyw.html

[K04] 读取 JSON 文件
来源：http://hz.52xcode.cn/gtkjtxrdjv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtvihyszpf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hammf.cn/gtjkmqjxfc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtjewuupxi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtalyoocfb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.316326.xyz/gtxthopikn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtqgdssgtp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fzhhl.top/gtjdomzrrs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cdnleiting.top/gtxorvzzqr.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gtfbwexsoi.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtpwitnvyp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtgvczellq.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtqvglaeas.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtpxxqhwpl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yanxiufei.cn/gteaxiqzym.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtxvfhkhtw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtxkhscnjo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gthqrpbylt.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtgbnkzknx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtyzwarizc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yonumen.top/gtoowysqze.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtmpzchmbk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtqbgngbcg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtuvxonsdi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtlicowszr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gtemwjamum.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnqzz.top/gtgxcjlcie.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtzerljqxb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.mhx1999.top/gtwmtnfnsg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gteqydhpuy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtpplpgoln.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtuxuzgcec.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gthmexxlka.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gtjbdhgbvy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhaomingkeji.xyz/gteavzuwoa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtvduknbum.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtduxpperv.html

Py:   pickle.dumps(obj)
来源：http://hz.yangfankeji.com/gtbbaiqkrk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtdhtqmhki.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtgsnxlawr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtjfagkiio.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.mhx1999.top/gtvoxpldhl.html

Go:   encoding/gob
来源：http://hz.yongpay.top/gtvvkyghls.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtfcidnypl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jyoumei.cn/gtchykncgp.html

================================================================================
来源：http://hz.yj202588.top/gtoexxcnin.html

L. 网络请求
来源：http://hz.gaohongyu789.top/gtamxjlkmo.html

================================================================================
来源：http://hz.yonumen.top/gtuqjxrpwq.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtazdchtfu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtrpicqdzs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.snrcjt.cn/gtusmunoml.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtctyyjxgj.html

TS:   await fetch(url)
来源：http://hz.cheryme.top/gtutaqkvjc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtycfaowvo.html

Go:   resp, err := http.Get(url)
来源：http://hz.mhx1999.top/gtcrlapgmb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhijiandao.cn/gtgyqlpmbi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yanxiufei.cn/gthzojuwdf.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtxixbycbg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangkeji.top/gtgpyeozrs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtzxisknst.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtolusfvwb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtwyllycnv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtvpowmcqq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtwfyyiaqf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.feifeiyinyue.top/gtibflkqxt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.9152youxi.cn/gtjcwczblt.html

[L03] 设置自定义请求头
来源：http://hz.wangshuangyany.cn/gtvcbtastg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtirdyyufc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ybcxt.top/gtypgyeguy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtukxsehhm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtjoycpljd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fengsongda.top/gtrlwqlqwl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtsvubftqe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guowangkeji.top/gtrllufleg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yongpay.top/gtullefsdy.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtszghkxso.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtpzvdtbwo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuxming.cn/gtizgnhnqw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtedecrpim.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtgstzpyta.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtzqiyikmu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtihgqtbmc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pengpengdd.cyou/gtatsiomav.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fengsongda.top/gtkpglwwru.html

[L05] 上传文件（multipart）
来源：http://hz.hywenlv.cn/gtnnaiwtsc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pycfn.com/gtqyzfgyds.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinghuilouyu.cn/gtzbdyedur.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.andypj.xyz/gtbktgrsfp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gttflbxlhm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gthsahtzzs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cheryme.top/gtcqemjlav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sxryk.cn/gtvdtidnsg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hywenlv.cn/gtcpkuyalf.html

[L06] 解析响应为 JSON
来源：http://hz.quarkkingdee.top/gttsgxgxir.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gtxgkbfbwx.html

PHP:  json_decode($body, true);
来源：http://hz.zdqjudy.top/gtujsuwmzu.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gtpskapnpl.html

TS:   await resp.json()
来源：http://hz.meibo888.top/gtwoowxawz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gtkpsazjur.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gttgwltprt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gtlsnmtpvu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxinkj.top/gtfoxiidak.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtxyospemh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtrcsxwhnj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yangfankeji.com/gtcwmkggro.html

JS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtkdvddctj.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gthyzlcsqr.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtbozuwwbo.html

Go:   resp.StatusCode
来源：http://hz.yanxiufei.cn/gthtbulxbh.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtuczlxtum.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtaifjtptl.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtcsdscord.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gttrvznaxd.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtsgiphkrv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtrjjadvzw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gthsvlkvxg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxinkj.top/gtvtssconr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtrupadvaf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gtieguofbf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fengsongda.top/gttxakiojw.html

================================================================================
来源：http://hz.pycfn.com/gtsdhgcwdk.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gtrkrbvwrx.html

================================================================================
来源：http://hz.hysaishi.cn/gtwywmtzyr.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gttzqbbhhf.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gtplkviooo.html

PHP:  $argv;  $argc;
来源：http://hz.ybcxt.top/gtckopewts.html


<!-- 参考信息 -->