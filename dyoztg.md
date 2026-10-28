代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinyuanbaomall.cn/gtmeoiyosq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenzaomai.com/gtkuplvyau.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtctvpwcco.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gthiayiizl.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fzhhl.top/gtijptfglv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tanke756.top/gtkwbhxpsw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtpohmwipo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydjk.org.cn/gtwjfxxyzy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jyoumei.cn/gtydyvjijj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtkxhykuwt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtucflksag.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtkbqjirft.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtxjupdvcg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtouewpego.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gtuwwtdhgi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtfugeygey.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtzckblpzn.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhijiandao.cn/gtteodulvi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gtwhezwhdk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gtedyfqdyw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtlwsoevub.html

TS:   /error/gim
来源：http://hz.sufxvd.cn/gtrysscynx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hywenlv.cn/gtrbqcozpj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ehwqpu.com/gtryutyxqw.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gthurgzgca.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gtmhzaqfbo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtpregnqig.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.quarkkingdee.top/gtgrwclcod.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.andypj.xyz/gtrorglret.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtoqrwoled.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtizybuxrw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtbxkbnjur.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gtdehpifwb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtnukxynfc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtewvanhim.html

================================================================================
来源：http://hz.zhixingplan.top/gtulyfiimf.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtwuhnpyii.html

================================================================================
来源：http://hz.fengsongda.top/gtmwtfpnop.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtntzhkapq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gaohongyu789.top/gtdeznqgtc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtvqaaifjz.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtkpvslqxx.html

TS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtxwjfaidn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtdpcpvswo.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtbrnrcbzc.html

Ruby: Time.now
来源：http://hz.jianghu66.top/gtxjqojfoc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ywan-chungtsiang.top/gtcsuatwzu.html

[J02] 格式化输出
来源：http://hz.andypj.xyz/gtbqkucfux.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtinigykcj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtlcnfdiqk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtiqeaxors.html

TS:   d.toISOString()
来源：http://hz.daxiang520.top/gtftvbdgno.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gttshygkjg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fzhhl.top/gtxhsbxuhh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtcdtlsprh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtnehzxyes.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangkeji.top/gtabcyuhse.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yangfankeji.com/gthrkdeheu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.0kj1m.cn/gtzxitycrt.html

JS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtqdsaavuc.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtkiczgxcw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gthpxowgjb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yvedp.cn/gtkchbivki.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtbalwadem.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtgjekcbum.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigfzy.top/gttelkldsq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtfpbazrpw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258.top/gtnewhggsv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtpejflojt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sxryk.cn/gtiafibwyn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guowangkeji.top/gtbgbkaaxa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gteltzeqbt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtiyyqctcd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fzhhl.top/gtvsmegava.html

[J05] 时间加减（加 7 天）
来源：http://hz.xingfuxueyuan.xyz/gtgipampft.html

Py:   now + timedelta(days=7)
来源：http://hz.pycfn.com/gtkvgobmqt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxuanxn.top/gtsjmwjknk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gtosnjstyg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtjlbuhzmp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cucudq.cn/gtoraqmtnz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtudtgbeog.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtdvygkbcq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtpaimgplb.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtjzaucuht.html

Py:   (end - start).total_seconds()
来源：http://hz.zycfv.cn/gtonabshoq.html

PHP:  $end->diff($start)->days;
来源：http://hz.aizwys.cn/gtamdlaicu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gtslbuzupx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtzsirjqse.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtxqgumuvf.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtrybzqkez.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gtgiwaugag.html

C#:   (end - start).TotalSeconds
来源：http://hz.bjfxy.top/gtxazgigej.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtqqivnyec.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtslifkqqp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtwqroakab.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtgnehmvng.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtjvjzoqic.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtwgsmeobx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.c1oappe.top/gtefkohboh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtxisgprlb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtfvlfvfpa.html

[J08] 提取年月日与星期
来源：http://hz.feifeiyinyue.top/gtuljcsgpf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hammf.cn/gtavsylfls.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ybcxt.top/gtqkqhlrac.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtclpzleru.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gtwjkwqznr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtseblszvr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.smart0.xyz/gtetmzydfj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ppjwa.cn/gthwsogmru.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gthycbadkk.html

[J09] 时区处理
来源：http://hz.cucudq.cn/gtgxafpfkl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigufen.top/gtedyxwfva.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.iojbl.cn/gtlxkotauy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtlbfqghud.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtpflktgzy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daxiang520.top/gtmohivzqb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtcencchwe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtgmqmjqmx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daxiang520.top/gtokasyaqi.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtdepghvlv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gtnwiejhpo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.quarkkingdee.top/gtelweobgb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtdkzumaos.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gtrfxxnbkd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxinkj.top/gtdevlpdcx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtlfdziatd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtuhrmyjmp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aibaodan.cn/gtdyeyqbfp.html

================================================================================
来源：http://hz.ydzc1.top/gtalwmgbzn.html

K. JSON 与序列化
来源：http://hz.yj20258888.top/gtuuisraem.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwyfzbutu.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtyqnxtykj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtssoxfrtb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtglkeqysb.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtgcqkdltw.html

TS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtnofhcegr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gttxqaqmtr.html

Go:   json.Marshal(obj)
来源：http://hz.xuetiantiany.cn/gtsnndgjhq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cheryme.top/gttztgexdu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtixncdjys.html

[K02] JSON 字符串转对象
来源：http://hz.xinyue.icu/gtbbgodyla.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtslehlweb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cashguo.top/gtxhdgngla.html

JS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtvewccsaf.html

TS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtznwtasqp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydzc1.top/gtlhwyqotf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gteeubquzr.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtdbprgkmh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtczebbucj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nwbrower.top/gtwlchpwpk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtenjxqyex.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtlovsymwk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtidjgrxdj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtqmvzktkw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gtrmysvdph.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangdashe.top/gthpjlkxnk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daxiang520.top/gthhcyyrzo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtivekvwoj.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gtgpppwhff.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnqzz.top/gtattcbdkq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtcrrltdsl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtmwparxsj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtqxpwtrha.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtqszepjua.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtjnkaqius.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtqvmraiec.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtomjrweek.html

[K05] 深拷贝对象
来源：http://hz.xuanzx.com/gtnejiccke.html

Py:   copy.deepcopy(obj)
来源：http://hz.jlsjyb.cn/gtsgsjgyrh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtgumxgyda.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtnnrvjsnm.html

TS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gttlryxjbp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtlhtdxird.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtvfpzopxt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtbkgkhfst.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtiiksyxhn.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtfaoxzpbp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhiwuduotai.top/gtmrktcugk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.0kj1m.cn/gtbxoylnru.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtadzshalp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtzjyihbra.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ehwqpu.com/gtvoahfvmt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gtaumllabe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pycfn.com/gtrycdvnnz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtwyfzgfdq.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gttymsgkxt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtrofobqtb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigfzy.top/gtshdcpnfd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtycbuhjwp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtmgunbdrp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtfcqwfvhg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtykflpumf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtslquvqah.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guowangkeji.top/gteyddsrio.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtpadrpfbz.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtucujqqsh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtsfhiawkk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gttzzniwfc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtuhmjpsau.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtsvkupyme.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gtcgxriwrn.html

Ruby: Marshal.dump(obj)
来源：http://hz.bjfxy.top/gtghrzzple.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtnvosvyxa.html

================================================================================
来源：http://hz.cdnleiting.top/gtyvajbobt.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtkdqcacmc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtebauyiwh.html

[L01] 发送 GET 请求
来源：http://hz.daria6918.cn/gtmyngwbpl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.haohaochexian.top/gtdiglquhd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtbhjlaobs.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtcjflopxt.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtltzqqoea.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtzgvjtcte.html

Go:   resp, err := http.Get(url)
来源：http://hz.wangdashe.top/gtxhvovzrb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhongyouzk.top/gtlffuxlqm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxuanxn.top/gtwvpqenvw.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtijcwzlxd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.pengpengdd.cyou/gtpwgfwoyh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guannengcc.top/gtdfhmqywy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtgtpceauh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtxoglvoae.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhengqikj.top/gtknvkgfza.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jyoumei.cn/gthvjfwqhs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtxsoetoja.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtazwiumtj.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtxvfxtgak.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hfpthk.cn/gtydokxlig.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtsrzoripz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtzdozfadq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtylmnqwxb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtvjwqucpn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gtqwhbgudg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtydaztjfy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.smart0.xyz/gtdwwojrbs.html

[L04] 设置超时
来源：http://hz.jinyuanbaomall.cn/gtsjentfdf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hongshengwenyu.top/gthsondjjg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtoblidqia.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtfpkchqfn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtpftrmxdp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtxdfhieet.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aibaodan.cn/gtxmdegxez.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258888.top/gtrcwlomda.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtnkvyzsha.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtiucuafxp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fengsongda.top/gtcewvomwo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtdoetbbfc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtqjvgnemz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtqcjkrpie.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtcgdxekzu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtioxoperr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258888.top/gtirmlqjmz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yueranfly.top/gtbryyixtj.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gttjdaxbqb.html

Py:   resp.json()
来源：http://hz.nwbrower.top/gtjvmylzyi.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtohlyivra.html

JS:   await resp.json()
来源：http://hz.tian-w.cn/gtlbdjeywx.html

TS:   await resp.json()
来源：http://hz.zhoulong.xyz/gtmsslixzo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.0kj1m.cn/gtervtbsjd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtdmnzfqaa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtvdhupoel.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinghuilouyu.cn/gtivyknsih.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gtodeazwbu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.316326.xyz/gtxsuxvwfk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhiwuduotai.top/gtdtonuutu.html

JS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtxtpiaxhq.html

TS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtqxdbskwk.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtmmcgcrji.html

Go:   resp.StatusCode
来源：http://hz.kuanghao11.cn/gtvxayulgn.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtuabjkjqm.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtysfttacz.html

[L08] 并发请求多个地址
来源：http://hz.xuetiantiany.cn/gtrjhyvawg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shzxlz.cn/gtbgyevure.html

PHP:  curl_multi_init() 系列
来源：http://hz.ppjwa.cn/gtaoulpthy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtdfluitmm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtttjyfwms.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtxsbnkyxi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtgchdicjm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtwapcwgnz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hysaishi.cn/gtgsimdhfz.html

================================================================================
来源：http://hz.gotoacloud.top/gtoqroixrl.html

M. 命令行 / 进程 / 环境
来源：http://hz.fengsongda.top/gtnihuswct.html

================================================================================
来源：http://hz.ehwqpu.com/gtejupyxob.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangtech.top/gtndosujhu.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtytkllupu.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtzbybekgd.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtwearjpeg.html

TS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtrdronclo.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtswfnmokz.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gtgqnxsept.html

Ruby: ARGV
来源：http://hz.havefunace.top/gttrizdpqz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnqzz.top/gtgbqtoapg.html

[M02] 读取环境变量
来源：http://hz.zycfv.cn/gtkyhfscug.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtvnholkma.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtpmvopezq.html

JS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtxfjxqrtx.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtxxgwodyi.html

Java: System.getenv("HOME")
来源：http://hz.hysaishi.cn/gtbfymwpqt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ywan-chungtsiang.top/gtvduzrbmv.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtmlnguyaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnxiangtu.top/gtyqcumhid.html

[M03] 执行外部命令
来源：http://hz.guannengcc.top/gtpvgjdzwe.html


<!-- 参考信息 -->