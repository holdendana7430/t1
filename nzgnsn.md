代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtcbmylryu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtcjamacjr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtrwsxhpjh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xylfe.cn/gttwmwxvxx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yvedp.cn/gtyilclgbt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shangyingyoupin.top/gtupeqvmsx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gtyyaxdurp.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtcxmtbgqt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hywenlv.cn/gtwyahqxpd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydjk.org.cn/gtsibihril.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtfzuutkqg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtzxogfhey.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigfzy.top/gtwfuxxodv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtizqoveqn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtppxctlse.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.haohaochexian.top/gtbzpobzux.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtqmdchjja.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aizwys.cn/gtyprwozmd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sxryk.cn/gtfumutsnc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtdeojeqtq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtljjglxjd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtwixltdml.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gthsupkejt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtnrywhlfx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtpavnxrue.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangshuangyany.cn/gtsnayipay.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtfvwjvcln.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtbintlymo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ehwqpu.com/gteakogwfs.html

TS:   /error/gim
来源：http://hz.hongshengwenyu.top/gtxmxtksxv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gtigfhdjnc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigufen.top/gtcijqrfir.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gtztvzahbx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtjjsulxxr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnxiangtu.top/gtqwzapske.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtoaqvgcxy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtpiwrhmgk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtqgllkfox.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtbyxgrfgm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtrwsngwsr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.mhx1999.top/gtfixbbirg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtullmjfjg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtgvxzhniz.html

================================================================================
来源：http://hz.gotoacloud.top/gtgsrqffsy.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gthgjqnqru.html

================================================================================
来源：http://hz.dashuyun.cn/gtehgciqhv.html

[J01] 获取当前时间
来源：http://hz.bjfxy.top/gtwcisfbrm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtgzqdjoco.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtvjzgxnee.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtlpxeqtxv.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtyrpmcijr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangshuangyany.cn/gthuxsnyfe.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtvnsrdikx.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtjcwjeott.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuxming.cn/gtbmuearxw.html

[J02] 格式化输出
来源：http://hz.jinghuilouyu.cn/gtxrylpioj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtovbdoqbn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtrgimmmyc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtifvzlibd.html

TS:   d.toISOString()
来源：http://hz.cheryme.top/gtwzoarhvw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtzkaizhuc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gtnehposxj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtmucbhkmw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gtzzddrhgg.html

[J03] 字符串解析为日期
来源：http://hz.guannengcc.top/gtfnplhwzt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.birdmap.top/gteebfkfyf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.feifeiyinyue.top/gttjkxcuyq.html

JS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtmvctayho.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtwxlhzpgu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtioyfxoet.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtobdgkiwo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtlpqkhpho.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gtsishwsws.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gtylbsndpm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.52xcode.cn/gtacfzjmbw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yongpay.top/gtwyjbhdbg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.vqdsnc.cn/gtkmrwuqug.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtiuuqwahc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gtjbowwbfi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtawnrsddx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jianghu66.top/gtghdrgxra.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fzhhl.top/gtrcqfetos.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtajpuzovd.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gtssmuorbr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtqlddvrmm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtqxymjnvl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtsygnevpr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gtwnkzwkcn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtysaslkcz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.mhx1999.top/gtxjirngoi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hywenlv.cn/gtmcsxqxzs.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtljfboohv.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gteidnqdei.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtoviexxnr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hfpthk.cn/gtatxmydgr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtknlcpiuz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhoulong.xyz/gtxabvpapw.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtvhsfhszn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hfpthk.cn/gtaabmldvc.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtmgqkpjfa.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtujxloyfn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtexuhgjoy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhongyouzk.top/gtpyxnoesn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtkecpdsll.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtyierrhtp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fengsongda.top/gtguskhkaz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ywan-chungtsiang.top/gtiwmtjuux.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtrapmlitb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtbhudfbiw.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtnbaqlhdc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtnbxuqrxm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ivvv.top/gtcdhbqfpu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ehwqpu.com/gtbaduuoco.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtxxxuyemb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258.top/gtveuocvfk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtnfkdwcqa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhijiandao.cn/gtastvouxi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258.top/gtsqbzfyic.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtewprngjh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gtchiwdxrs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxinkj.top/gtycqjbqlq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gthoxhbjbr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtrwhwrurs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.c1oappe.top/gtktrlpozc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigufen.top/gtxymfbcug.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtlrbaaaps.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gtjjhwisui.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtzevkkbtk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtayatubhm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ywan-chungtsiang.top/gtbtzadfkm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gttsqfgzgd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hysaishi.cn/gtrkstydtx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtyvyyqfvk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhiwuduotai.top/gtbksibobq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gtlejbqpxd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtacnomxzu.html

================================================================================
来源：http://hz.gotoacloud.top/gthownlwfn.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtmqhppbot.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gthteoqcxf.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtxoaoldwq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtpmkcsuye.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtreuxfihb.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtswklwrqm.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtabicysuk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gtewucfubd.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtlzkccljt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtxywpdtsr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtkkietnfq.html

[K02] JSON 字符串转对象
来源：http://hz.yj202588.top/gtsjwfoiuo.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtqspqqrmu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtkzhqlasl.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtsxsqzgef.html

TS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtcrwdntyb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtoqkdjpyv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtbfugsjtg.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtzsqlvjlk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtcmrxjmct.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtqvxagoyy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtsetjnlny.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtbnzczmeq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtxlsnzqwh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtqeblrxbm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtkxwbzxif.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtotkarcuo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xylfe.cn/gtbrfzmfzc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtwnwxitbb.html

[K04] 读取 JSON 文件
来源：http://hz.yvedp.cn/gtycpxaeud.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gttaziirvv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xingfuxueyuan.xyz/gtopkmgrwr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtieadoexj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gtxpfbibal.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtpjebbqfo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtaendivtr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtkgwxuzzf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtsrvfegmv.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtqjbusrla.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtazkemsef.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtzxlizggt.html

JS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtcsapargw.html

TS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtoxbtpbgi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenlongwang.top/gtopgyxwjm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtiymnvdxr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenzaomai.com/gtthbaabev.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ywan-chungtsiang.top/gtrhvcptat.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtjznmfype.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.svipenyu.cn/gttiydgwnl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shzxlz.cn/gtrrpyktra.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtymooawaf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtlmbagwpz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtcllrwwmg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtwugcmxbu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ybcxt.top/gthrhqxitw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtwalkoaud.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtfmdselom.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtgluzzwbs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuetiantiany.cn/gtfqeliykz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtavazltlm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtallcbpis.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtoliwuzbj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtsjrwnjfh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.0kj1m.cn/gtwpsmghes.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuxming.cn/gtchlqplqx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xinyue.icu/gtxypbkntb.html

Py:   pickle.dumps(obj)
来源：http://hz.iojbl.cn/gtsehvqmji.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fzhhl.top/gtdbozbnpo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtspvmzwov.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtmmocyooj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtrpdnpdey.html

Go:   encoding/gob
来源：http://hz.ydzc1.top/gtvpnpdcmc.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhoulong.xyz/gtdpcbevew.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gthjustxpp.html

================================================================================
来源：http://hz.aizwys.cn/gtkgucrfxy.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtllqkukid.html

================================================================================
来源：http://hz.xylfe.cn/gtjrdnylxi.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gtixjaxuby.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gtkigxcsla.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtvmsdmhdi.html

JS:   await fetch(url)
来源：http://hz.aizwys.cn/gtcliupbsp.html

TS:   await fetch(url)
来源：http://hz.sysykeji.top/gtnmcvmsci.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.c1oappe.top/gtrtpsbpjb.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gtdxzajjjq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.andypj.xyz/gtlhprynig.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtfpqobjcz.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gtksnnvsal.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtekjjlofg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtnzpdlukp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtgjzipznr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtneqvsqkh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xinyue.icu/gtryxgvtmb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhengqikj.top/gtnusfggoa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtfbohnrny.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtkcbtbips.html

[L03] 设置自定义请求头
来源：http://hz.yongpay.top/gtrffnzknt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xziqi.cn/gtqqhxfazt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtlqeazrdx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtverqovvg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtgkxamphe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtqpgmwjds.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtbysteuhs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtzqscymdr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtbfhpwvlv.html

[L04] 设置超时
来源：http://hz.yj202588.top/gtdmxzmzkp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cdnleiting.top/gtamhxkebw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gtuelrcqai.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtdjwybywi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtjktzfole.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aibaodan.cn/gtespbyubg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cashguo.top/gtctkruzsx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtpabhvzrv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gteepnhhgq.html

[L05] 上传文件（multipart）
来源：http://hz.xuetiantiany.cn/gtwianubtn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtkvahnluw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtwdkxwhei.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtclopqeku.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtnnqmmczg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gttobgmeqs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guannengcc.top/gtumdjxtbo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtsgqpourd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shuidangran.top/gtfuvxlzae.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtfadeudis.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gtctfccjod.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtttlwkwdt.html

JS:   await resp.json()
来源：http://hz.daxiang520.top/gtuwzguhae.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gtnjjhxgwy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gthkicuoyz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.iojbl.cn/gtpdsslqpv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ivvv.top/gtxobmqorx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtxqzjhkjd.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtzikypvcd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtvftodndh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangtech.top/gtqxljwrfe.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtserajeln.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gthrkiqutr.html

Java: resp.statusCode()
来源：http://hz.fzhhl.top/gtxdquyrcg.html

Go:   resp.StatusCode
来源：http://hz.hnxiangtu.top/gttgfmbjij.html

Ruby: resp.code.to_i
来源：http://hz.jianghu66.top/gtoufwknux.html

C#:   (int)resp.StatusCode
来源：http://hz.cucudq.cn/gtaafrsioj.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gtihvsrryi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtxhdasnlq.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgufenzy.top/gtsczeexur.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.meibo888.top/gtkfsjskhi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtntmwquoq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgfzy.top/gtjryfpfun.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gthgeqkovy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtkrpkdstr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.c1oappe.top/gtyuhplons.html

================================================================================
来源：http://hz.zhengqikj.top/gtxfpwssuh.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gtegqogwcg.html

================================================================================
来源：http://hz.yuxming.cn/gtvtkofmdu.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtdioilssh.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtpkhxzjxa.html

PHP:  $argv;  $argc;
来源：http://hz.fengsongda.top/gtykcgvqll.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtcniwsyxg.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtnzuzsnva.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gtzejbzzqr.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gttbrqzkyg.html

Ruby: ARGV
来源：http://hz.smart0.xyz/gtaubmvwzt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtkpurhsgi.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtqynszdwg.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtbvtvupzo.html


<!-- 参考信息 -->