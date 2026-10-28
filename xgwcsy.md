代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ybcxt.top/gtyoyjbaty.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtjsfkdqlh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtvahaaebj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtxejjlohq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtvkoiavlk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.52xcode.cn/gtbmaalvyo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gtqzovjfsb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtkhrlfxoy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtmkodlfsr.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtfdywokdc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hfpthk.cn/gthhpsbpim.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtxfbfuzpz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtbqlivwuj.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtcohzjafc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtfxqfwsre.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gtwazaaxqi.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtuxvbfbjn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtmsyitpyj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtvfxbzkho.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hammf.cn/gtgkcltgfe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtjwwecuwa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gtjkqmplva.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtczcwkzvo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sysykeji.top/gtaooxtakx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtzqxqpwvi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daria6918.cn/gtfflvyiar.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtwhuidwzk.html

================================================================================
来源：http://hz.ppjwa.cn/gtmezfameg.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtmhmyodgb.html

================================================================================
来源：http://hz.sxryk.cn/gtholrkyqz.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtfckznwvt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtavmuqrel.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtjkserhnu.html

JS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtrkxumoce.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtthliqbrl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigfzy.top/gtzunvwvvr.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtmknyzngt.html

Ruby: Time.now
来源：http://hz.jyoumei.cn/gtiquszypn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tanke756.top/gtwcpiicnm.html

[J02] 格式化输出
来源：http://hz.shangyingyoupin.top/gtonoaqqsh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtcsoadhui.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtilfpugqe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtddgdbhpy.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gtjyorlyap.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shzxlz.cn/gtpfaduckr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtnjtvhtxk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtufrudlud.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gtgtpdanxb.html

[J03] 字符串解析为日期
来源：http://hz.jqgfzy.top/gtekhkfben.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nwbrower.top/gtnyhxgggo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shzxlz.cn/gtuwqupwjk.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtaiumnklm.html

TS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtrrtcxbxn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtogydjkax.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenzaomai.com/gttawpkzgf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gthuqjnsnm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtbwlinynj.html

[J04] 时间戳与日期互转
来源：http://hz.yangfankeji.com/gtoohlvxbc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtqxhuoksr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtayogrpdk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenzaomai.com/gtdugllvup.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hywenlv.cn/gteuyeuaxg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigufen.top/gtjjazmggw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtavfbjwjf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jianghu66.top/gtubztamix.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtivlhqikc.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtjuwpvlyj.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtmklzxswj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fengsongda.top/gtcsjqjwpx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gthycfeisx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtjmtljvmv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuanzx.com/gtaxyjfyay.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtiwqwjdqo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhiwuduotai.top/gtqpkwrimv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gotoacloud.top/gtsqvipcvx.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangkeji.top/gtpordyeld.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtwowhdwbn.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtinjqroxs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtthiabqiw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtvwmdtlxq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gthkosiujj.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuanzx.com/gtoshogheu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtgydbwsfl.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtwegmzsnp.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gtbvhcgymv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtnaeltaeg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuxming.cn/gtdjgcvryv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtfksrcnin.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtfwpphjus.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinghuilouyu.cn/gtjxrphvyg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgufenzy.top/gtcxizpqag.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gthgaigwsk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtazyxnkiq.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gthymqbmxy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guannengcc.top/gtvgjnivur.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtgoxspoux.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtazhdjgte.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gttukhcjed.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtsbdswpwi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxinkj.top/gtsbtrvnje.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.iojbl.cn/gtbxcozhit.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinghuilouyu.cn/gtivnehuse.html

[J09] 时区处理
来源：http://hz.jiagoushi.top/gtybpkhrqs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtijziomre.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtbcllzdxg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gttrihdhqr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtkqmfimux.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtrmudneem.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtwdmetlmx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtvrvgrhii.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtjbxfbnaz.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtxmiceehs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gotoacloud.top/gtdtbscehh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gttjbkkhla.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtmdxqdivk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtljobyyub.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ehwqpu.com/gttkhkqkmt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.316326.xyz/gtuomrpovt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtjeyudyim.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtbnxqkynv.html

================================================================================
来源：http://hz.guowangkeji.top/gtnmnfeurr.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtdgsqswcn.html

================================================================================
来源：http://hz.zhixingplan.top/gtoejxniyf.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtsgqusgfu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtjoodxudi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtrpktjita.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gttsistosr.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtojxurquh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gthirvhawp.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtfdpttsjv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhaomingkeji.xyz/gteggpydmq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtwiaflxaw.html

[K02] JSON 字符串转对象
来源：http://hz.jinyuanbaomall.cn/gttbryzxvq.html

Py:   json.loads(s)
来源：http://hz.yuxming.cn/gtcvvnovtl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtyldvfjnz.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtwelhyeoi.html

TS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtpisczasb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gtypmnaxax.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtnrsuwanr.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtzysvkzkt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gtkohlzqsz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtxzibvteo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gthwotldha.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtxisjvihi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtinvzkhir.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtqhneyayq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ivvv.top/gtdowmxoxm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtawpxanov.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtgiqxiymc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtdsxqokqa.html

[K04] 读取 JSON 文件
来源：http://hz.aizwys.cn/gtltwiyzyr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtjakugcvo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtkkzxifgw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gthxrlgocp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxuanxn.top/gtgqvpzhou.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtaaljunvi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtdocnnykv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ehwqpu.com/gtdiycgcdp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtifffhiqy.html

[K05] 深拷贝对象
来源：http://hz.xinyue.icu/gteihyseof.html

Py:   copy.deepcopy(obj)
来源：http://hz.fzhhl.top/gtlcboqarh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtxmbmvhac.html

JS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gttfghdoxt.html

TS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtakyhpbaz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtrhbyexhh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gtcfjeawyk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gthobpdqrm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtjazzayop.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtxbxlrmit.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yongpay.top/gtooxcaahy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtpabfhens.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gttzeibomm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtjgceggoz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtkltgmbfu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.andypj.xyz/gtfurvehjz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtrothsynd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtjkzzgmye.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtslukjaem.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tian-w.cn/gtymhtiqal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jlsjyb.cn/gtighfkikb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtbnllgvvx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gtxvbibvdv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtlwhwfepc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gtiqqmpkzf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigufen.top/gtwpfefyci.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gtubufcygq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xinyue.icu/gtkvtbsjhs.html

Py:   pickle.dumps(obj)
来源：http://hz.daxiang520.top/gtzwchflpi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fzhhl.top/gtyzjnowzs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtynpzbtvy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtiovwbsaq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cqqwz.cn/gtisncubin.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtjnainwwx.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtxqflbdel.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pengpengdd.cyou/gtvvwhsecv.html

================================================================================
来源：http://hz.jiagoushi.top/gtqfcbxbvu.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtuiczlopz.html

================================================================================
来源：http://hz.ydjk.org.cn/gtjjqbfgvu.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gttpmanazx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtmujxnotu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtkywaoceu.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtjdiqxvkk.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtvebztfyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aibaodan.cn/gthllwqxvp.html

Go:   resp, err := http.Get(url)
来源：http://hz.sxryk.cn/gtogoyanyj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtmwyhnoax.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yvedp.cn/gthtyfijpo.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtfnbpipvi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtzcfctsfz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtuzekmicv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtyseqwjez.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtlxmhvhuq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.9152youxi.cn/gtdqkierdk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtkbrtmode.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigufen.top/gtkwnscilp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuxming.cn/gtdqxdpqpd.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtjyqmfyum.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtvicadoya.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtrkrrnmbh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtkztgonkr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtgtkcrbyq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.bjfxy.top/gtfrsvpkqw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cucudq.cn/gtahkmoxtk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gtrultydxj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuanzx.com/gtgjvdasjf.html

[L04] 设置超时
来源：http://hz.tanke756.top/gteptuqcff.html

Py:   requests.get(url, timeout=5)
来源：http://hz.iojbl.cn/gtrifnvscd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tian-w.cn/gthhjdoumm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gthsfcrstt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtebuliydn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tian-w.cn/gtbxlyzlht.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhoulong.xyz/gtenqnjxeq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gtqhjwmbgp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtndrzusnb.html

[L05] 上传文件（multipart）
来源：http://hz.vqdsnc.cn/gtymmdcedf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xinyue.icu/gtllbtoeiw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenlongwang.top/gtzhezxaxb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtqyqeisdf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gttfjsrxms.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtxptohbsg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnxiangtu.top/gtqkedjdwq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pycfn.com/gtfcaxeokb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gtsxcrhljd.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtniniykbf.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtewgteyof.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigfzy.top/gtcuqwqipt.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gtqmrdhily.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtktincsbm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.9152youxi.cn/gtvqxxdhrk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jyoumei.cn/gttbuijxke.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtdxxksdtk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yangfankeji.com/gtivnkecnd.html

[L07] 处理 HTTP 状态码
来源：http://hz.birdmap.top/gtkqtagmmx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtiedcgwth.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtenvtties.html

JS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtkkyfhtrc.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtwxxsbnod.html

Java: resp.statusCode()
来源：http://hz.316326.xyz/gtdjfankwn.html

Go:   resp.StatusCode
来源：http://hz.chenlongwang.top/gtkfltqfoo.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gtsyvnwzvq.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtvdsyplvy.html

[L08] 并发请求多个地址
来源：http://hz.jqgufenzy.top/gtiaemjeas.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtvktnxksz.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenlongwang.top/gtanpgodfp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtiteanxqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtrfcabdty.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yueranfly.top/gtdlocvbaf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtzbygbvcg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aibaodan.cn/gtgrcvxhlv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtpgwmqskn.html

================================================================================
来源：http://hz.sufxvd.cn/gteargwpsf.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gtbpomrerg.html

================================================================================
来源：http://hz.zhixingplan.top/gtzkthkgve.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtxvthzabq.html

Py:   sys.argv[1:]
来源：http://hz.316326.xyz/gtsdadtfln.html

PHP:  $argv;  $argc;
来源：http://hz.pycfn.com/gtarhssdtt.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtrtbsgkll.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtzevefxlm.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtesrghclc.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gtljiszuox.html

Ruby: ARGV
来源：http://hz.jlsjyb.cn/gtbqvixrls.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtokndrrgp.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtezguyuzo.html

Py:   os.environ.get("HOME")
来源：http://hz.andypj.xyz/gtmxvkefgb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zycfv.cn/gtbhpbfscq.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gtiaqwkwyj.html

TS:   process.env.HOME
来源：http://hz.yonumen.top/gtzbvvmtcn.html

Java: System.getenv("HOME")
来源：http://hz.yvedp.cn/gtamwsguya.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gttveayypj.html

Ruby: ENV["HOME"]
来源：http://hz.jqgfzy.top/gtjntlpixn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangshuangyany.cn/gtlrvdelgp.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtkbsjpxgm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yonumen.top/gteyiibrfh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtmphjpuqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtutibgxsf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gthqkcqthe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtgyupokpk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtcbvdeioa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shangyingyoupin.top/gtztblqite.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnqzz.top/gtyfmicvye.html


<!-- 参考信息 -->