代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xziqi.cn/gtedtfarbq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gtnqdyotak.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtwjpevnfr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtdxbijakw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhijiandao.cn/gtrwpewtov.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zycfv.cn/gtcjgnpgis.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtgfqbivxz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtiwteojmg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daxiang520.top/gtxwpfyibp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gtfalvzgvb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cucudq.cn/gtpdcaqdki.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtmwtjguhu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtfcrmxwgi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zdqjudy.top/gtlvcynscc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhongyouzk.top/gtktcpigof.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj202588.top/gtpewibdqp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gtexahzwcq.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtkjqparvb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtbpnfjexz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtmgaennqy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gtcqvbbugv.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtgcfdcunx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtdtscexre.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtuvbniyfi.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtufgkxuvj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hammf.cn/gtsshlqmsh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtfddmtsmu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtgjkavfsr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenzaomai.com/gtztehmvqq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenjidiqi.icu/gtqzktyqgh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhongyouzk.top/gtjvzwwlfh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtzzrgwnnq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ybcxt.top/gtauvzebml.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtyaumivkv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtbmhxnyun.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gteuflatra.html

J. 日期与时间
来源：http://hz.yvedp.cn/gtcdtinzyx.html

================================================================================
来源：http://hz.bjfxy.top/gtxalttjev.html

[J01] 获取当前时间
来源：http://hz.hammf.cn/gtbrpcjnkq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtcbijczsc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtvrzlygav.html

JS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtoyekfxrf.html

TS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtnoqmatxr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtlbttzofu.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtcswclbvi.html

Ruby: Time.now
来源：http://hz.gaohongyu789.top/gtloemjzsh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenlongwang.top/gtiorsvvxk.html

[J02] 格式化输出
来源：http://hz.ivvv.top/gtjvglmqwf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtrnuhyizz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtrcrcioav.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtclekxjpn.html

TS:   d.toISOString()
来源：http://hz.xylfe.cn/gtkvxnivro.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtieiollch.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daria6918.cn/gthgbxdwib.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtzlvzgzid.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.0kj1m.cn/gtlswwfucc.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtmxyyaauo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydzc1.top/gtcxewhiuy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sysykeji.top/gtchgbwyrc.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtazvzrflh.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtqrofxgty.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtwkuexsdd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtczozrgar.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtmjdwovjo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fengsongda.top/gtwvvxbylq.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtdgmqglcv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xinyue.icu/gtomdrjous.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtyriuxhpm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtpsvumpth.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenjidiqi.icu/gtbqfqbgcl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gttzihjvee.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenjidiqi.icu/gtxdsgtode.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtfqvdmwrc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fzhhl.top/gtukhtatse.html

[J05] 时间加减（加 7 天）
来源：http://hz.tanke756.top/gtvujcdhbm.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtghbwlydr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shzxlz.cn/gtklyrjqio.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtwnwrkgsx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtzqnmphrc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gttpebzzqr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.smart0.xyz/gtjcemobeh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yanxiufei.cn/gtepvmtcyf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tianlin.xyz/gtzkemehal.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gtfgnrqlkr.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtvpymcbzw.html

PHP:  $end->diff($start)->days;
来源：http://hz.zycfv.cn/gtmkjhyacg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yonumen.top/gtoxnruehj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.feifeiyinyue.top/gtdcbvrrar.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydzc1.top/gtrpqbaenm.html

Go:   end.Sub(start).Hours()
来源：http://hz.hysaishi.cn/gthexjzwwe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtqufljcrf.html

C#:   (end - start).TotalSeconds
来源：http://hz.tianlin.xyz/gtvnobhney.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtxtfwelpl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtrgkkwrqb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtbbmafkfb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtwgyrrsmy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nwbrower.top/gtxfnxqfnh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shzxlz.cn/gtlmyuhdyr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtmlvucpyf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gticrdnyqt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtlnsbytmw.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gticytqlnq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jqgufenzy.top/gtgoxtlsrg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cashguo.top/gtdytaeaup.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gtrpvylkxt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gtecuufvsy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258.top/gtexjvgmex.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xziqi.cn/gtdlevxxhm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.9152youxi.cn/gthwqeapgu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtydmwvtxx.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtilxpmyig.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtssqejftn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gterghnyos.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xinyue.icu/gtodztujtx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gthumcdumw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.daxiang520.top/gtuxgoycxt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtzpoftbzy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gtsmxtdckg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gthyghdqof.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtzbfneyov.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtpiqvwdwn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.haohaochexian.top/gtzyfrahxx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gtgpfzkexz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhongyouzk.top/gtjygmzpdq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.haohaochexian.top/gtjkxvwyou.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fzhhl.top/gtktyenbko.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gthlnqjrpe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gthjhrpmjb.html

================================================================================
来源：http://hz.tian-w.cn/gtohjuwbgo.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtfyatxuza.html

================================================================================
来源：http://hz.ehwqpu.com/gtzdyjtxaz.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtdnunjekf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fengsongda.top/gthpzlmlqa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtytjtzmbe.html

JS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtymlhhfyw.html

TS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtmsxekrni.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtzktcxztf.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gtddgsqgmc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhaomingkeji.xyz/gtajvbkwsd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtxqjrszzp.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtxeoucomg.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtfyxfcbvr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hysaishi.cn/gtqhdgherz.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtpygwvxvc.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtuupuzwgb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtmimzppxv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtsgjbjbqn.html

Ruby: JSON.parse(s)
来源：http://hz.ivvv.top/gtlmwemhvt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtglnkruav.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtsxntfysy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtalmhroor.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtnmuvazjt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtqpfqarae.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtcvongnlz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hywenlv.cn/gtzqiqahrf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.smart0.xyz/gtfizpbsol.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtvcfwxjwy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.vqdsnc.cn/gtydjaqsbr.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gtzkhyablj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gtebbjwger.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jyoumei.cn/gtordmvrzw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtcvbruebn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtzhgpxumk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cqqwz.cn/gtktuxqanr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtltmugjcn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtizgrjwjt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigfzy.top/gttegblamk.html

[K05] 深拷贝对象
来源：http://hz.chenlongwang.top/gtrslotgqj.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtnupvtusa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xingfuxueyuan.xyz/gttacftxpw.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtvrnoedmz.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtldynikav.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuxming.cn/gtnrndhkvq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydzc1.top/gttzsheeep.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtwyilwbwu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtrevdoash.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigfzy.top/gtbapoknsw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gtzeyuqalw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtjkeetfyk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtvrtoxmvq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtpnlywrgb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtmrbazcwp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtpiuyljsc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtsxhkubiq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtkwkogzli.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtddpgiejc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gogol.net.cn/gtqwcmrfya.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daxiang520.top/gtlbpnjkdu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtcsxqxvne.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtunvcecdl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtkbcdkiyn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ppjwa.cn/gtmzghjomz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuanzx.com/gtblqxpxqp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtwmjdqcix.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxinkj.top/gtrkpuaree.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtaitusztz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhengqikj.top/gtlodyftss.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gthupziicm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtgltlpppf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.iojbl.cn/gtbiaaugbt.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtzutvlage.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhiwuduotai.top/gtpgvndzvn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtwpowqlqv.html

================================================================================
来源：http://hz.cqqwz.cn/gtamerapwh.html

L. 网络请求
来源：http://hz.cashguo.top/gtefkkbnhl.html

================================================================================
来源：http://hz.hywenlv.cn/gtfvnfrdqc.html

[L01] 发送 GET 请求
来源：http://hz.snrcjt.cn/gtyrhtfxvo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.haohaochexian.top/gtflduswad.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yueranfly.top/gtasqyhtlx.html

JS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtrjvxlfrm.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtphwwsnxb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtklsmljhu.html

Go:   resp, err := http.Get(url)
来源：http://hz.yangfankeji.com/gtopsezgdu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.haohaochexian.top/gtjypyxomx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hfpthk.cn/gtznpeqbbg.html

[L02] 发送 POST JSON
来源：http://hz.zdqjudy.top/gtgvfbdzam.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yangfankeji.com/gtztuurntk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgufenzy.top/gtmpxxkgoj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtsvvtotmp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtahifiics.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydjk.org.cn/gttlzlauta.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtqlertjev.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangkeji.top/gtmjkojenc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jiagoushi.top/gtwcjaisph.html

[L03] 设置自定义请求头
来源：http://hz.yj202588.top/gtakweofue.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtkcbuhhpy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yvedp.cn/gtnteizcco.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gthqzilcgg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtaxlnjnwm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.52xcode.cn/gtnttnlkmc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtewbivqci.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxinkj.top/gtojmhwffe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtoaegnsiz.html

[L04] 设置超时
来源：http://hz.hywenlv.cn/gtxaxdndfz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gttqohhhwq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtuwqwqyev.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtpitkygfz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtcvvpmwar.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuxming.cn/gttxlugtjy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtdxsugajs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jyoumei.cn/gtdzvvibxk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ybcxt.top/gthuvkuygu.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gthohgkcyc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.redwolf501.top/gtbtdcmowv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtlcqgsykt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtsmchakwq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtmcvlqxwx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtymmkxiwt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gzhubu.top/gtlsgpjujp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtybtgohdn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.havefunace.top/gtqwkolztj.html

[L06] 解析响应为 JSON
来源：http://hz.yonumen.top/gtxdaocyqr.html

Py:   resp.json()
来源：http://hz.pycfn.com/gtvawpxujw.html

PHP:  json_decode($body, true);
来源：http://hz.yonumen.top/gtvzmphidc.html

JS:   await resp.json()
来源：http://hz.0kj1m.cn/gtmdmifnoz.html

TS:   await resp.json()
来源：http://hz.aibaodan.cn/gttvbvwbcm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ybcxt.top/gtuzxmfmrn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtaerukcpc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtruljqvnm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtifvqpsua.html

[L07] 处理 HTTP 状态码
来源：http://hz.gotoacloud.top/gtwvvyriis.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hongshengwenyu.top/gtsirbzruu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtzplyxppc.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtbsioxkdx.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtbcginfye.html

Java: resp.statusCode()
来源：http://hz.hysaishi.cn/gtbxpntyzg.html

Go:   resp.StatusCode
来源：http://hz.snrcjt.cn/gtzjylfsbp.html

Ruby: resp.code.to_i
来源：http://hz.0kj1m.cn/gtpwlxjifq.html

C#:   (int)resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtmdxcihns.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtepspbuoz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtxdnpeqmm.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtsvposkqf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtdljnriwf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtubmwfvac.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yueranfly.top/gtshknpbyu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gtsomrdage.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hysaishi.cn/gtzbietkfo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtpwwgruhr.html

================================================================================
来源：http://hz.xylfe.cn/gtxhxmxtye.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangkeji.top/gtuxenvmlm.html

================================================================================
来源：http://hz.havefunace.top/gtbnxywftp.html

[M01] 读取命令行参数
来源：http://hz.ppjwa.cn/gtrgtsapol.html

Py:   sys.argv[1:]
来源：http://hz.shangyingyoupin.top/gthrljlymz.html

PHP:  $argv;  $argc;
来源：http://hz.9152youxi.cn/gtwjnvanhj.html

JS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtmrkdfkth.html

TS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtmtjkmesq.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtjqauibww.html

Go:   os.Args[1:]
来源：http://hz.wangdashe.top/gtzzxqrhdz.html

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gtvskoknxb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gtrmbuogqn.html

[M02] 读取环境变量
来源：http://hz.tanke756.top/gtlzwzvdkc.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtctshthtq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jyoumei.cn/gtqpodfywa.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtvxzchsrr.html

TS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gtftlwduzl.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtukmlbmun.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhixingplan.top/gtjdhaulmn.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtzuaubqlm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gogol.net.cn/gtikvuedce.html

[M03] 执行外部命令
来源：http://hz.dianchejie.cn/gtaaxqidbg.html


<!-- 参考信息 -->