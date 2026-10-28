代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtwptesmja.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gthytvrbvd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtknyejujv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtvdqwmyld.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gtbhixtdms.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gzhubu.top/gtisxishnc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gtkurdaofy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtmiichfzm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtzzghsuoy.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtpttpiakh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gttrsttpcv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtauebrhfz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtxeizqbql.html

TS:   /error/gim
来源：http://hz.9152youxi.cn/gtnrxmjgpl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtuccfyqlt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.wangdashe.top/gtjuthovtf.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtdnstivnd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtytteosbd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.snrcjt.cn/gtbtzltqfk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.birdmap.top/gtyxstpgxv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gaohongyu789.top/gtuslwkgam.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtdsikcteu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtximxworg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtrkoxodrf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sweek.top/gtqrxiemhv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gtqljwnmhu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtdxjaatio.html

================================================================================
来源：http://hz.gaohongyu789.top/gtydmltrsj.html

J. 日期与时间
来源：http://hz.xylfe.cn/gtfhcodncw.html

================================================================================
来源：http://hz.pycfn.com/gtwwrlpnix.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gtahpthvwc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtmrwxxken.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtwnswyzzu.html

JS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtnvtestyd.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtejvywdeu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ehwqpu.com/gtmktiiyvn.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtrrwkprxc.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtluarqerx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gtgkfzouyg.html

[J02] 格式化输出
来源：http://hz.mhx1999.top/gtbbupxzck.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtdekxzrdq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtdzyroecw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hfpthk.cn/gttogvfgtd.html

TS:   d.toISOString()
来源：http://hz.xziqi.cn/gtzwirlngh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gtzrvewghg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtsftvzncq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtlzewyctp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxinkj.top/gtshgbcbqk.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtwrwophkw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtyldinugy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtcnschezj.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gttomqbfwb.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtvvqodiqc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtgeizdrhw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yvedp.cn/gtzxiyylox.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gttfbswddu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gthfvrqszy.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gtzzdeatyo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.quarkkingdee.top/gtouortnvi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.meibo888.top/gtahksjpvw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.andypj.xyz/gtmtokorti.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtlpjheqwz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gtljwqmzio.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daxiang520.top/gtiuvpejrt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gturflxach.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.meibo888.top/gtprmjvcur.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gtitstgvzc.html

Py:   now + timedelta(days=7)
来源：http://hz.pengpengdd.cyou/gtizttzlzs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtsuikfsoh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtltbnqrhs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtgjsuikkc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gtzonypoue.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zdqjudy.top/gtvprbrkqb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.smart0.xyz/gtyetlzwfe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gthurygqxg.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtmkykvguj.html

Py:   (end - start).total_seconds()
来源：http://hz.hnqzz.top/gtfwdkxkll.html

PHP:  $end->diff($start)->days;
来源：http://hz.mhx1999.top/gtyfrwjdcu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jyoumei.cn/gtapcjbaud.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fengsongda.top/gthjmukjki.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xziqi.cn/gttiznjsmu.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtvswijkyh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gtenjckgna.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258888.top/gtrrccwuqm.html

[J07] 比较两个日期
来源：http://hz.feifeiyinyue.top/gtbiroksxz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtdmflsmga.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtuxzxkvzr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtxhcmpdoq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtvxahtnpe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtaxgpcmcv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gtvpaezrkz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtycpvvoow.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtfdjrqlwq.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gttdedxldt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtpgjavdph.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxuanxn.top/gtmfcyecqm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ywan-chungtsiang.top/gtazshtnmw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gthcgfopqy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yanxiufei.cn/gtrohaaoto.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.kuanghao11.cn/gtwkhuropr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.havefunace.top/gtfoqnzvfm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gtzvtykxjx.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtifdqouqp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtdkrzftxo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtjmjyupid.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gtbjollpvl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtecannmma.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangtech.top/gtqiegijtl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtpmdsobrl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gtovfjlnsp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xinyue.icu/gtoqhdglfm.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtxhvrjlwv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xylfe.cn/gtqbddklda.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yueranfly.top/gtxjcaxozd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jyoumei.cn/gtombikvaw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtsdfffqal.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gthbqhyxob.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtauvqdgzt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhoulong.xyz/gtsfsqltyr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtsjcbpgry.html

================================================================================
来源：http://hz.52xcode.cn/gtxbdnrhth.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtornskvba.html

================================================================================
来源：http://hz.aibaodan.cn/gtmkjmzulu.html

[K01] 对象转 JSON 字符串
来源：http://hz.mhx1999.top/gtgkxjcuij.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtfethtnqo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtzysjzend.html

JS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtwdlasqzb.html

TS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtovfsjmbf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtqepsohkd.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gtlalhrluk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhengqikj.top/gtpoanwzqx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gthbriuglr.html

[K02] JSON 字符串转对象
来源：http://hz.shzxlz.cn/gtmcyxnamr.html

Py:   json.loads(s)
来源：http://hz.shzxlz.cn/gtuctynlmu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtyrqovtxv.html

JS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtcmtiuxij.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtkfatyggv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yanxiufei.cn/gthlnexysw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtumvwdomf.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtlxporvoi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtlbltqvfi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.c1oappe.top/gthdqthgkn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gthwibfylg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtetujffec.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xziqi.cn/gtieqlvrhs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtetcmvgbr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtdglwendj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.svipenyu.cn/gtcmvvqqxv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xziqi.cn/gtrpumuctu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtnlckeegt.html

[K04] 读取 JSON 文件
来源：http://hz.nanxinkj.top/gtizsvbjpy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtqkbqashu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtjchejltz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtnzwgcmvt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtwyitoktw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtsxgcmvwy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtsbubjcuj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hysaishi.cn/gtvgimvpvx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sufxvd.cn/gtzlwqeaon.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtgxlrrjle.html

Py:   copy.deepcopy(obj)
来源：http://hz.wangdashe.top/gtlwbffcaz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtnfhporch.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtujwvlejh.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtktovdivx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gzhubu.top/gtlabqjnyj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gotoacloud.top/gtkzkoyjaj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangdashe.top/gtgkvjifql.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuxming.cn/gtysexkwfx.html

[K06] 解析 URL 查询串
来源：http://hz.haohaochexian.top/gtyruvnpfc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinghuilouyu.cn/gtzmtwnmjl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtvjvjnngg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtcmnoecls.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtnabjhcto.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhiwuduotai.top/gtiidjkyzs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtoqhsgwhb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yvedp.cn/gtfsmnmous.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtqewhydxv.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtzevubbxf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtxmcecvgv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.9152youxi.cn/gtllgwogpg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtqfkkzntz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtkccrbadg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtlhmvbugd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shuidangran.top/gtduthbmcp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtoudjkven.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtpqzbxygn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtyjmtrjmu.html

Py:   pickle.dumps(obj)
来源：http://hz.bjfxy.top/gtfdxmlyef.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtavqwdodu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtamcbrmhd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtanxdvsul.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.smart0.xyz/gtejgadeyf.html

Go:   encoding/gob
来源：http://hz.ppjwa.cn/gtntkcvwim.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtgvmhvthq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtheuragfk.html

================================================================================
来源：http://hz.hywenlv.cn/gtafxlddmb.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtzdkrhqhc.html

================================================================================
来源：http://hz.yonumen.top/gtfeqstxvr.html

[L01] 发送 GET 请求
来源：http://hz.zhaomingkeji.xyz/gtjbhqdsrv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhiwuduotai.top/gthacolzdz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.0kj1m.cn/gtxmorsjtx.html

JS:   await fetch(url)
来源：http://hz.yuxming.cn/gtsuupeopg.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtqbntzhku.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtnlgbxwge.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtcieoadyb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gogol.net.cn/gtidvcuxdq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtrywzrwis.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtqdnsgdpe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydjk.org.cn/gtqqfxecdw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xingfuxueyuan.xyz/gtqhgesukd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtzqwpfstc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gtarabbmgl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xziqi.cn/gtvbnymggd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhiwuduotai.top/gteyppusxo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xziqi.cn/gtpfbbdjwt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtupzupmjc.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtcbbjyluu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.9152youxi.cn/gtlbkjdjzj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtuuxqkypb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gthxvbfwlm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtrfbzwsum.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.0kj1m.cn/gtrsmxknmz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gtvipbhnun.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhixingplan.top/gtjymrvtxw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtnjufylfy.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtocqaghbj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtcorzzgij.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinyuanbaomall.cn/gtejonqrtf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gttkfynfae.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtktmxkqqn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.bjfxy.top/gtvbyhbmdn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guowangkeji.top/gtffcmzilv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtjpqizubl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtxcbllpyz.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtbkageyhz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtppadvsgb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtfztupuwo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtysjfqeuq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtwhrjufkg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtzlutgvqe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jianghu66.top/gtnfjxxzxv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtgblrgpwr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sxryk.cn/gtudrlrytl.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gtdiqapdxw.html

Py:   resp.json()
来源：http://hz.wangdashe.top/gteqbwiems.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtpygztebb.html

JS:   await resp.json()
来源：http://hz.316326.xyz/gthohviugx.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gtxfkywktc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtgvzvjgnb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtxkcufjwl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yueranfly.top/gtipigovlg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.redwolf501.top/gtncxyuekt.html

[L07] 处理 HTTP 状态码
来源：http://hz.ppjwa.cn/gtieiunpqx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtmnnydxta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gthtiybcne.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtshfalfah.html

TS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtycbubgut.html

Java: resp.statusCode()
来源：http://hz.yj202588.top/gtppdipaug.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtzilctdxw.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtuqjpilqw.html

C#:   (int)resp.StatusCode
来源：http://hz.yonumen.top/gtpewbejav.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtbbrrixwf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangkeji.top/gttskmmydv.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtyefqdnbr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtcglmirsy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtojincjnu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtbmshljgz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtagonbiav.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhixingplan.top/gttesykrrr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hywenlv.cn/gtnvcbiurr.html

================================================================================
来源：http://hz.xylfe.cn/gtnhgturit.html

M. 命令行 / 进程 / 环境
来源：http://hz.smart0.xyz/gtbmhsuwpr.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtsjtkwsjh.html

[M01] 读取命令行参数
来源：http://hz.chenzaomai.com/gtflrxxvcj.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gtonxcrfwh.html

PHP:  $argv;  $argc;
来源：http://hz.vqdsnc.cn/gtgqapijpu.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtkhgykifa.html

TS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gtftdqbndf.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtxucbihlr.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtrrvwctga.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtzcgxjgbi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gtnfmxofuo.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtzmniaeaq.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtozdxesvh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gteerodxll.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtutmztixe.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtomtmszdj.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtfkteocar.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gttqfitacv.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtoullmxgo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtcqewkpty.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtlauavice.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gtmistsxeg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daria6918.cn/gtdtlydnyo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtxqdbgxlj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jlsjyb.cn/gtosmumfdt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gtfnwztzas.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sweek.top/gtkirbuurs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shzxlz.cn/gtdeqzbzei.html

C#:   Process.Start("ls", "-l");
来源：http://hz.0kj1m.cn/gtvxrdttlf.html


<!-- 参考信息 -->