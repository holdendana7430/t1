代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.pengpengdd.cyou/gtwrvpemma.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.havefunace.top/gtudbodqza.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtywucgzbm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenjidiqi.icu/gttuqokwjs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtblklgaad.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtjltwafle.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtruaicchu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtddvpmlzs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtrpadnitw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gtxmgknakp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shuidangran.top/gtreowumwc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gtcmokwxal.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtanshaobs.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtbaolbxny.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtfrwgzgno.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtqdwzarxb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtompyymmd.html

TS:   /error/gim
来源：http://hz.sufxvd.cn/gtbcasntxt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gtvidblpcf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtxthilwlj.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtddpwuybg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtpkklqpsd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gtgsvzcztf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ivvv.top/gttopmqdra.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxinkj.top/gtooglshqq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtvxwuorlw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtqiedkcgp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtbjmfolnw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgufenzy.top/gtjnrleswg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtnldhimez.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtcrmkffhw.html

================================================================================
来源：http://hz.tian-w.cn/gtkcqjiobq.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtymfuryvq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtosrwcwkv.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtabwsqige.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aibaodan.cn/gtdiasltxh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtxxwfvxpq.html

JS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtnfzcyccr.html

TS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtujoecpes.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnqzz.top/gttbtrryrn.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtxecnsbbn.html

Ruby: Time.now
来源：http://hz.nwbrower.top/gtnwrjixvl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gtvsiyclhd.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtrjsdzugt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtybsblhst.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtqtcmwuqf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtyeavnanu.html

TS:   d.toISOString()
来源：http://hz.svipenyu.cn/gtoiimiwpa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtqmvcgprw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gtcrrtneqz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtrsttemda.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtbtwwtzfg.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtdseegklh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yonumen.top/gtrgjykzmb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gthtxwhspv.html

JS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtgcuhdsca.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtzblfoxgk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtndwxhwtf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daxiang520.top/gtseerwmac.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pycfn.com/gtquzwbmje.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuxming.cn/gtpnzzmzlv.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtseywttqc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtylpvzzvf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.redwolf501.top/gtuveuidqe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.52xcode.cn/gtkndwhtef.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gtzkegoewf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.52xcode.cn/gtwlqxhhwq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gttjmubdox.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ehwqpu.com/gtqrlmofbb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnqzz.top/gtqfdmcnui.html

[J05] 时间加减（加 7 天）
来源：http://hz.bjfxy.top/gtqbzwgfzn.html

Py:   now + timedelta(days=7)
来源：http://hz.wangshuangyany.cn/gtmmtkvojj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dashuyun.cn/gtijtkuifm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtcxkpwfij.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtsfffnsxa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hysaishi.cn/gtpioalseb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gthgeqinir.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtwjojzuyc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtnydcncku.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtukvrwkln.html

Py:   (end - start).total_seconds()
来源：http://hz.vqdsnc.cn/gttvbfepoi.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtqkajzidb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtiusecxhj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sufxvd.cn/gtotiwcuha.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtlzcvvyve.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtoavrdjqq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtivujsmob.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gtryixdghx.html

[J07] 比较两个日期
来源：http://hz.guowangkeji.top/gtwkoauzfd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtuaketqbv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.52xcode.cn/gtwlpeiyrc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtunatpejq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtytusrmui.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yonumen.top/gtobxrthqu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtolvvnkkz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtrfitdxcz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtdxrwlhrb.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtjkynompj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtkeaawgon.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtziojzlhi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zycfv.cn/gtalwwwatg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hysaishi.cn/gtlizmohnn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtsxquaaum.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shangyingyoupin.top/gtpgpixgek.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtrmcryqpy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtwwbminli.html

[J09] 时区处理
来源：http://hz.haohaochexian.top/gthjnjhcgw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gturtsffnp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.9152youxi.cn/gtuosgbjxa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtwuszbpqv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gteixhbasi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gthhlctwwg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtrkmzfxci.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtupqphuqf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtcjolwkls.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtsewfazzn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sweek.top/gtgpxsiuia.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.feifeiyinyue.top/gtapzdtzcw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtqjliyigs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gtnjjgcpte.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.iojbl.cn/gtnojyazad.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtiwfkwtrv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtzqzdmesr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.c1oappe.top/gtktunjica.html

================================================================================
来源：http://hz.xziqi.cn/gtmauphvus.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtdbtujbvp.html

================================================================================
来源：http://hz.aibaodan.cn/gtuicggnsc.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuanzhike.top/gtwxniqgid.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gttpryqkch.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtnvwcavww.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtdnftyyyu.html

TS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtrnjmzorn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtfedrlowg.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gthogkgyms.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.vqdsnc.cn/gtfphhlhxx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtsutxnoog.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gtxlvpklbo.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gttzqqegyi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgufenzy.top/gtyshkqnui.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtedkoxiix.html

TS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gttqappnml.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.smart0.xyz/gtkgurfigq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtkbgiqydj.html

Ruby: JSON.parse(s)
来源：http://hz.guannengcc.top/gthgnswhmn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258888.top/gtdjarohgc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtfouaicvz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtipomnqyn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtnkwjpnww.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtrbdkrzxb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtheqtnbrw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gteougofuc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gotoacloud.top/gtscuuxjwy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yangfankeji.com/gtwztdronq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gthjedxmnt.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtzqvnstwg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtqdodbyjj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtwsvrakif.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtuckynueg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtgslovybt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydzc1.top/gtabjdzdbi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtrdeblfpm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtvnzhpjew.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cucudq.cn/gtchpvodij.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtqwqjqeyv.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtinjzueur.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daxiang520.top/gttatqkaec.html

JS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtokzetwdo.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtlkeafmun.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tian-w.cn/gtrogzfacb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtbcwbghjr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtztkxmnlf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtrvkkuvgu.html

[K06] 解析 URL 查询串
来源：http://hz.wangdashe.top/gtcuwcxeup.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gtyjwhmkdh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtuhyoylzx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtsvymjbfw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtwbbcibds.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtppmpwlfe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.svipenyu.cn/gtwkgwraav.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gtopaiaxuk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtbnqjhdvf.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtoumyghdv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtjvnaqfhp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jlsjyb.cn/gtmftpvxka.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtofzdsggy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtscmiuzbf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtozpaimpu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtzybmwmeq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gtjbuyyxbe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.feifeiyinyue.top/gtxxtymybk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtmtyrwhqx.html

Py:   pickle.dumps(obj)
来源：http://hz.snrcjt.cn/gtfplyirrb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuanzx.com/gtcqncfgli.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gttnhyqabr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gtgdatugtn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cheryme.top/gtieqnrnre.html

Go:   encoding/gob
来源：http://hz.yuanzhike.top/gtokcopdas.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtswnomngy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhixingplan.top/gtbyxjiydz.html

================================================================================
来源：http://hz.xinyue.icu/gtcqqftanh.html

L. 网络请求
来源：http://hz.daxiang520.top/gtuvdwvney.html

================================================================================
来源：http://hz.xziqi.cn/gtlereslmm.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtqyfavttp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gtmhzpluav.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtgdqkawlt.html

JS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtqhbqjdxb.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtmvptcauo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtpsliufte.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtigvbzjok.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtpzdkmuyc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtpusvckiu.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtxwqdbkns.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhiwuduotai.top/gtonezxuef.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gzhubu.top/gtqxfqeepc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtfclpujcy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtzthbplkf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenzaomai.com/gtskokmttl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.andypj.xyz/gtfugpveld.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtsgnkjiaj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.birdmap.top/gtynvobvvg.html

[L03] 设置自定义请求头
来源：http://hz.shangyingyoupin.top/gtvirgkoze.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jianghu66.top/gtukealret.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgufenzy.top/gttgvovvfj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtratyedqa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtbremrlqp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.haohaochexian.top/gtfvzysmva.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtanlvazjk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtqkilgzgl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtzujjtvet.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtahvalrjt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuxming.cn/gthgoddgga.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigfzy.top/gthqjlvhxr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtwuppubzu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gthfjzahzp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gtbwzemrhu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtwxoynlxd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sysykeji.top/gtxvpjjyjf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtgombzgbr.html

[L05] 上传文件（multipart）
来源：http://hz.hnxiangtu.top/gtapotdapr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtrxowxylz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xuetiantiany.cn/gtcuskfjec.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtfsbqdcwo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gtmiykaboe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtmcbffarr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj202588.top/gtctcgsvlh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hammf.cn/gtlicmrynb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtejbeknsd.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtjehvhbjl.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gtsuyuuyuy.html

PHP:  json_decode($body, true);
来源：http://hz.pycfn.com/gtcgjokluv.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtfutvskmn.html

TS:   await resp.json()
来源：http://hz.guowangkeji.top/gtcnmxrghm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtqxmcxnal.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtykqizyve.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnxiangtu.top/gtnozesixa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtaiaubxov.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtqqjgiqdu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydjk.org.cn/gtdktvpgnt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtuysaduwb.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtkwdvnbga.html

TS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtaugnfcsf.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtkvbplyye.html

Go:   resp.StatusCode
来源：http://hz.yangfankeji.com/gtzzkwvoex.html

Ruby: resp.code.to_i
来源：http://hz.yanxiufei.cn/gtmruznhnp.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtwjxkkmkl.html

[L08] 并发请求多个地址
来源：http://hz.pengpengdd.cyou/gtccpgqxbb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtmkcrsibc.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtqhfpaqiz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtycjwslnx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtsyroqlde.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtobcjuonh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenlongwang.top/gtgofyywzl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtwehpsjew.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gtcxkksmhh.html

================================================================================
来源：http://hz.xziqi.cn/gtzbgxicrw.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtbgqjqipv.html

================================================================================
来源：http://hz.sysykeji.top/gtddqpxhai.html

[M01] 读取命令行参数
来源：http://hz.pengpengdd.cyou/gtnqqjsgzg.html

Py:   sys.argv[1:]
来源：http://hz.52xcode.cn/gtnpzfkjbc.html

PHP:  $argv;  $argc;
来源：http://hz.hysaishi.cn/gthtysdqhy.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtrhoszrlq.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtbwfdbihp.html

Java: args 数组（main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtxawbiujk.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtwzexcqhh.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtbprqahim.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jyoumei.cn/gtorevqymn.html

[M02] 读取环境变量
来源：http://hz.tian-w.cn/gtvutozoyz.html

Py:   os.environ.get("HOME")
来源：http://hz.zhixingplan.top/gtcaqbprpj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhoulong.xyz/gtpmscmspv.html

JS:   process.env.HOME
来源：http://hz.zycfv.cn/gtmrifixpm.html

TS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtqzkbgjkj.html

Java: System.getenv("HOME")
来源：http://hz.iojbl.cn/gtkiudfxux.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ivvv.top/gtsefublss.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigfzy.top/gttrkvdora.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yangfankeji.com/gtebxrkckj.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtsdeprrrf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtwlvxmoup.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.andypj.xyz/gtnfhiegvs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zdqjudy.top/gtfakzhfwj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.daxiang520.top/gtkxhdvmub.html


<!-- 参考信息 -->