代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtwvjpuilf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtmetmegkw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtitsldsro.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtxruigevi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinyuanbaomall.cn/gtjokifliy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guannengcc.top/gtjksukcfs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtdqlwqmnd.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gtysswzzna.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtykvziugm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtrbieqxiy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtdtfdrxtb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtvraukeje.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jlsjyb.cn/gthjlzdbnm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhoulong.xyz/gttvpplgvu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtcvziflom.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guowangkeji.top/gtlpgtrjcf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gtadupqnkg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtzidixqdy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydzc1.top/gtwzaextaq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gtuqmuhdvz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtripufwvb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtqekkflcg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangtech.top/gtxzyeieye.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnqzz.top/gtyjeswvcg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtfrfktlil.html

[I07] 忽略大小写与多行模式
来源：http://hz.pengpengdd.cyou/gtvanyljui.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.havefunace.top/gtfzhjogpc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtxlrefrws.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtrxqkgmae.html

TS:   /error/gim
来源：http://hz.tanke756.top/gtprwhkuqm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtehazqkin.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.feifeiyinyue.top/gtuoxsquuk.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtjwqejfqx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gtdytjkytb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gtzucdkhlz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnxiangtu.top/gtgvifofea.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jianghu66.top/gtkmrjszfq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gttyvjaoho.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtcwcfoxtd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtflkcajcy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtxupowdaf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258888.top/gtrayajicl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtjcnjmlhf.html

================================================================================
来源：http://hz.yj20258888.top/gtfcldkwtn.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtpvhjasxt.html

================================================================================
来源：http://hz.yangfankeji.com/gtxwhkdlfu.html

[J01] 获取当前时间
来源：http://hz.chenlongwang.top/gtpzychbao.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cashguo.top/gtwwwhmniy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtpuljigkw.html

JS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtnriaaekg.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtnzsxvxkn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuxming.cn/gtoomwxshb.html

Go:   time.Now()
来源：http://hz.fengsongda.top/gtzaahxajw.html

Ruby: Time.now
来源：http://hz.jqgfzy.top/gtjuvrkgxu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.bjfxy.top/gtinzwelby.html

[J02] 格式化输出
来源：http://hz.quarkkingdee.top/gtvapvhpdl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gttncynslc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtfqosutnk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtfvsbbpdr.html

TS:   d.toISOString()
来源：http://hz.chenzaomai.com/gtycbfkppg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dashuyun.cn/gtxvwlkxjy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nwbrower.top/gtuvwlseqi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtffrunado.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtwmbnevdf.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtnqhofjns.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guowangkeji.top/gtgnvupveb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtzvtgauul.html

JS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtyypryfsi.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtifdflxke.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtuntevcym.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtikvmpbio.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtweunbpxn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhaomingkeji.xyz/gttwtybdfj.html

[J04] 时间戳与日期互转
来源：http://hz.dashuyun.cn/gtshvbamth.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuanzx.com/gtbdrsomjl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cqqwz.cn/gttnkxkzvl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtyknkmgxi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sysykeji.top/gtnfcdpapx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guowangkeji.top/gttudimmxs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guowangkeji.top/gtxnflsbdy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuanzx.com/gtwwqrhzjp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhiwuduotai.top/gtoykmeiyg.html

[J05] 时间加减（加 7 天）
来源：http://hz.pycfn.com/gtawkooahr.html

Py:   now + timedelta(days=7)
来源：http://hz.yj202588.top/gtzrqdizsz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtlerdvhhe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtfhujldea.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtesozdxjl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtydbfhtob.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xziqi.cn/gtvjtaeore.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtnislffon.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtttvlopfg.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtzvaezzjg.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtjvspwpkq.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gtuntclhlz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dianchejie.cn/gtovmkdbmc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtizndjkrq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtwtapgjpm.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtfcohaewe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtfirjzumk.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtalfxccxd.html

[J07] 比较两个日期
来源：http://hz.quarkkingdee.top/gtsvhqsnou.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtdjwftfey.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtvxbnbvta.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigufen.top/gtvprhdawn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gttqooahgc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenzaomai.com/gtugzjhtnp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tian-w.cn/gtmcgusgxi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtimxgvqil.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtmmoxlrir.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtriucjafa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnqzz.top/gtwgmzoolo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtpqrrfqtf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gtwlfgqnla.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gttfikeiac.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtcoaxupuk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhiwuduotai.top/gtwylrutjl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtdfvgynmo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtjsebqexl.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtpdkshkrd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aizwys.cn/gtvnpjnrqu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.redwolf501.top/gtbrooaxwj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtjcdukulx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtlxeaehso.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtwpemhflb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xylfe.cn/gtzzhfsjiu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhongyouzk.top/gtefdfewqg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtykdxahto.html

[J10] 取今天 / 本月第一天
来源：http://hz.sysykeji.top/gttuhotfql.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.meibo888.top/gtlyddofsn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gthclzisss.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.52xcode.cn/gtivszzylv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtyqinblfb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtpdmysdnw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtexgbmhyp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.bjfxy.top/gtapwzfpjo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gtucivehrk.html

================================================================================
来源：http://hz.mhx1999.top/gtlafjjscu.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gtmmpyoydh.html

================================================================================
来源：http://hz.bjfxy.top/gtzizrakbu.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gtfyjicben.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gzhubu.top/gtcobbefnl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtdthzwymb.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtblkaivwm.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtudvluaie.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gtpacyiakv.html

Go:   json.Marshal(obj)
来源：http://hz.quarkkingdee.top/gtpgnzylrz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtdyqhydpo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zycfv.cn/gtdricotod.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtriebkygc.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtwbriiofa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tian-w.cn/gtgnloykrx.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtmvbetovp.html

TS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtsncsrcyf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gttjkdhezw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtobvijguj.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtktrpbbow.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gtfdlnfduw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jiagoushi.top/gtcsqisnox.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtfunblhay.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtvtypmmfe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtbfotwniv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtqaopgkfj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenlongwang.top/gtxmqcdhib.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dashuyun.cn/gtckbzjwhk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtquoclkjw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtpeteobzi.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtvskslybw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yvedp.cn/gtnrukjago.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtusqiknfz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtrkvrlfhj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtekcgurhc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtjofrapqz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtllqjhdpk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tianlin.xyz/gtisskhxka.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtjbvwotei.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtmxnmhjlz.html

Py:   copy.deepcopy(obj)
来源：http://hz.guannengcc.top/gtgqncjpib.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fengsongda.top/gtgphxvdmk.html

JS:   structuredClone(obj)
来源：http://hz.tanke756.top/gttpirsikh.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtvheviwpl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ywan-chungtsiang.top/gtubgpkhup.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtcjityyqg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.0kj1m.cn/gteezbpuly.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtlqdpucql.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gthaggbvma.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtwfruhdha.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtxqsvzgjl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtvyukrrch.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtxztaotyn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gthygkmfpq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.pycfn.com/gtewepretp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtumyroepe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gtveodzlvu.html

[K07] 进制转换
来源：http://hz.nanxinkj.top/gtxhtblolo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pengpengdd.cyou/gtsadqtsdv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtjvxaukqp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtakaihuzb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtmadbsmwq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtvsymiprr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hnqzz.top/gtosxfrfmn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gtodezdgnu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhiwuduotai.top/gtwnsxuxlf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gtswihtskb.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtjvptvbez.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigufen.top/gtrozxhdic.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtwrzpnwla.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtwsqtirjc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtcplsywch.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gteizuiawj.html

Ruby: Marshal.dump(obj)
来源：http://hz.guowangkeji.top/gtnpjzqmfx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtokvyvqzw.html

================================================================================
来源：http://hz.yj20258888.top/gtrimanuzu.html

L. 网络请求
来源：http://hz.zycfv.cn/gtfcuwqnyk.html

================================================================================
来源：http://hz.sysykeji.top/gtiwghifzz.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gttgtbugol.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.iojbl.cn/gttfkhceic.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtaondfidb.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtxmhuekae.html

TS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtnnezcxpp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtrkyrngzh.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gtihwcfsfc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtvebfewwd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.kuanghao11.cn/gttevnwlkx.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtvpufvwgv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.svipenyu.cn/gtigsgokqa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtmwyxkpwy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtvxssfbtp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtoqttbwey.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtfplonior.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuetiantiany.cn/gtembzcjnm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtihsswfmr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtpqgtumtp.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtgpzfyqci.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gtwobeqfbh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gtlosyrkgm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtqvzuuvth.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtpwrbktme.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtlrdkvkil.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangdashe.top/gtkphqtryc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtiglzykkv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtevppntfv.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtsmcqjrlj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tianlin.xyz/gtmsxbnrsa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gtddnriazb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtophwrytd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtiymhorav.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtwnizirpr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuxming.cn/gtgiphyqma.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtxamsyqkd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jyoumei.cn/gtcwgkksgv.html

[L05] 上传文件（multipart）
来源：http://hz.xingfuxueyuan.xyz/gtsgehylix.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ehwqpu.com/gtucafgvvd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hysaishi.cn/gtmilabgdm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtfhfkxqou.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtowrysglv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenjidiqi.icu/gtnnpgupfx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guannengcc.top/gtzianweee.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtqsnaviig.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aizwys.cn/gtginmqrgu.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gthcokwiad.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gtgpnigxam.html

PHP:  json_decode($body, true);
来源：http://hz.cucudq.cn/gtsfovrwop.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtfwumpons.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtsqjuhduu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zycfv.cn/gtrkaxlarr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.snrcjt.cn/gtwyfulkch.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jianghu66.top/gtbwqvghat.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhiwuduotai.top/gtoaxpxvnv.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtcdnokebv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jyoumei.cn/gtprzyhgdj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtoauwsjcz.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtuxnuoexc.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtnqjymtyj.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtspmllipk.html

Go:   resp.StatusCode
来源：http://hz.cheryme.top/gthuohzmom.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtdyqqnetu.html

C#:   (int)resp.StatusCode
来源：http://hz.jianghu66.top/gtbhucgezz.html

[L08] 并发请求多个地址
来源：http://hz.jqgfzy.top/gtbfetyvsp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigufen.top/gtinpdltpt.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gtaynsraio.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtfhdsadoe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtvfmsbrqr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.52xcode.cn/gtqzlcxcpy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtezojoivk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xingfuxueyuan.xyz/gttlegbuik.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sufxvd.cn/gtwurixqhc.html

================================================================================
来源：http://hz.sweek.top/gtncadwhqg.html

M. 命令行 / 进程 / 环境
来源：http://hz.tanke756.top/gtblsggblu.html

================================================================================
来源：http://hz.dashuyun.cn/gtqbxaeqmv.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gtlthvnigs.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtkfkfmyii.html

PHP:  $argv;  $argc;
来源：http://hz.shuidangran.top/gtveswpauu.html

JS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtwshbwwxp.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtbhgjoakf.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gtjrducces.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtajgykpqw.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtxamcklnw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258.top/gtirddnzdk.html

[M02] 读取环境变量
来源：http://hz.zhijiandao.cn/gthpxekcng.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtalcouimi.html


<!-- 参考信息 -->