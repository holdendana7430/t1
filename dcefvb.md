代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtyaqthgje.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtpjycxqzb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtptofsiyl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuetiantiany.cn/gtwaewxxqe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtakwgrpla.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydjk.org.cn/gtvracizoo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtphtiyyke.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtxybctire.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hysaishi.cn/gttjahymgy.html

TS:   /error/gim
来源：http://hz.shanyushiyangkeji.top/gtdcrwlkjd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cheryme.top/gtrlaeiwmt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.52xcode.cn/gtldlyrjuq.html

Ruby: s.scan(/error/i)
来源：http://hz.smart0.xyz/gtkszlbqfc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gogol.net.cn/gtioygcakd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangtech.top/gtgbzngtyn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shzxlz.cn/gtgfqbqcwl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aizwys.cn/gtinnfdbxj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtwdxbjtkh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj202588.top/gtdbvjdhyx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtdxlnkrhp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhoulong.xyz/gtndduzqrs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ywan-chungtsiang.top/gtywduubzo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtbupuorwc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvnyuvqix.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtyzgxhwjm.html

================================================================================
来源：http://hz.smart0.xyz/gtttrgwwbu.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gthewvvnvt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydzc1.top/gtaixhqzkd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtmkgdzixh.html

JS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtytpgieie.html

TS:   new Date();  Date.now()
来源：http://hz.hywenlv.cn/gtxgrvykbh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtgknpcitn.html

Go:   time.Now()
来源：http://hz.daxiang520.top/gthutlnabb.html

Ruby: Time.now
来源：http://hz.gotoacloud.top/gtdcrzgodb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtxhpzapen.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtuhflnvri.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtkzpfhdwl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtbudvbtmr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ywan-chungtsiang.top/gtpelcqmli.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gtmbkbngjs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtetzawmua.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtvnzshoql.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtexshlixh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.bjfxy.top/gttsymeddr.html

[J03] 字符串解析为日期
来源：http://hz.xuetiantiany.cn/gtymhsywsg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhijiandao.cn/gtvxmuufcu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtjkamjeua.html

JS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtypmyfixb.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtpcncghbd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtiaaamtij.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtxozpxleh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtwsuqmaht.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aibaodan.cn/gtkdmlvjgu.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtgmwkxrya.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cashguo.top/gtrpuvodnv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtkssmwqha.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gtxtbkbgpw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtlczzmvll.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinyuanbaomall.cn/gtzjokgkhm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jlsjyb.cn/gtjmprhoxh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtuxvxapsr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtblirwcqn.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtukagfmjd.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtyjjhpfub.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtwospumgd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtllrhnnzs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtrtgbjbfl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtkrwhused.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gttznrlrht.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shangyingyoupin.top/gtppscwgrc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtslncuumc.html

[J06] 计算两时间之差
来源：http://hz.dianchejie.cn/gtdcnuyzbp.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtbslivpxa.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtqvumdfla.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtrkfuucfr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.vqdsnc.cn/gtflyizgsc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtcxefvhpb.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtodlvqzlx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtwevttjha.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtlkfrkvry.html

[J07] 比较两个日期
来源：http://hz.chenjidiqi.icu/gtzroilcgb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtyrfexusn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gttzlrqdjd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtqcagjdin.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtvaxremct.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtqgbjoszi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhiwuduotai.top/gtcezvrsvj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtmlubklyv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtqxwzwplc.html

[J08] 提取年月日与星期
来源：http://hz.yongpay.top/gtbwehenci.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtymhubpje.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sysykeji.top/gtqpogusrs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj202588.top/gtudeicfmw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtgzegbprw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtifzctypf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shangyingyoupin.top/gttbxknotg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtaqtardjk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtyqpekxdf.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtojrefrcq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxuanxn.top/gtcmpezcri.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtreeqcnqs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtzxdearsw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtiuqewaaq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuanzx.com/gtqfhlcloy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenlongwang.top/gtrzdcawbn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtnklpsrdn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yvedp.cn/gtdlukndea.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtfophmbdm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.andypj.xyz/gteprqeneh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guowangkeji.top/gtnhjjsvjl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtiolyhtyw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtitaijfmb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtnuejutgs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.bjfxy.top/gtrfjcvfzx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shzxlz.cn/gtzsqcpyfi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenlongwang.top/gttqqsaoqq.html

================================================================================
来源：http://hz.dianchejie.cn/gtzkrplbjx.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gttprbdncq.html

================================================================================
来源：http://hz.redwolf501.top/gtzwqogyym.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gtekajvett.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gthjyisgzt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtivuhzqme.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtflwksqtx.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtlcfjfznf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtekgrwzbm.html

Go:   json.Marshal(obj)
来源：http://hz.nanxuanxn.top/gtajckemqp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenjidiqi.icu/gtzpjqgnjr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtjlanfwuv.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gtdzhkxphq.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtdsfcdbbm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ehwqpu.com/gtrnilxbeg.html

JS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtsnckjdds.html

TS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtexbmmyhj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtehybeowh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtcmcckkmm.html

Ruby: JSON.parse(s)
来源：http://hz.meibo888.top/gtrmfmljmd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtxcdspdus.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtfzlizesw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.birdmap.top/gtkkvtlvay.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gteruxqrvi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtrtcwefqq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtovixxeop.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydjk.org.cn/gtryjybytx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtjbheoarn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gtwatutaij.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtqdsfjaxt.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtvyngvibf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gtgziajxzy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtejexmnwn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtmrjbkyqm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtietlxxyn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtelwyoawc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtwdowgeei.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gteljcrwcf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gaohongyu789.top/gtfnskakkr.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gtlarmmpuz.html

Py:   copy.deepcopy(obj)
来源：http://hz.hywenlv.cn/gtqcmpxzcq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtnywyrjuw.html

JS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtqsmzneec.html

TS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtwfjxctau.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sweek.top/gtfwhooime.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtlghscefv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtzmtziplo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtjsmoqkxk.html

[K06] 解析 URL 查询串
来源：http://hz.xuetiantiany.cn/gthuykwngc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtztnwkirg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtxypgfgyr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtuupjkpaz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtvtjzcmia.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtpgepbcgi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtldxxmctf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtizxmvhpv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtlfgphhvd.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtjcwmxvtq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.pycfn.com/gttjsfdxnf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtvtrqafgb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtbsccixdu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtfmfzsfwf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gteqtpibbu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aizwys.cn/gtojsdzazu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtyafcibfj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtcpaytzfx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnxiangtu.top/gtifqiwsal.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gtgcxggxzr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yanxiufei.cn/gticmywbts.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gthrnqoudj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtntuuekzt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtvrgjnmlm.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtlciahibc.html

Ruby: Marshal.dump(obj)
来源：http://hz.hfpthk.cn/gtlhbbbuvy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gtbapxdtym.html

================================================================================
来源：http://hz.svipenyu.cn/gtangvopwe.html

L. 网络请求
来源：http://hz.yonumen.top/gtpxfxtvtb.html

================================================================================
来源：http://hz.jinqigufen.top/gtkshmczou.html

[L01] 发送 GET 请求
来源：http://hz.yanxiufei.cn/gtzbdkgbqx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtgzwoitjy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.feifeiyinyue.top/gtgnrfokpo.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gtsfzhsjwb.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtgoequhys.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gotoacloud.top/gtcxugvhoy.html

Go:   resp, err := http.Get(url)
来源：http://hz.quarkkingdee.top/gtllkbgnha.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ivvv.top/gtjqbmnyht.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtdqmhubsp.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtllycywrh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtyozaqzia.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtiyllkmbw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtlidjmnmy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtcaiuubkw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtukaghgya.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sufxvd.cn/gtnjeromya.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gteugbqgcc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhoulong.xyz/gtgbuqrdgw.html

[L03] 设置自定义请求头
来源：http://hz.cashguo.top/gtiztbtkav.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ywan-chungtsiang.top/gtcznpecjr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.bjfxy.top/gtmumvhgfj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtqsihqtrq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtreghvkpb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sufxvd.cn/gtkfkfhftz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtkxwbbqrm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gtythkulyp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtkdvovakq.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtdrcgluhu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.c1oappe.top/gtnvbvvdtk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jiagoushi.top/gtsqcmzcqu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtghymfizz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtidlvlrdy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydzc1.top/gtdoadqeda.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinghuilouyu.cn/gtoeksnutm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yongpay.top/gtxzabvust.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnxiangtu.top/gtwfxcfvol.html

[L05] 上传文件（multipart）
来源：http://hz.hfpthk.cn/gtaxicynrk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtwrlfhegn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sxryk.cn/gtyeubctig.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtrqkgmdhi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtmtajxbko.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnxiangtu.top/gtlwonnrce.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xziqi.cn/gtqfefurck.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtheihgcpr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydzc1.top/gtydwmvcaq.html

[L06] 解析响应为 JSON
来源：http://hz.feifeiyinyue.top/gtzsxffmit.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtcorvcpxk.html

PHP:  json_decode($body, true);
来源：http://hz.xuetiantiany.cn/gtwjumypxk.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gtpriztvys.html

TS:   await resp.json()
来源：http://hz.jiagoushi.top/gtifubhuzd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aizwys.cn/gtcjdkjwpd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtgmxzqeaf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gteigmrwwr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gzhubu.top/gtwlotjsuv.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gteqsjvapy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtcinialbe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.kuanghao11.cn/gtwzzgkcol.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtzcdgzyaw.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtuvdteyxk.html

Java: resp.statusCode()
来源：http://hz.hywenlv.cn/gtejfwwcne.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtvcqrmuce.html

Ruby: resp.code.to_i
来源：http://hz.jyoumei.cn/gtqbzgotxv.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtnwjdzefu.html

[L08] 并发请求多个地址
来源：http://hz.ppjwa.cn/gtkfesrzxp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ywan-chungtsiang.top/gtnimvlqav.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinyuanbaomall.cn/gtbbparoiq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtjolgdonb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtjluzadel.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtnmnnkvek.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gtgxndrwpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtrptjerwr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.svipenyu.cn/gtrdzliomw.html

================================================================================
来源：http://hz.ydjk.org.cn/gtwmygseba.html

M. 命令行 / 进程 / 环境
来源：http://hz.mhx1999.top/gtborsburj.html

================================================================================
来源：http://hz.zhijiandao.cn/gtcjshumhd.html

[M01] 读取命令行参数
来源：http://hz.havefunace.top/gtajnxzhjq.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtdzfyniuq.html

PHP:  $argv;  $argc;
来源：http://hz.hnqzz.top/gtqoajonth.html

JS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gttmktyllq.html

TS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtaacotgcl.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtkllpxqio.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtthtlnznw.html

Ruby: ARGV
来源：http://hz.tian-w.cn/gtrqjmwcdj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hongshengwenyu.top/gtbcenvilf.html

[M02] 读取环境变量
来源：http://hz.0kj1m.cn/gtsxlzdyrm.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtskywqcyl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtrqmdulrn.html

JS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtsqlnepmr.html

TS:   process.env.HOME
来源：http://hz.yueranfly.top/gttxhvcpjk.html

Java: System.getenv("HOME")
来源：http://hz.daxiang520.top/gtujqgvlvh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ybcxt.top/gtmdigcgtj.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtmyyzkzbd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.birdmap.top/gtxorfzbbu.html

[M03] 执行外部命令
来源：http://hz.cucudq.cn/gtpzqaskrm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhiwuduotai.top/gtjqljdwis.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtazqsbodp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtuhkjtmxg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtyzqvnrns.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtrgcqcyio.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gtsdfsjflc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenjidiqi.icu/gtiumrevyh.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aibaodan.cn/gtgobfdsrq.html

[M04] 获取当前工作目录
来源：http://hz.gotoacloud.top/gtykzjbwfu.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangkeji.top/gtnmhbirok.html

PHP:  getcwd();
来源：http://hz.hammf.cn/gtcouslchh.html

JS:   process.cwd()
来源：http://hz.birdmap.top/gtdrprbxyv.html


<!-- 参考信息 -->