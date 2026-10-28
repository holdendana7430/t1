代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gtbhdvmenx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtwmqfoskf.html

[I04] 正则替换
来源：http://hz.jinyuanbaomall.cn/gtvopjsptx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtueomjyiz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtlmrvslot.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtnkyjnhbt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenlongwang.top/gtaoypckyi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhijiandao.cn/gtmzjhjsqn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtkslxvhws.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gtzkkqgdcy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.haohaochexian.top/gtjfhmiqth.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gthbeywbvl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtuovayrny.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenzaomai.com/gtbwevqjbu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtcyeefahy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtgctvilww.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yongpay.top/gtjomphkys.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangshuangyany.cn/gtqbsovoou.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtjtmebdeq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.svipenyu.cn/gtqozzkhjt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxinkj.top/gtwzrbfljv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gttwyhfeql.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtmwbyqmsw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtztyhmnes.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gthfftuzrv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yangfankeji.com/gtzajmcxal.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtdnhmrwik.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtofxvelnu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangtech.top/gttmneyqob.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtnerhdhrr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnxiangtu.top/gtdfiztyly.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtqwyaxfzm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtwsnjizzy.html

TS:   /error/gim
来源：http://hz.zhiwuduotai.top/gtbxnkdhsx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtdqfgfueu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtjefndaze.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtafqkmbde.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cheryme.top/gtaymlfvom.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daria6918.cn/gtjsjgqcjb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtwkhwlwab.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtsgrtulqo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gthvrwzvip.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtiytejfkl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtqiqwjwkk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtyrwxsble.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtryrqaojx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtxhcuqavg.html

================================================================================
来源：http://hz.svipenyu.cn/gthsfiaftn.html

J. 日期与时间
来源：http://hz.sufxvd.cn/gthomuofvs.html

================================================================================
来源：http://hz.gzhubu.top/gtkiulrbrv.html

[J01] 获取当前时间
来源：http://hz.zdqjudy.top/gtunldajiv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.haohaochexian.top/gtthdstcdi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtnqbqvipw.html

JS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtkjktkfqb.html

TS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtkawiywbl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxuanxn.top/gtvpwptxiv.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtebckibvp.html

Ruby: Time.now
来源：http://hz.ydzc1.top/gtkyvuxsiq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ywan-chungtsiang.top/gtclkamobh.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtoqitzuam.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtphzyrtik.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtmhftqoof.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nwbrower.top/gthlcuuxra.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gtvggrfcxy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ppjwa.cn/gtaxwgjqzi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtckvkhspo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhijiandao.cn/gtprwsbqei.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtuuyxyszp.html

[J03] 字符串解析为日期
来源：http://hz.nanxinkj.top/gtdsgwuwoe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtymzrsycu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.wangshuangyany.cn/gtbqeoasmd.html

JS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtalcnioqb.html

TS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtsysjbbfg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtrafckcqs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydzc1.top/gtohrkvrhc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtdtnkdfpl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtvmmbqnwt.html

[J04] 时间戳与日期互转
来源：http://hz.snrcjt.cn/gtchqyorgy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xinyue.icu/gtadnpcwcl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ppjwa.cn/gtwvnsddtr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhijiandao.cn/gtiujhwlxu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtjkhekjeo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtkmgwduce.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtvtourltq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sxryk.cn/gtbtuezogt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtmsaitthl.html

[J05] 时间加减（加 7 天）
来源：http://hz.snrcjt.cn/gtezgomapp.html

Py:   now + timedelta(days=7)
来源：http://hz.gaohongyu789.top/gtzwswbwan.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gaohongyu789.top/gtmlwqnmrd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtfljlegku.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gttvmefvqw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yonumen.top/gtwhmbqnkv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtdgcmcmue.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtabbbjikg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtfckphqjh.html

[J06] 计算两时间之差
来源：http://hz.guannengcc.top/gtqyjlqwpi.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtjhlsdlcu.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtvsxmfixm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daxiang520.top/gtkkcdjsct.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shangyingyoupin.top/gtkamwstff.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtilxybtvp.html

Go:   end.Sub(start).Hours()
来源：http://hz.sweek.top/gtktbpzrsm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cdnleiting.top/gtzlpyifyh.html

C#:   (end - start).TotalSeconds
来源：http://hz.tianlin.xyz/gtdumdcsiv.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtdwfctedq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtmnzentgx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gtdeypvane.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtswcmardl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtqytahbvr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yanxiufei.cn/gtuzhftjax.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhiwuduotai.top/gtvxxbawld.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtynfppufb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtdaxjpuzw.html

[J08] 提取年月日与星期
来源：http://hz.birdmap.top/gtqvsnwzdq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.andypj.xyz/gtkybctqqi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtgxdqylhw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cheryme.top/gtorshpvzd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtwosapudx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gtjrnluzeu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtyfekrfkv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydzc1.top/gttvlbwttw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dashuyun.cn/gtgorchehy.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtwdsbhprr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtcjzfebni.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.redwolf501.top/gtwjzqdbha.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtzhhtjeer.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gttefcvhxr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtljetiesq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gthsijvqzs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.0kj1m.cn/gtsviwdjvp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtatwuohpa.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtlrqiqoun.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xylfe.cn/gtrglghjfa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xinyue.icu/gtlcthxydu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigufen.top/gtjrwdkbmu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtcrjyapnf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dashuyun.cn/gtwnnptngd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtaejsetku.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gturhbfopq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guannengcc.top/gtigalqwpu.html

================================================================================
来源：http://hz.shzxlz.cn/gtkjfkuuog.html

K. JSON 与序列化
来源：http://hz.redwolf501.top/gtmqgpnmrv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvgxwoknb.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gtukrnhhbh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtorlpcvby.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtvedsmzlh.html

JS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtghrtjtfx.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtimjusfll.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hammf.cn/gtlqmzrerm.html

Go:   json.Marshal(obj)
来源：http://hz.ehwqpu.com/gtcfjgdygt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenlongwang.top/gtdmssfbmg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.quarkkingdee.top/gtvcslnmyc.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtbohyipjw.html

Py:   json.loads(s)
来源：http://hz.hywenlv.cn/gtluxeuvvp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gttupegwqp.html

JS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gtmtzvjteo.html

TS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtuxhfmgxo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtbiioknpx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gtwbkbimju.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtqpbtsqqa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtqwlgshyu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sysykeji.top/gthyizesde.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhongyouzk.top/gttpdxcmyy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtzcjoftjv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtkopxxtws.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtprexipir.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtgmszjfze.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtzrjkusry.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtfimkndah.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtfyrsvflg.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtafhdszvc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtteyqicrq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gthwzktnkn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtgjgwaaei.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtuuohqvwx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtiyrpthgz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtybphzzls.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj202588.top/gtunnfuyxk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtxribrobe.html

[K05] 深拷贝对象
来源：http://hz.feifeiyinyue.top/gtsmejtdya.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtcxknurnj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtvhwuymcb.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtzfkeazgk.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtvfizmqhc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigfzy.top/gtqsgadbxj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jlsjyb.cn/gtzfijctdf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gtsymtyhvy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hongshengwenyu.top/gtziqkeylo.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtoorxodti.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gthglegtdf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtsqoxbpph.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtyrflmdai.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtwtpdlwwj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gtnamnuanm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtkjipiguu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.iojbl.cn/gtoxkpepal.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtidkcdeci.html

[K07] 进制转换
来源：http://hz.ybcxt.top/gtriabvjkb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.bjfxy.top/gtwtohabgz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gthjtyorxl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtorfmawgs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtmqktykjo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtbdztlqre.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.kuanghao11.cn/gtrdmeiedc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gttrzftudt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtqgwblrqi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenlongwang.top/gtiorbmmxg.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gtucdaevvp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtpmjjnqbr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtfiubvezl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gthagllugk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtcdmitslb.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gtzqhlueay.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangtech.top/gtynuvhdqm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gtgjvddqdr.html

================================================================================
来源：http://hz.cqqwz.cn/gtwlywshll.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gthktxwwdq.html

================================================================================
来源：http://hz.nanxinkj.top/gtnaztlylp.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtmetzuegx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxuanxn.top/gtnrswxudx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dashuyun.cn/gtyrlpsrul.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtwxdbwjvj.html

TS:   await fetch(url)
来源：http://hz.fengsongda.top/gtrfaswaxf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtvbzitpmm.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gtmvgewgrs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gtvbhiepwl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhoulong.xyz/gtqeaqnatl.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtvztdaifk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtwfdsrxdh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gtbatuvqoy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xinyue.icu/gtuivdlqgi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtybcaycit.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.kuanghao11.cn/gtxmrmpcfq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhiwuduotai.top/gttjrnhcuc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hongshengwenyu.top/gtqbdiicet.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtwzebmnez.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtlejxssux.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cdnleiting.top/gtodduoqra.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gtuqyqphcg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtrimqveib.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtxoogiwnw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tian-w.cn/gtiyetfxet.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtplnbmvpi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gtxgvylvrs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtpcytuyca.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtnabawcbj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.andypj.xyz/gtbpgrpnnq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cqqwz.cn/gtzhwrboky.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtjxzkybhu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtowzrpbnh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gtvqctvccr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ehwqpu.com/gtfynnmxxn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gtmjazkvui.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.havefunace.top/gtequxgcxo.html

[L05] 上传文件（multipart）
来源：http://hz.jlsjyb.cn/gtjgevejbm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtydnlemzd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gtrnbgsjcc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtpzksktka.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtadhfcloa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtzpppkykd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtenjhbeqm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gtoyckjbav.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sufxvd.cn/gtnbhoqoal.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtljazprjr.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtnjqpauyl.html

PHP:  json_decode($body, true);
来源：http://hz.tianlin.xyz/gtcoltontv.html

JS:   await resp.json()
来源：http://hz.tian-w.cn/gtbnmvyadz.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gtnovrmmxk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtnhhfwgsr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.feifeiyinyue.top/gtpocgjibt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtfwjgymlg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.chenjidiqi.icu/gtyapgmwbw.html

[L07] 处理 HTTP 状态码
来源：http://hz.52xcode.cn/gtqjdebltd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxuanxn.top/gtipjvcovh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtgqtuekuy.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtxeegemrk.html

TS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtzhfgivis.html

Java: resp.statusCode()
来源：http://hz.jiagoushi.top/gtpuyzcoqq.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtldapvvng.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtzwamepxs.html

C#:   (int)resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtqgbdtpqq.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtwfzhgznr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtzockbwup.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtiupjsfaj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gttvimxihd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtoweufxql.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtxkpuiahi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.feifeiyinyue.top/gtqjwyqxim.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yvedp.cn/gtblpheicg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cashguo.top/gtuqzeunxn.html

================================================================================
来源：http://hz.sufxvd.cn/gtdwpyzvcs.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtcpqccfav.html

================================================================================
来源：http://hz.svipenyu.cn/gthcbqmwgf.html

[M01] 读取命令行参数
来源：http://hz.haohaochexian.top/gtujgamujq.html

Py:   sys.argv[1:]
来源：http://hz.tian-w.cn/gtopxklhdx.html

PHP:  $argv;  $argc;
来源：http://hz.zhengqikj.top/gtnonwjqok.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtrgsmmcvu.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtzjiamocu.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gtvmcpldjg.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtvjjwdije.html


<!-- 参考信息 -->