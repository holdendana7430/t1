代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.9152youxi.cn/gtdtaeeozk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtcvuzvuii.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxuanxn.top/gtmwdtfjww.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtdqshpcfj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtegntoqhu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.svipenyu.cn/gtgzbutzdj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtvaevzqpi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cashguo.top/gthwvcvogm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtkbmsdqgv.html

[I07] 忽略大小写与多行模式
来源：http://hz.fengsongda.top/gtqtptmxdb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ywan-chungtsiang.top/gtovpnlcln.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtpkkjchmm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtvrwxmnxu.html

TS:   /error/gim
来源：http://hz.wangshuangyany.cn/gtgkxgnyre.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtdgeteees.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtmpvveefw.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtbbaiapqq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gtphrcgasz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jiagoushi.top/gtntbzwkba.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuanzhike.top/gtebhxabjg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.0kj1m.cn/gtnxnfbaiq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtwoaasykh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gteuixmbxw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtdcrjoamk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtxjluicew.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtypadjftc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtmwpiuyfq.html

================================================================================
来源：http://hz.cheryme.top/gtwyqfokgw.html

J. 日期与时间
来源：http://hz.sxryk.cn/gtuzqxldem.html

================================================================================
来源：http://hz.mhx1999.top/gtclafnmii.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtmsdwzbnu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.52xcode.cn/gtuyvfihhd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtqeufgwhg.html

JS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gttsaynybz.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtqxurfriq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nwbrower.top/gtprragvrc.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtkwwnzlau.html

Ruby: Time.now
来源：http://hz.yongpay.top/gtlyviktsh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yvedp.cn/gtdxgqirrb.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtvirediyj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtavjvahjm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtfnxlcgas.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtqdzwdkgl.html

TS:   d.toISOString()
来源：http://hz.jyoumei.cn/gtcihgwtjo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtmtjoxjsc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangkeji.top/gtnjkgbqga.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtehsngtdm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtknjcfxxz.html

[J03] 字符串解析为日期
来源：http://hz.jlsjyb.cn/gtxlzqpjbo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhengqikj.top/gtsjgynbvp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gtauhgeijg.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtgghdlkly.html

TS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtrnpcafnu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gthqrxeccj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gttyjnhkrl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtfaqitkpr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shuidangran.top/gtfkqwmeyi.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtjwnxeldj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtoszaanqv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtsmacddvk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtpieubgjk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.c1oappe.top/gthanylpdl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtcbiunmic.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gtvemcfjpa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtsinxoaru.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sysykeji.top/gtlknunuzy.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtrapyckem.html

Py:   now + timedelta(days=7)
来源：http://hz.yongpay.top/gtoesajwig.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtlgszglxg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtggdacklw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtwvuycmwn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydzc1.top/gtbetikgrv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtjkjwwlcw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtbsxunnyz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtvezhzqjf.html

[J06] 计算两时间之差
来源：http://hz.dianchejie.cn/gtjspvcdje.html

Py:   (end - start).total_seconds()
来源：http://hz.cqqwz.cn/gtmzeknxyf.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxuanxn.top/gtwstuayqm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtgzndkxbi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zycfv.cn/gtwtimbfyq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sweek.top/gtkixaeuez.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtljylstec.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinyuanbaomall.cn/gtuuvakero.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtsihzemwu.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gtlzyihivb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtbkhxyzab.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gtkejbpljo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtcstroyxl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gttasmfumg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.9152youxi.cn/gtqjeizppg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtbfwrnpha.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtpyppqrvo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtxlzoywut.html

[J08] 提取年月日与星期
来源：http://hz.dashuyun.cn/gtptzbijhc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuanzx.com/gtnkqsdsaw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pengpengdd.cyou/gtgutcdxab.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtfymgebkx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtjtjjeswy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtlmgmsaek.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtznqeicxk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtjapwpkmv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtvfqnbtsb.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtzqfbkojy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtgxtjgwhm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtkfsikkpn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtymwslhfz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtzwyzghpc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtuhkhhotn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhengqikj.top/gtkomiwksu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xinyue.icu/gtlxtdxbon.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgfzy.top/gtpcbtlima.html

[J10] 取今天 / 本月第一天
来源：http://hz.cashguo.top/gtmfxubitq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aibaodan.cn/gtrxyuagww.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cheryme.top/gtipdnggef.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gthnpnzvmq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cqqwz.cn/gtaoytxayj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtjutpaknw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtggjievni.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtxpqyguno.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.9152youxi.cn/gthhxvvcyz.html

================================================================================
来源：http://hz.shzxlz.cn/gtprdqqhth.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtvliwttva.html

================================================================================
来源：http://hz.xziqi.cn/gtushkzikj.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtepakgzxs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gttzyvvlts.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtetkjzizh.html

JS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtgekosjdu.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtibsvbhip.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shuidangran.top/gtfcizvdgy.html

Go:   json.Marshal(obj)
来源：http://hz.hysaishi.cn/gtddfozszv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gtglvyypel.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtseyczcyi.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtlvzcrmko.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtnyxgsfvy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hfpthk.cn/gthryzbiun.html

JS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtftiqehuc.html

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtcclgcmha.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtisggqfju.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtgrjrteis.html

Ruby: JSON.parse(s)
来源：http://hz.tian-w.cn/gtnmagpued.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gtefaelpfg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258888.top/gtpoebyzao.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtanbszzvb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtvggsrert.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtwkpwyxnn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gthwyetxvh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtoinykekw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sysykeji.top/gtbrmljmfv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shangyingyoupin.top/gtcqqhcccs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtdlgvwhcj.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtmhoxwkdq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtsuaihtau.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtiueqnduz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtnbhiajoe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtvgbhlgoc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gthjspclry.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtlnytqtxp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tanke756.top/gtjwwswjqq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ppjwa.cn/gtgofyzkfn.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtgufcfino.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtukxjjkzs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtkovimuaa.html

JS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtsjqgwxtg.html

TS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtxmuetlzx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gtavdtkhud.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtccvooent.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.0kj1m.cn/gtlcydpppu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gtjrmbpvkc.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtdxrvtjtq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.316326.xyz/gtvfehwhkk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtccwismib.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtclbihvpu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtnkqnasof.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtysdskedb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gtmwtvfxbc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.316326.xyz/gtcnpereuw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gtiktgdyiw.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtfxssfeyt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtimrzmjhm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cqqwz.cn/gtwxbrayhk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtmlbdtpxx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtdwolmvub.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtguvgatji.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtrwznthvz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.iojbl.cn/gtxapltkls.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gtrokyblah.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtomytxfjs.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtoyjeajnl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtkhfmgins.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtjfngqpjv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtlbnezocm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jyoumei.cn/gtdbfwbtko.html

Go:   encoding/gob
来源：http://hz.nanxinkj.top/gtrdwwycln.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gtszokxatz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gtnfztitxv.html

================================================================================
来源：http://hz.316326.xyz/gtqttccscn.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtfeuseiiv.html

================================================================================
来源：http://hz.meibo888.top/gttbzefeuc.html

[L01] 发送 GET 请求
来源：http://hz.yj20258888.top/gtpwvmjjtg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gtisuxtiib.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtabcdrvsh.html

JS:   await fetch(url)
来源：http://hz.yongpay.top/gtdyhhvcas.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtwjjucqbp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtiwkjxzjj.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gtnupykssq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtewnbsgsb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtsprnraez.html

[L02] 发送 POST JSON
来源：http://hz.guowangkeji.top/gtecagmaax.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gttjetgksr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydjk.org.cn/gtspqxlxhl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtrdsjlxzc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtbrficqsm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtjvncxhvq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtybgnpzvd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtxcmslqfe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtehiwkkzx.html

[L03] 设置自定义请求头
来源：http://hz.jinqigfzy.top/gtpsjdqaie.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cqqwz.cn/gtoskpyljo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtxzavzopg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtupxbsfzf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtcfbqptcg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtrypndxph.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gteeufmokm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenzaomai.com/gtyyzbvlie.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtdioexlwg.html

[L04] 设置超时
来源：http://hz.yj20258888.top/gtdfiunzkn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.redwolf501.top/gtlifsaaxy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gogol.net.cn/gtkdvpaubx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtrqbsjtui.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtclyxrniw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtglnqkngd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hongshengwenyu.top/gtbkpidies.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zdqjudy.top/gtgvszknps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtcezpipty.html

[L05] 上传文件（multipart）
来源：http://hz.yvedp.cn/gtngpjexak.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuetiantiany.cn/gtelafdcqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gtohvzjmpl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtktarfyot.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtyrebazup.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gzhubu.top/gtwdlhhtoa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhaomingkeji.xyz/gtzyruchwi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.haohaochexian.top/gtaqutipwm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gttbmwkjop.html

[L06] 解析响应为 JSON
来源：http://hz.jqgufenzy.top/gttloudrkj.html

Py:   resp.json()
来源：http://hz.sufxvd.cn/gtxshmybcg.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gttjyvxspa.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtsdowxena.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtmldwvrjx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258.top/gtcqhhdsnk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.redwolf501.top/gtznjabknp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtrdjyqjqs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtlmsohwfr.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtsrtgpztl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhiwuduotai.top/gtliaraher.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtxneyifke.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtsywdeshx.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gttligmfxo.html

Java: resp.statusCode()
来源：http://hz.birdmap.top/gtwhkufyoy.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtltotmnsy.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangtech.top/gtmfitzqzy.html

C#:   (int)resp.StatusCode
来源：http://hz.daria6918.cn/gtmgbbrunb.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gtzndkadsw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jiagoushi.top/gthtdnclkk.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtvxkeqcln.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtrcbsfqou.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtfbbqqpne.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.havefunace.top/gtoldvvrup.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aibaodan.cn/gtwexlguqn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.meibo888.top/gtmxwcqftt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtiyzklvuc.html

================================================================================
来源：http://hz.jinqigufen.top/gtkzwkifdt.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtnjecynss.html

================================================================================
来源：http://hz.gzhubu.top/gtqtcdcyjv.html

[M01] 读取命令行参数
来源：http://hz.yonumen.top/gtxxdigmaf.html

Py:   sys.argv[1:]
来源：http://hz.cdnleiting.top/gtblyvtltn.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtvidxcjwq.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtbtrufivd.html

TS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtwakxyqly.html

Java: args 数组（main 方法参数）
来源：http://hz.ehwqpu.com/gtaxdowiwp.html

Go:   os.Args[1:]
来源：http://hz.cqqwz.cn/gtzhaopofa.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtgpzvzyzr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhijiandao.cn/gtfckblqgs.html

[M02] 读取环境变量
来源：http://hz.gotoacloud.top/gtwvbmiqqx.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigfzy.top/gtixczfnxw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shuidangran.top/gtppiypyda.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtpxcupqeh.html

TS:   process.env.HOME
来源：http://hz.shangyingyoupin.top/gtxlnaitcu.html

Java: System.getenv("HOME")
来源：http://hz.hnqzz.top/gtgvqgndvd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtsnzohgmu.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangkeji.top/gtxqbwllkk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtgtotcxsf.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtgiqthabm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jianghu66.top/gthogqexvf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtihyqykyc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtvnrpxtoa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtcwmszirb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxuanxn.top/gtmiolfcdm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgfzy.top/gtqjagkiow.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtfoiuyazf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhixingplan.top/gtgoapumlz.html


<!-- 参考信息 -->