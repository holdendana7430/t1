代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gtennalard.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtpkybuydg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtgdtgiipx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtpiomwlmn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtmphmfkpt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtllqwffqz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtxpoxiwss.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gtuiwkwdcy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtnzjzymld.html

[I07] 忽略大小写与多行模式
来源：http://hz.jianghu66.top/gtbsysendo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xylfe.cn/gtjzssipkq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daxiang520.top/gtwohtshjt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtsbjgkvax.html

TS:   /error/gim
来源：http://hz.dianchejie.cn/gtuvbgwcav.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jyoumei.cn/gtehvpmfaa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yongpay.top/gtjfjscqnv.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtlaynvgst.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtmmcvpoka.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gtuhueklpy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhaomingkeji.xyz/gtmplwzomb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxuanxn.top/gtzlfetavg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtvilywazn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtkpuveszq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtahozshqd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinghuilouyu.cn/gthlpwjhoh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtkanwbnmn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtfboqaxwr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbpcxrxek.html

J. 日期与时间
来源：http://hz.shuidangran.top/gtabvnssur.html

================================================================================
来源：http://hz.0kj1m.cn/gtyaloxjnb.html

[J01] 获取当前时间
来源：http://hz.pycfn.com/gtgukhlkln.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtitzfskgw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtcgdtvczu.html

JS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gttsmbaldf.html

TS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtfqnxtlmb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shangyingyoupin.top/gtaiqccqmf.html

Go:   time.Now()
来源：http://hz.jyoumei.cn/gtcphdwsqx.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtlfmrzuox.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtxeyvoisq.html

[J02] 格式化输出
来源：http://hz.kuanghao11.cn/gttizfmamo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gthgnxfjbo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtujrtspxt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtiymtpiez.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtxfsyboor.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigufen.top/gtzdrcndzn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtepouxjug.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtdjmwqzlh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtqbhgmufo.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtuxmjxcum.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cdnleiting.top/gtfthgdwje.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cheryme.top/gtgtfsxdnx.html

JS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtinxpteir.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtoulaomqj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gttodjbmqa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtyivyhyec.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtwsoqdwei.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtsscyzjle.html

[J04] 时间戳与日期互转
来源：http://hz.cucudq.cn/gtwnpglhbq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtfgcsrlus.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daxiang520.top/gtccscpfui.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.meibo888.top/gtsyqgkdus.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhaomingkeji.xyz/gtdpkomszi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtjlvcebhf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtgwqcopon.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnqzz.top/gtahxpnghm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtrieterha.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtozyggisb.html

Py:   now + timedelta(days=7)
来源：http://hz.hnqzz.top/gtfjglvcwh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.c1oappe.top/gtpwdgfylv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtdzhnajpj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtxeutzype.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gtwybmtkdi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtsciigiks.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yangfankeji.com/gtqcqigspf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtfoqhdhvw.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtfecielon.html

Py:   (end - start).total_seconds()
来源：http://hz.chenjidiqi.icu/gtodmfsvsc.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangdashe.top/gtuwtzwlsg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gthhxmsghw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhixingplan.top/gtfpmrubrz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guowangkeji.top/gtnxncsjcc.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtudoegqux.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydjk.org.cn/gttysehumu.html

C#:   (end - start).TotalSeconds
来源：http://hz.meibo888.top/gtrpbkxfew.html

[J07] 比较两个日期
来源：http://hz.cucudq.cn/gtmodovixt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtwidvvbrk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zdqjudy.top/gtwhlrmfoi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtnogzilvv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtwjuzonox.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ppjwa.cn/gtbrsouhbs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jiagoushi.top/gtezotjnfy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtzzizyswf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtkaeauvlv.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtpnypxsuj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtmgoklbkw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtjrbddqis.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtsxpalxlb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtgwziayfo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtyimjvwnv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhaomingkeji.xyz/gtmgfbecix.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtwedosxef.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtayqrills.html

[J09] 时区处理
来源：http://hz.tian-w.cn/gtsytlexyg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtbrsflgib.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.smart0.xyz/gtmllishta.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtucnhboct.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtoaoxlxay.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.c1oappe.top/gtvajdibjo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtkptrdvbh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtmymccrkx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gtyqycwngu.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtbavsgnmq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.bjfxy.top/gtacrverru.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtusjtiesj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gtmzzerkwt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtuhdextyd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtrbvuoyfs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.snrcjt.cn/gtnaoxmnos.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtkuyzoagi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ybcxt.top/gtveozwwrw.html

================================================================================
来源：http://hz.hywenlv.cn/gtyzzcpvqx.html

K. JSON 与序列化
来源：http://hz.yangfankeji.com/gtrxkhxiir.html

================================================================================
来源：http://hz.nanxinkj.top/gtdxlgglxg.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gthyycrpwu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtulprbrue.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtzmwrvjxa.html

JS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gtfjswwoku.html

TS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gttvuzidkr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jianghu66.top/gtuzsndykl.html

Go:   json.Marshal(obj)
来源：http://hz.redwolf501.top/gtvueyadwh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtkeyuyimg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenjidiqi.icu/gtljgltmmy.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtreafsdnv.html

Py:   json.loads(s)
来源：http://hz.yueranfly.top/gtyjkupfqm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtredjbmoj.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtcdawugwt.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtuwqyejpa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenlongwang.top/gtivrpfsug.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gthzwilasa.html

Ruby: JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtdykztcbl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtqikuqhsb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.316326.xyz/gtokhuhgiv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tanke756.top/gtizpnzrsv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtaqnepqgu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtylmgizav.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtcjqarcpu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gthsihmktb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tanke756.top/gtmslxxzge.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtampcnvkx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gtrfzredky.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtagnxxuqj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtyeqrnrie.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtxyhwsaqe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtllgeiweo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtrxjneghx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj202588.top/gtjewlfbna.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gtlujxgfcn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258888.top/gteeyvffas.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtrutofkyx.html

[K05] 深拷贝对象
来源：http://hz.jianghu66.top/gtnrbntxlc.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtdupmpsmc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sxryk.cn/gtxwzzilmt.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtjoylxtkf.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtnueyfanl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigufen.top/gtmkfirfdp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtpzxkqvwv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtpplrqdej.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xziqi.cn/gttwxufnsh.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigfzy.top/gtqbfkehlm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xinyue.icu/gtzltvltue.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtftyaiqcl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtmkhamaze.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtkotphamd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtumbnlasq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtukcecwfn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtffrchfdz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtganuclue.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtgwwnpdek.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtvicwzsdl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtltwaebym.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtgvzfibxb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtoqqusjva.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtruornrcp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tian-w.cn/gtlzbuzebs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xylfe.cn/gtupmxjbjr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.c1oappe.top/gtbmzpxdzq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gtbdighjfu.html

Py:   pickle.dumps(obj)
来源：http://hz.tanke756.top/gtokreaoog.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtkiuqqgst.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtafizyzzs.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtrugsaldx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtmhhnhdkz.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtxofdxlct.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinyuanbaomall.cn/gtoqjqvewb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yonumen.top/gtegwzviyf.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtizbihfga.html

L. 网络请求
来源：http://hz.shuidangran.top/gtsswchemi.html

================================================================================
来源：http://hz.sweek.top/gtanrapwsr.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtthrcauvc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shuidangran.top/gtsaxzkunb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtavdzevit.html

JS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtzswrxlnq.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gteebepnuq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gtqyvugsrx.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj202588.top/gtgwqphtqi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtbwpagyun.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtdovwysjr.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtqqqvshsv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtzkoieyuf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tanke756.top/gtyzjabukj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtouyvxotf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtjlmhvqlv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.birdmap.top/gtzdwrtxtl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cqqwz.cn/gtziknjpdi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hywenlv.cn/gtunvuhtvz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guowangkeji.top/gteqshczyy.html

[L03] 设置自定义请求头
来源：http://hz.chenzaomai.com/gtbkgxihtq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shuidangran.top/gtyohoidgh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtyfkbvrki.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtmkgliexy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtwczbange.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxinkj.top/gtzflspgfz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gtbfgabhjr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtptgrxuzc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtvkegmfzc.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtcxdzgvhc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ehwqpu.com/gtyqtvmjnz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtsuengrof.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtheorknlc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtphxuegsy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhoulong.xyz/gtyttfceja.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guannengcc.top/gtqlixyxii.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.0kj1m.cn/gtlyhrrswo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtgxejkcfa.html

[L05] 上传文件（multipart）
来源：http://hz.guannengcc.top/gtzacngcde.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangdashe.top/gtybxlqqpo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtpzbyinol.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gttrkhddbs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gttrcfogzg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hammf.cn/gtryakttij.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fzhhl.top/gtkthbghyx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtuzkuuzaq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenlongwang.top/gtzcxyzwze.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtelpgcjjl.html

Py:   resp.json()
来源：http://hz.ydjk.org.cn/gtfbcqbnjy.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtzbtlysve.html

JS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtmvhkqvmx.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtztrshxjw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtocrkkavi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pycfn.com/gtchbhbcil.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zycfv.cn/gtxskcrhdb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.9152youxi.cn/gtkawkesnt.html

[L07] 处理 HTTP 状态码
来源：http://hz.cheryme.top/gtzqehwliu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gtedjckybf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtgciflosw.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtxwaszrbw.html

TS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtblizojwv.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gtndlvtdrf.html

Go:   resp.StatusCode
来源：http://hz.vqdsnc.cn/gtlpomohhn.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtazqcnees.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtfzwkldyh.html

[L08] 并发请求多个地址
来源：http://hz.aibaodan.cn/gtgjloimcl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtnfnkhpxw.html

PHP:  curl_multi_init() 系列
来源：http://hz.iojbl.cn/gtzutawpnm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtqxktxxen.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtktrvrfyn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangshuangyany.cn/gtyjnmbubc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtthidlwxu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gaohongyu789.top/gtzsxkhydm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gtyrvffsec.html

================================================================================
来源：http://hz.9152youxi.cn/gtfraosuiz.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuetiantiany.cn/gtsgqcnjfo.html

================================================================================
来源：http://hz.xylfe.cn/gtsgbpsyzb.html

[M01] 读取命令行参数
来源：http://hz.daria6918.cn/gtytwgbsju.html

Py:   sys.argv[1:]
来源：http://hz.shuidangran.top/gtexnteuyj.html

PHP:  $argv;  $argc;
来源：http://hz.zhijiandao.cn/gtlaqtdgth.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gthzbaflxe.html

TS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtekvwamyz.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtpyqjulva.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtijkijgse.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtihzlbzao.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtpcrwayfu.html

[M02] 读取环境变量
来源：http://hz.ehwqpu.com/gtmplfscrh.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gthtuntveq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtetxvaoqc.html

JS:   process.env.HOME
来源：http://hz.316326.xyz/gtxbvgygbh.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtvrbmhxio.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtonlgplry.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtocpxvcgq.html

Ruby: ENV["HOME"]
来源：http://hz.yonumen.top/gtuyqhtysx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtgoqfvpqw.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gttfjekhxg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtoujbcyft.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sxryk.cn/gtkyjsapmh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtiyttlxhq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtzhbxxexl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xziqi.cn/gtydzwzrwt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtlyzpsdvf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydzc1.top/gtlwvhthus.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nwbrower.top/gtbguqntcj.html


<!-- 参考信息 -->