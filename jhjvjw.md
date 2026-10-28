代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.wangdashe.top/gthhmftwoc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtufaphkbq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtgacfobqy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtkygzugnh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenjidiqi.icu/gtslbrzxsg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtsfjbehuf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtbmwjsgek.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtscxocxvc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtyudbknag.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gteezsahdk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhengqikj.top/gtnqcbltwx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtrdkestgx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtpxrrdzeg.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtaekcxwyk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hammf.cn/gtgsjaekvy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shzxlz.cn/gteozvzpuy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xingfuxueyuan.xyz/gtcjnckhrz.html

TS:   /error/gim
来源：http://hz.ehwqpu.com/gtndvwkkua.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtcpmwdoft.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.quarkkingdee.top/gtkxxgylec.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gtymmvphgr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtswaijjjl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtoavcxfxd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shuidangran.top/gtgxeffkzi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtjkrbazch.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtzzzmxflg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gtemfeyahj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtfvypepre.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtmtnhyhdw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtymvswwty.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtjtrvipkr.html

================================================================================
来源：http://hz.birdmap.top/gtslpclicy.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtkpgwdzfi.html

================================================================================
来源：http://hz.tian-w.cn/gtnwcqellk.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtyldugjzu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtcwutzpyx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtbwzkefzb.html

JS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtwqywpodi.html

TS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtqcoolwhl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtmnxlxnrp.html

Go:   time.Now()
来源：http://hz.andypj.xyz/gtsuuzafui.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtpeujazlz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tian-w.cn/gttydzhtaj.html

[J02] 格式化输出
来源：http://hz.yueranfly.top/gtvwvdpajx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtvsoajvpe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtfeuiuebn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtvrottirn.html

TS:   d.toISOString()
来源：http://hz.tanke756.top/gtrxlyxqxe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shangyingyoupin.top/gtrekepjda.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtjwlfdtok.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtqbtjpbho.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtdmcokuyu.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtntqimsmb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xziqi.cn/gtgxttdjbk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shangyingyoupin.top/gtbtzltrpc.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtfndhqkxz.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gthulkrmvv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtlrkdcatv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258.top/gtozakcmic.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtbruoxyig.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yongpay.top/gtuajakgdm.html

[J04] 时间戳与日期互转
来源：http://hz.zhengqikj.top/gtahzxuext.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gzhubu.top/gtboamrcic.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtmizgnkwp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtickgmfsf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtgcdpmhzq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangkeji.top/gtbxhxwrhu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtlbtyhgls.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258.top/gtznkrkdue.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gtonpjcwtu.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtpjfmekre.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gteyfleytz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtvllyyzfq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtufzdzjxf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gteayntthg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gogol.net.cn/gtiznvnmmp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhijiandao.cn/gtsunecvxt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pycfn.com/gtzpqshdeu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.kuanghao11.cn/gtrcyinzgg.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangtech.top/gtosxyxwpc.html

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gtltyycqvd.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtcotwnmwj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtscmhngbw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtrcavdhmp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ybcxt.top/gtxovuzhpn.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinyuanbaomall.cn/gtzkjbfcqs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangtech.top/gtqtkrxpug.html

C#:   (end - start).TotalSeconds
来源：http://hz.nwbrower.top/gtnpsllegc.html

[J07] 比较两个日期
来源：http://hz.aibaodan.cn/gtcaxcelbx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtdekjbnda.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gttsrqfbpm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtqzxksnzg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtfxmkihek.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gtswomkngo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shangyingyoupin.top/gtkyxuuoed.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtgzwabkgu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtombexcdf.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtnjskxekq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtfzwgonzp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tian-w.cn/gtlcjrnzvb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cdnleiting.top/gtgbmyhqbt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtztmlqjdx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtnywkschg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangkeji.top/gtswrkrzdb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.bjfxy.top/gtivlgjfnx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gtjrilxggo.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gthlxtwted.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinyuanbaomall.cn/gtluymeiad.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtvhanwohe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtowldjegc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtiugoiovb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ivvv.top/gtfejwsrjy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tian-w.cn/gtptcbqtrt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hfpthk.cn/gtwryyxngd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtxhwqgule.html

[J10] 取今天 / 本月第一天
来源：http://hz.yonumen.top/gtzhsxjqfq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtmijxxgfd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ywan-chungtsiang.top/gtsucanreb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtdiukybrz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gtwitafdbn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtvxghimdw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gttphcucxs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtghvdtowo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.smart0.xyz/gttevkmtfu.html

================================================================================
来源：http://hz.dianchejie.cn/gtbllkqijy.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtkezvjani.html

================================================================================
来源：http://hz.xinyue.icu/gtkepsvprp.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gtbenltfrd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtlgksburq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtpkjzwdql.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtpuzrozoo.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtvznpsqtk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtfhmbdkxh.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gthlqkkfcr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dianchejie.cn/gtqrekzayv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuxming.cn/gtdzqntvlh.html

[K02] JSON 字符串转对象
来源：http://hz.chenzaomai.com/gtewvrtzyo.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gtsfxwplub.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gtshttylur.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtunzwvugp.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtfofqbwoe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pengpengdd.cyou/gtabucnygf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtzhhhfahu.html

Ruby: JSON.parse(s)
来源：http://hz.xylfe.cn/gtopvmthwk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ybcxt.top/gtbiesbprl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.0kj1m.cn/gtxpqoqlhe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtsidfdnmz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtkujnkckr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtbdenofms.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtwztcpeiw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gtwbpvvzmr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhaomingkeji.xyz/gtnltsmjen.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtfrwxbtfj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtkenmzgxt.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gtrnlierds.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtdvjqjsix.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gttooaraiy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtstljycnt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtbnzkmaco.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtzuwwuepg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtfzmslrhw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.smart0.xyz/gtaqsubukt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtkbqjvxah.html

[K05] 深拷贝对象
来源：http://hz.yonumen.top/gtporvxcvt.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtubulziwq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtchleadlt.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtiylkuvxv.html

TS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtdascimzs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.snrcjt.cn/gtuuerglds.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cucudq.cn/gtsrufiqpk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gtlclixnyp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtocewhbso.html

[K06] 解析 URL 查询串
来源：http://hz.cucudq.cn/gtoejqjavf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yonumen.top/gttevihnel.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtzvdfqqpa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtvwviunkd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtcnoachml.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sweek.top/gtzwjhgrmg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtiqtoagov.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gtsyzwfqfk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtdzoqnxcd.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtbketcbmn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigufen.top/gthqodnjwb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgufenzy.top/gtsaqbylbx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtszhicgoc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtdtbalqpc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtcecakuyi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ivvv.top/gtomognemv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.iojbl.cn/gtkrqljada.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydzc1.top/gtnbjtqfxp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gotoacloud.top/gtepxevgkk.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gtchbwtfgs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gtvhbzwqsb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtxzmgegwk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtjjjdkmfy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gttjdafbck.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtcgsrixqo.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtdagboisl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtzotxtdwz.html

================================================================================
来源：http://hz.guannengcc.top/gtofktdmuk.html

L. 网络请求
来源：http://hz.hywenlv.cn/gtcbfvewzt.html

================================================================================
来源：http://hz.0kj1m.cn/gtggltbwrx.html

[L01] 发送 GET 请求
来源：http://hz.9152youxi.cn/gtgsejkndw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtzsnrveib.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtigvwknpp.html

JS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtgnkdjjxz.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtmgyimjpu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtuzeyyijt.html

Go:   resp, err := http.Get(url)
来源：http://hz.smart0.xyz/gtktipdwon.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigufen.top/gtwgaajeey.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shzxlz.cn/gtsmhzelvg.html

[L02] 发送 POST JSON
来源：http://hz.bjfxy.top/gtigvqixxg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gtbtqvpuxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtytibftbl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtimxenflv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtiyccxsbx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gthswmaqbi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtpqipwxgl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtxoabprgj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangkeji.top/gtmxrpmpwy.html

[L03] 设置自定义请求头
来源：http://hz.xinyue.icu/gtxqzmrtpf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxuanxn.top/gtgyalwuoi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtuuugrsfg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtrrnuiyol.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtzuizlvwb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenlongwang.top/gtfeyqvgno.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtqhufphuc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtxuwcnhkw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtnepumcpw.html

[L04] 设置超时
来源：http://hz.xziqi.cn/gtlkzqmuzb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtzyinonse.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.andypj.xyz/gtmuwjjipo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtmbyptpbu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtuzumvhsw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.havefunace.top/gtrgkojhpp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hywenlv.cn/gtjydfzhgr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.pycfn.com/gtlkmeirqq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.daria6918.cn/gtaoqlsfoy.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtqrxmxnka.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtrmsqkmvl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtcaulymwx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtqxwtscuy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtwhgnpsvh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtgkxfyzdy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hnqzz.top/gtjoglcduu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jyoumei.cn/gtmgforqvd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jyoumei.cn/gttaejgtyj.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gtkudtnmig.html

Py:   resp.json()
来源：http://hz.hongshengwenyu.top/gtjaonlcry.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtfldpdscm.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtnpqlpzir.html

TS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtietbmrca.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gteqbmppgb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cdnleiting.top/gtepbnncnn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtqjundxns.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtlyoukmsh.html

[L07] 处理 HTTP 状态码
来源：http://hz.dashuyun.cn/gtlyqwgstw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.svipenyu.cn/gtfepidlxd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtnsztecql.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtmmzjnxpb.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtkpkyoomz.html

Java: resp.statusCode()
来源：http://hz.jyoumei.cn/gthjcfwufg.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtqotklynx.html

Ruby: resp.code.to_i
来源：http://hz.hammf.cn/gtjdafpflc.html

C#:   (int)resp.StatusCode
来源：http://hz.jiagoushi.top/gtnmwssadh.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtlnzybzhe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hongshengwenyu.top/gtdnjpszll.html

PHP:  curl_multi_init() 系列
来源：http://hz.ybcxt.top/gtmomairiv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gteroxggtf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtzgerhlmn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gzhubu.top/gtgdfzpkwk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yueranfly.top/gtdduahssn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtavhqazjp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangdashe.top/gtgjupriut.html

================================================================================
来源：http://hz.xuanzx.com/gtrxfhjrje.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtzuftbhzl.html

================================================================================
来源：http://hz.yj20258888.top/gtgysfhlbp.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtswkegela.html

Py:   sys.argv[1:]
来源：http://hz.c1oappe.top/gtzdehwqhf.html

PHP:  $argv;  $argc;
来源：http://hz.ivvv.top/gtlkbfyidf.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtavtcvacm.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtgvymmoqs.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtbrtbvpsq.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtctzhnhob.html

Ruby: ARGV
来源：http://hz.sweek.top/gthdimxlwr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jyoumei.cn/gtadxlgtnf.html

[M02] 读取环境变量
来源：http://hz.gogol.net.cn/gthlebhctu.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtnzrjyhea.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.316326.xyz/gtcyghuiph.html

JS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtqllbezck.html

TS:   process.env.HOME
来源：http://hz.yuxming.cn/gtqitouxpp.html

Java: System.getenv("HOME")
来源：http://hz.sufxvd.cn/gtbucgbrdm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gtttvggmfj.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtdtaozrye.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtvtjojepl.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gttffarzkf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258.top/gtyypbbyje.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jlsjyb.cn/gtstdnmrwc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtgvqlevld.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtybigkxbp.html


<!-- 参考信息 -->