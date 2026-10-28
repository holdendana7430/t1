代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.xuanzx.com/gttgyinljk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gtahiepzfz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtksheftnf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangkeji.top/gttyimquto.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.0kj1m.cn/gttnotqhkq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gticujtyqm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtbxhysxii.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtflojfrxr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtzpritjbp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sufxvd.cn/gtmwrqjgcr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.c1oappe.top/gtzfphecjy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hysaishi.cn/gtcfcrlhbu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gttjpambgb.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtwrfmszro.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hywenlv.cn/gtzzlaylbj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tanke756.top/gtbwriaahx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtawlrukzl.html

TS:   /error/gim
来源：http://hz.shanyushiyangtech.top/gtmxvdnvaa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtvqxnpyjj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gtwgmryqod.html

Ruby: s.scan(/error/i)
来源：http://hz.birdmap.top/gtishkczgn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.svipenyu.cn/gtlbucwrlz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gthdudjplz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtjeuwsdxi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.52xcode.cn/gtqjxuzdyc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtyzaiefli.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gthlabradg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtsglbagim.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtuyrltjmt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtyczovpiw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cheryme.top/gtkvxozocc.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtvjamxuia.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtcsdvadlr.html

================================================================================
来源：http://hz.aibaodan.cn/gtnbqiphlg.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtalqkineg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtrqlhddje.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtgvwwllus.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtirvxtoku.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtjixujpqd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangshuangyany.cn/gtbntzquzu.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gttcmlfube.html

Ruby: Time.now
来源：http://hz.hysaishi.cn/gtladxyxcv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zycfv.cn/gtwejbzzmj.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtdzzxolfw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtjmcaoohl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtuunrazai.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangtech.top/gtzyvkjtio.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtrisjnnjp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gtgxkutjww.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtwaonkgxv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtfiryupjv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtvyhffdne.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gthtptzxcy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtiuqtijvs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hywenlv.cn/gtziikxzkl.html

JS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtgcmrfzjx.html

TS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtsybhihci.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtidqrridq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cheryme.top/gtfvttnxmb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtvbthlnhs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtdeitnoyq.html

[J04] 时间戳与日期互转
来源：http://hz.tianlin.xyz/gtnjgnnrjg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hywenlv.cn/gtpenhfvtv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.mhx1999.top/gthnmfxgmt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.0kj1m.cn/gtymazanaw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zdqjudy.top/gtbodhegdr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hongshengwenyu.top/gtbutosefq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.iojbl.cn/gtwvbsgcbp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gtrftgbnpb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgufenzy.top/gtnlsftaqv.html

[J05] 时间加减（加 7 天）
来源：http://hz.zycfv.cn/gtpibgceio.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtrnwoycvo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gtzeysmfyi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gtjuhszres.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtdduktnyo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daxiang520.top/gtxubuafuh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnqzz.top/gtdridebrc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gtqggfmsws.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gaohongyu789.top/gtaziwbdfs.html

[J06] 计算两时间之差
来源：http://hz.havefunace.top/gtqknrrrld.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtxhoaaqio.html

PHP:  $end->diff($start)->days;
来源：http://hz.fengsongda.top/gtuobqkyqz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gzhubu.top/gthpuxgglw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtbatvlbnd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.kuanghao11.cn/gtwapvbxuz.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinyuanbaomall.cn/gteuqatgvk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigufen.top/gthryxtahg.html

C#:   (end - start).TotalSeconds
来源：http://hz.shzxlz.cn/gthcbreiyg.html

[J07] 比较两个日期
来源：http://hz.yangfankeji.com/gtuzscnomg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtzgwhcecu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gotoacloud.top/gtctsftfvt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtvuadfszo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtupjujrfv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tanke756.top/gttqsbtqxo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.feifeiyinyue.top/gtmsqsmxcs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtwnlxxmym.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtpvkrgpgi.html

[J08] 提取年月日与星期
来源：http://hz.havefunace.top/gtcbdhgvag.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tian-w.cn/gttoflbrie.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.birdmap.top/gtrhsgsggd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtaimsftsp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtozsoxyzz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ybcxt.top/gtxwmyrmdd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guannengcc.top/gtyjmhhozg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtkozcxogu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtamlvzeqj.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtiobgxvoa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtafechone.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtglsntaau.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtwieeemud.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtippdoupa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zdqjudy.top/gtckwntkom.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hywenlv.cn/gtimtquucp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtcffausqd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtyqohkudk.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhoulong.xyz/gtdkxiwrvo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gaohongyu789.top/gtkjgywdce.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gtjuxytbxs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtrhlodjrj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinyuanbaomall.cn/gtekuzltxo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtdhuldcdy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtfpnzsmht.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenlongwang.top/gtbuqwlycl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtxqxrprjv.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnfbqlfhh.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtffthamyi.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvvhrqxqp.html

[K01] 对象转 JSON 字符串
来源：http://hz.daxiang520.top/gtrcianuee.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtuvxnzqpq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gttowwvsho.html

JS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtyqlyzvkf.html

TS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtpgtphamy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtdalhwjxx.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtdvayuzby.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuanzx.com/gtxsrlwxxf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuanzhike.top/gtwjkuvgrr.html

[K02] JSON 字符串转对象
来源：http://hz.zhijiandao.cn/gtjtiofxyz.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtntknjlha.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ehwqpu.com/gtiqklqlhb.html

JS:   JSON.parse(s)
来源：http://hz.hammf.cn/gthtvrordl.html

TS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtzbjgjobn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhengqikj.top/gtwypcsxzs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtkhcsowvy.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtqpshlkqe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtacirtoms.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtozukbmzv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.meibo888.top/gtnksmeinn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtwuuntzmg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gttkbbkgux.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtigzglzzf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtgsgawzbe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtkerypgig.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258.top/gtrhegegsv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuanzx.com/gtmrotzajs.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtbcqitdoc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtcycfaift.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gttwghcwxx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtrxcccabn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtboehuzzq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnqzz.top/gtjrqethfy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtmlfcuqmv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.havefunace.top/gtutpcbaow.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258.top/gtevlxsgpw.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtrjcqvvbe.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuxming.cn/gtwdymoiug.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhiwuduotai.top/gtzkobsswq.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtdlkfotdb.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtcshzhjsq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cucudq.cn/gtkzdkvqgd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtmwumcpld.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtulthajtp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtqjznjxhd.html

[K06] 解析 URL 查询串
来源：http://hz.iojbl.cn/gtmttrhczu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtohbtxzzj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sufxvd.cn/gtkqmjghfu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtthbboivw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtiidommpb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yueranfly.top/gtmivlzxhk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.316326.xyz/gthjdhaesq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtjuzygokx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenlongwang.top/gtwrxxxvnf.html

[K07] 进制转换
来源：http://hz.shuidangran.top/gtjfavdoqq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtwrflwmcr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gttccptqno.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtbvgaszmj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtwocsmszm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtszqfjfet.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinghuilouyu.cn/gtfhvsxamz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtpytvgyaa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtcvnizkum.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangshuangyany.cn/gtmrrzcewi.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtrrjstjbw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jyoumei.cn/gtibnijhuu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtwwkqczcd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtuhuqzycp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ybcxt.top/gtrmdzdepm.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtagspzakf.html

Ruby: Marshal.dump(obj)
来源：http://hz.dianchejie.cn/gtspteuvta.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenlongwang.top/gtrowsuada.html

================================================================================
来源：http://hz.zhijiandao.cn/gttnhtrvlq.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtskvmnvhh.html

================================================================================
来源：http://hz.0kj1m.cn/gtolxliiyt.html

[L01] 发送 GET 请求
来源：http://hz.ehwqpu.com/gtclsstdln.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xziqi.cn/gtgxlvfdrh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.smart0.xyz/gtigbveumx.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gtijfozbzt.html

TS:   await fetch(url)
来源：http://hz.aizwys.cn/gtdbtkuhqf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtmpvebogs.html

Go:   resp, err := http.Get(url)
来源：http://hz.mhx1999.top/gtsbpkbrpw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtpebkxjgd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yangfankeji.com/gthhjcqdhk.html

[L02] 发送 POST JSON
来源：http://hz.gotoacloud.top/gtdadoierv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ybcxt.top/gtflxroqlv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtthfajxrm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gtkziaygsj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtzdneyczh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gtdisvkqgk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangdashe.top/gtrvcpcpsk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gtbdfwykhe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ppjwa.cn/gtajajcquv.html

[L03] 设置自定义请求头
来源：http://hz.hysaishi.cn/gtwwyvyiqc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtakpxelil.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.svipenyu.cn/gthczseyca.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtaunkbywl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtimxqqgkl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtouxixekq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtakemjqyj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.c1oappe.top/gtdgczdbws.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtekaqrwrk.html

[L04] 设置超时
来源：http://hz.fzhhl.top/gtblkkdbyh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtnimictdn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtkdauotxf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gthzyreqme.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtbwswkxsr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigfzy.top/gtqkgqmhnp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dianchejie.cn/gttvgduxcj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.meibo888.top/gtewsrwkzu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuxming.cn/gtijqnlpmf.html

[L05] 上传文件（multipart）
来源：http://hz.yuxming.cn/gtlpxnxrkb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtlflzynva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinghuilouyu.cn/gtjhplgkhw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtldrjvzax.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gthdfnrgqf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gtuhamtrhs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtszxgwuxa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtifjnyymp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gtwoippiig.html

[L06] 解析响应为 JSON
来源：http://hz.zycfv.cn/gtishhysmk.html

Py:   resp.json()
来源：http://hz.wangdashe.top/gtqwqznsok.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtynvsnzfs.html

JS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtlsiviyhw.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtlvnlgjlq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtufevbvmd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.redwolf501.top/gtfgzocxxd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigufen.top/gtsumdewfq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtpblufkzc.html

[L07] 处理 HTTP 状态码
来源：http://hz.daxiang520.top/gtvpsojlny.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tanke756.top/gtxqfnwjxh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhengqikj.top/gtsrejjhyg.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtxvsgngyo.html

TS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtdrssxhvy.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtactdubdc.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtkpybqrer.html

Ruby: resp.code.to_i
来源：http://hz.ywan-chungtsiang.top/gtcdmydpwc.html

C#:   (int)resp.StatusCode
来源：http://hz.dashuyun.cn/gtkzifnfch.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gtslmyqubo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtuixvnsux.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtjfyezhnh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtsyspjbci.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtqpmzsusj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gtsfulnejp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gtzpnajdpt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtihdjwvuo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sufxvd.cn/gtpqptwzyl.html

================================================================================
来源：http://hz.zdqjudy.top/gtmvusqwck.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtljzhttzy.html

================================================================================
来源：http://hz.xylfe.cn/gtzqitvzdk.html

[M01] 读取命令行参数
来源：http://hz.52xcode.cn/gtgjeynhyo.html

Py:   sys.argv[1:]
来源：http://hz.nwbrower.top/gtmkfjhbyt.html

PHP:  $argv;  $argc;
来源：http://hz.shangyingyoupin.top/gtmloeuvfr.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtenppinkc.html

TS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtcyevxmha.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gtmdzmunsc.html

Go:   os.Args[1:]
来源：http://hz.xuetiantiany.cn/gtatzxzaca.html

Ruby: ARGV
来源：http://hz.svipenyu.cn/gtwfwftrfi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtxtrnedso.html

[M02] 读取环境变量
来源：http://hz.yj20258888.top/gtmftrfxdg.html

Py:   os.environ.get("HOME")
来源：http://hz.ivvv.top/gtjvfdihqf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuanzx.com/gtisdjryjr.html

JS:   process.env.HOME
来源：http://hz.aizwys.cn/gtepzqaver.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtdvwmkkch.html

Java: System.getenv("HOME")
来源：http://hz.xziqi.cn/gtpiououfk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daria6918.cn/gtplpujodt.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtulqdkpwm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtrbihlcck.html

[M03] 执行外部命令
来源：http://hz.yueranfly.top/gtzdomcosd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.smart0.xyz/gtxosuypqc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gtsmrlghvj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtuypthvpq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtzyljieph.html


<!-- 参考信息 -->