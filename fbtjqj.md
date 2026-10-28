代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtfdsehqxo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtvwrelqxj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gtyacingmo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gogol.net.cn/gtgiucblcd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtgiukveet.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtnbuuvmyr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yangfankeji.com/gtgwjnmgit.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gtbzkdnexm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuetiantiany.cn/gtorremnqx.html

TS:   /error/gim
来源：http://hz.gzhubu.top/gtxbwypnak.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtzyayppaj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gthvhtoqkx.html

Ruby: s.scan(/error/i)
来源：http://hz.svipenyu.cn/gttixdwbne.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ehwqpu.com/gtmfqhgswb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jlsjyb.cn/gttkrwfobt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangtech.top/gtfgvulfgx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtqdbtsirc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtgrhkdefj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtlxyeuygy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtiiptoshq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigufen.top/gtcspttszu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.andypj.xyz/gtwjarqwdl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gttvrqyomv.html

================================================================================
来源：http://hz.xinyue.icu/gtrtvidfyq.html

J. 日期与时间
来源：http://hz.meibo888.top/gtzwvnsbrl.html

================================================================================
来源：http://hz.jiagoushi.top/gtgmjffemp.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtngstqrbn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtoradwbvn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gttdelgsta.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtrsradrdx.html

TS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtxvbilrnu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shangyingyoupin.top/gtcwxghblr.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gthpohcdfq.html

Ruby: Time.now
来源：http://hz.gogol.net.cn/gtplgaqrac.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.feifeiyinyue.top/gtsswuuijo.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtbxbcecgs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtukzjjgka.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtyecbppso.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.haohaochexian.top/gtsyemxzaj.html

TS:   d.toISOString()
来源：http://hz.xuetiantiany.cn/gtrbjwvkzk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.haohaochexian.top/gtfsxcnmpe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gtobocfnbt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gttxzewjwo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtzeiupbpr.html

[J03] 字符串解析为日期
来源：http://hz.jyoumei.cn/gtptzpalor.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenlongwang.top/gtrzysbrsw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigufen.top/gtaqzygxbx.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gttxutghzo.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtzerfexrg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtmztgvpwb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtfflguirn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtiklrxovt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtwwzjklrn.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtuxifmctb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gtxzdahlsd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gtaudguroa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtvubkfjxc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gthhjidhfw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtirptdhpw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtwzfzuuik.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgufenzy.top/gtcsjtayyy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sufxvd.cn/gttsemxqpe.html

[J05] 时间加减（加 7 天）
来源：http://hz.hfpthk.cn/gtjhllmwaz.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtijpdwsgu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gaohongyu789.top/gtpaikbxka.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtbjlamuuj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gttpmvslax.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ywan-chungtsiang.top/gtnlqrerjh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gtlourvsnt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtgkjewima.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gzhubu.top/gtlvpumgcj.html

[J06] 计算两时间之差
来源：http://hz.jiagoushi.top/gtrftmhgsw.html

Py:   (end - start).total_seconds()
来源：http://hz.hammf.cn/gthimntjwx.html

PHP:  $end->diff($start)->days;
来源：http://hz.smart0.xyz/gtbiseywzv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cucudq.cn/gtpyoadixy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtexsloahr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangtech.top/gtpakgpczz.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtnonrryms.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtglpzlbsn.html

C#:   (end - start).TotalSeconds
来源：http://hz.52xcode.cn/gtzlucrzmr.html

[J07] 比较两个日期
来源：http://hz.yj20258888.top/gtvuulfuue.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtfiyqdydp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtuwgkwiva.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtjzzegrkg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtdxiwilrz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtacbntxkm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtyqipikpy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtvvewmpju.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtctkivzfn.html

[J08] 提取年月日与星期
来源：http://hz.jqgufenzy.top/gtlretprta.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinyuanbaomall.cn/gtrxpaazwn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ivvv.top/gtoytntqhz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fengsongda.top/gtarfkruev.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtvrhansrj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xylfe.cn/gthnabhxfj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtmhpfkrco.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fzhhl.top/gtbeakuyyj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtsjzlsids.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtkehsggok.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinyuanbaomall.cn/gtswdrbihd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxinkj.top/gtbwuhorve.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtwyyxdahm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtfwupyvje.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtflvajtol.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gtgeclyodu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtoyvxmmhf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.pengpengdd.cyou/gtgifeetkh.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigufen.top/gtaatzefmz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtiemcdycv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtfuucdzqp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtoupipsnb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtyipomrya.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gtgpuljwau.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtvpsnsfmn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hongshengwenyu.top/gtzejlhcfn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gtentctoga.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtsckfrfmx.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtijddlspc.html

================================================================================
来源：http://hz.gogol.net.cn/gtzyrtxlfr.html

[K01] 对象转 JSON 字符串
来源：http://hz.yonumen.top/gtvilqlzts.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtgkeaaext.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtejgwyifv.html

JS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtyoefvhcv.html

TS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtmovntaxh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtgyrtlcbq.html

Go:   json.Marshal(obj)
来源：http://hz.yvedp.cn/gtlztcrtys.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258.top/gtvzzypyxf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtjtdgrlha.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtvhzalhdk.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gteqzwhmyk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhongyouzk.top/gtdaboooyx.html

JS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtylnzgodr.html

TS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gthffhmpwv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hfpthk.cn/gtjeijzsmd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtyaskcmpl.html

Ruby: JSON.parse(s)
来源：http://hz.dianchejie.cn/gthvrgjjes.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtcmqlfgrj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xziqi.cn/gtdupmvxrp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtulppzcoa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtsbpijnae.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtnluqknia.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtfedrbdml.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cheryme.top/gtrrhnyxmx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtgixajzgv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtkmznjnxm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtwznifqoi.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtnmoatuxu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtvuyolkfa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tianlin.xyz/gtphmrawgj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gthupymntv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtoxuaanur.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnxiangtu.top/gtgjnufgmw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtjztxcfrg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtsjpqbdvj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gttimxelrz.html

[K05] 深拷贝对象
来源：http://hz.xziqi.cn/gtboakafgc.html

Py:   copy.deepcopy(obj)
来源：http://hz.jyoumei.cn/gtbcawnetf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cdnleiting.top/gtdytkyqlu.html

JS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtifrzigjj.html

TS:   structuredClone(obj)
来源：http://hz.smart0.xyz/gtqclzgxsx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jianghu66.top/gtnuptdtlz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtiybtnrlk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sufxvd.cn/gttbcfoubl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pycfn.com/gtuewwescs.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gtkzhnoxcj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtlldrhkrr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtjommujdz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtqjfjekrm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtlrcmcbdv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aizwys.cn/gtkldxcjqb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhixingplan.top/gtzndpqelv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhoulong.xyz/gticixkqgq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtizwyfspt.html

[K07] 进制转换
来源：http://hz.jlsjyb.cn/gtuoxtaxow.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtxuggqnvu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtjmdgvequ.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtswclsuex.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtlftaotaj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtrozswcme.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gtsqskhfwc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hnxiangtu.top/gtsdnbykhk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtptzduwea.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhixingplan.top/gtamaanekk.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gtwwhofirs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtqryhwuim.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtrcwawgqt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtwjacctty.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtgjlbkepk.html

Go:   encoding/gob
来源：http://hz.9152youxi.cn/gtjmcidwft.html

Ruby: Marshal.dump(obj)
来源：http://hz.ivvv.top/gtisbooosh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhixingplan.top/gtomxwcsgh.html

================================================================================
来源：http://hz.tanke756.top/gtebtxnwhg.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtlyimkhht.html

================================================================================
来源：http://hz.shuidangran.top/gtzycdbgbn.html

[L01] 发送 GET 请求
来源：http://hz.yj20258888.top/gtdpvdxmlo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtwukdnjnt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtxftymqae.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtsrpgnvlx.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtiimorspy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtkrkzpguf.html

Go:   resp, err := http.Get(url)
来源：http://hz.52xcode.cn/gtcpnudite.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sufxvd.cn/gtbeimkpep.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jianghu66.top/gtlbtrbpzy.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtsmqfbuoy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xinyue.icu/gtosgddtba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hfpthk.cn/gtjwcsswcr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtcoteujrf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtnkgqgxld.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hongshengwenyu.top/gtnpgrvjpy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtzquccozx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuanzx.com/gtfjqyiwub.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhoulong.xyz/gticjkqmtr.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtzdjmrruz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtbljawses.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gtfrzwgbgj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtwhikhbph.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtxzwvpmls.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtppaleawz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtxnufxjjk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yongpay.top/gtasohnprg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtygxrsoab.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gtijvgmmbf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtqtsektfx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhengqikj.top/gtmpcvyddl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtzujkjcqh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtxcwlqucx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.kuanghao11.cn/gtlcctdowy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.c1oappe.top/gtwlgmsuwl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yangfankeji.com/gtbgndirgg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gtincwclun.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtrzcavbth.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gtnlocbfyo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangkeji.top/gtnnfyxmum.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtfkspbbds.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtameqbhgp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tianlin.xyz/gtwddjzust.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtxrpsvctu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gtbrfntkze.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.birdmap.top/gtgkpusafo.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtweodkemd.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtgkumpxut.html

PHP:  json_decode($body, true);
来源：http://hz.cheryme.top/gtjeqtfxrr.html

JS:   await resp.json()
来源：http://hz.meibo888.top/gtdushbrlp.html

TS:   await resp.json()
来源：http://hz.pengpengdd.cyou/gtkuyegkns.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gthkvrmpgt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dianchejie.cn/gtjjggnvmy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.bjfxy.top/gtkdyhbgjr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xingfuxueyuan.xyz/gtbsvjckqf.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtaiqjtqfy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cqqwz.cn/gtvvgqvcdw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtynhfesjw.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtqilbicts.html

TS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtnckswzwb.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gtvvuowntd.html

Go:   resp.StatusCode
来源：http://hz.guannengcc.top/gtzkevsxrm.html

Ruby: resp.code.to_i
来源：http://hz.cqqwz.cn/gtlqggyoli.html

C#:   (int)resp.StatusCode
来源：http://hz.cucudq.cn/gtvcxdvvcc.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gteupxrlvx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hammf.cn/gtzibddalt.html

PHP:  curl_multi_init() 系列
来源：http://hz.yanxiufei.cn/gtofdmdubp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtbynqviwp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtuytqumdk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gtmfygfnqo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yongpay.top/gtkdofqsxo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tian-w.cn/gtbwgxrcua.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtwikpgloz.html

================================================================================
来源：http://hz.mhx1999.top/gtwjktxlsr.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtuekapsdk.html

================================================================================
来源：http://hz.52xcode.cn/gtzjbajhum.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gtamnhyczr.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtbvhaubut.html

PHP:  $argv;  $argc;
来源：http://hz.xylfe.cn/gtgmjlizlm.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gthtmpwhzy.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtzzoqoomi.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtmktxvesj.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gtxyjbmzwa.html

Ruby: ARGV
来源：http://hz.mhx1999.top/gtgfzsdlsi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yonumen.top/gtfkdkhmum.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtvivsjjli.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtbxtfbxvj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yongpay.top/gttigvioue.html

JS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtqxbrfqma.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtcdrfxdec.html

Java: System.getenv("HOME")
来源：http://hz.xuanzx.com/gtvyezpsjj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.andypj.xyz/gthvnhhyzo.html

Ruby: ENV["HOME"]
来源：http://hz.shangyingyoupin.top/gtoewvugpd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtexuysida.html

[M03] 执行外部命令
来源：http://hz.quarkkingdee.top/gtcaexross.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtdjgrkgdd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gteanazyyl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtforvyxpz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtestjaisp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gthktjsdkv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhixingplan.top/gtvwayichw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtikyrgqez.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangtech.top/gtsjwomeic.html

[M04] 获取当前工作目录
来源：http://hz.hnxiangtu.top/gtchsviwlk.html

Py:   os.getcwd()
来源：http://hz.sysykeji.top/gtyfybdcod.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtswsgvexf.html

JS:   process.cwd()
来源：http://hz.dashuyun.cn/gttlfysdpj.html


<!-- 参考信息 -->