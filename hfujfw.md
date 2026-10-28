代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtyuezfgta.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtglitcsjr.html

[I04] 正则替换
来源：http://hz.redwolf501.top/gtyqhwzsbx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtawijdcxm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.meibo888.top/gtdwegdupg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gthenhwtoo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtwcvglpwv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xziqi.cn/gtgncfjejf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtlqpeimjd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.kuanghao11.cn/gthtkvbcle.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gtzsubogsc.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtsuekgyhk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtsqjejtro.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtivozurgl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtnmsgdfvh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtiiqslwez.html

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxuanxn.top/gtcuzoihaq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.snrcjt.cn/gtfqthdpaa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtngjcujjz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuetiantiany.cn/gtmsrnyhcd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtzocohbpc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtsclsdefm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gtxuxulmxv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtvdlvccun.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtjsuoafwa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gtxkmzodwu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtixbzfzvd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zycfv.cn/gtysbxsmml.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtkzjahfxh.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtdglgxupj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhoulong.xyz/gthdfsaaca.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtdqheuuzv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtlpjzdhgz.html

TS:   /error/gim
来源：http://hz.bjfxy.top/gttletsphz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shzxlz.cn/gtxqxhzepz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jlsjyb.cn/gtoirwjhxc.html

Ruby: s.scan(/error/i)
来源：http://hz.hongshengwenyu.top/gtjbjqwrwi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinyuanbaomall.cn/gtdspocqiq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenjidiqi.icu/gtpyliclly.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gtncgxymbr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gaohongyu789.top/gtcvrhralt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtxonskgbb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtpstoggdg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtdpalnrgm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fzhhl.top/gtyjgknldl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.quarkkingdee.top/gtivvdmxqf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtjtdbrclx.html

================================================================================
来源：http://hz.daxiang520.top/gtiydyobsy.html

J. 日期与时间
来源：http://hz.cashguo.top/gtjxnkgxlj.html

================================================================================
来源：http://hz.fzhhl.top/gtkobisxcy.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtholrelda.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gtgczgulgj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtsfkodvsx.html

JS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtsomcefzg.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtzvoayxtj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gthfhxlqvl.html

Go:   time.Now()
来源：http://hz.jinghuilouyu.cn/gtvawbkpip.html

Ruby: Time.now
来源：http://hz.cheryme.top/gttxqplbyp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenzaomai.com/gtsthjlznd.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtvqvdqhdm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtllabvtsu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtisxkpqui.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ivvv.top/gthzgpblsg.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gthrzqkcni.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guannengcc.top/gthaxhkemh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxuanxn.top/gtaekckvyj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtqnbvscrq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gtokgkinmf.html

[J03] 字符串解析为日期
来源：http://hz.hnxiangtu.top/gtuabaolvw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gtvldxhdfl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtdhfphpms.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtouppjxgt.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gthuuojaym.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtpffmmnak.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtqlbwoxdb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtebcojpqc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xylfe.cn/gtghwlouzr.html

[J04] 时间戳与日期互转
来源：http://hz.shuidangran.top/gtwumlmjpd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.mhx1999.top/gtjtxtbjzi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gttsbazyqg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtpddkwium.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.bjfxy.top/gtmetjgkea.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yongpay.top/gtfczihung.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinyuanbaomall.cn/gtahbwkoha.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dashuyun.cn/gtnabvdsox.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hywenlv.cn/gtjuohyeqc.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinyuanbaomall.cn/gtrnxclpod.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtchsbpujt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gthizpecez.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtevwnbdtc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtdpulqmiu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtcklevevf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gtretarvtm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtqyfrfwea.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.vqdsnc.cn/gtapdsahnv.html

[J06] 计算两时间之差
来源：http://hz.ivvv.top/gttjoorjbg.html

Py:   (end - start).total_seconds()
来源：http://hz.cdnleiting.top/gtxkevyuxd.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtpddzverg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtmavszqen.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgufenzy.top/gtdreybnec.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.snrcjt.cn/gtmvlsszhv.html

Go:   end.Sub(start).Hours()
来源：http://hz.52xcode.cn/gtjiaqvdgz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shangyingyoupin.top/gtgocuiwrw.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gtxocphugb.html

[J07] 比较两个日期
来源：http://hz.xuanzx.com/gtkyioyztu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtbttcjyac.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gttyuvjcrs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtbcjocjmh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtcppcdwuc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.bjfxy.top/gtsdytzmve.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtaqukazky.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtqbovqxaw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gttnnqgvzs.html

[J08] 提取年月日与星期
来源：http://hz.hysaishi.cn/gtngqfmdgn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cashguo.top/gtfuhljggq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gtcckwzyzz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtpywovxxa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtsortmali.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sweek.top/gtpnpsmcas.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtucgwkydp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.52xcode.cn/gthmhvagvv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gttvuszshu.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtcycfkcej.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gtntnzywwu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtbkxnwfqr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtbzlgkzug.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtryafjoqz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtzfjnkyro.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shzxlz.cn/gttasohsft.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.0kj1m.cn/gtbtmqsmsh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gtrqwoqksu.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtmwcaogmn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gteejsauur.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtwgcmjrfx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtdumwmksa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenlongwang.top/gtspmguksd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zycfv.cn/gtcxnckpju.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tianlin.xyz/gtrerooyxy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuxming.cn/gttylffogn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtusueembt.html

================================================================================
来源：http://hz.cucudq.cn/gtweurnbhi.html

K. JSON 与序列化
来源：http://hz.hammf.cn/gtjxeaqhhs.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtcnxeqqms.html

[K01] 对象转 JSON 字符串
来源：http://hz.andypj.xyz/gttrgczrqd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtkrxhgttc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtwlgvjutw.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtjdssnhsa.html

TS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtozjfpnpx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtrmueaeyc.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtcnxgwohs.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtwdppzklm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtbsmwdmgz.html

[K02] JSON 字符串转对象
来源：http://hz.tianlin.xyz/gtlppmaiqp.html

Py:   json.loads(s)
来源：http://hz.ppjwa.cn/gtbetwhjzm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gtzqlcijpf.html

JS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtzctyexkf.html

TS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtkqfbafrl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gtzyiyaafx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtdbfnakqp.html

Ruby: JSON.parse(s)
来源：http://hz.yuanzhike.top/gtzittcebm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtbdwtynvf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtwaxjlmzm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtokijospc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtjekkwsuv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtptmkrfgd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtrldmtgmc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.snrcjt.cn/gtrvbrfjdc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtmjpaxtpo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.316326.xyz/gteygamncj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtidaseizy.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtxalvcniw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangdashe.top/gtsvqxzkkr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gtgqeesnyk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtlzxtyzso.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtvlrzkjci.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtoczvojjo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtczxgzupk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tianlin.xyz/gtxudkftsm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtfwqgukzj.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtqmjkgpmc.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtibntsgip.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtcophbqay.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtlnpxmfhf.html

TS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtstxmeakn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtlwziigve.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tianlin.xyz/gtougnzcfa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtjvxuwulh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.snrcjt.cn/gtsigqppzj.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtereyfzwn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gthquhekle.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtwkoqdyxv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtkvvjmibp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtofpljrsm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hysaishi.cn/gtirxdjhnd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtfulhuphm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtfcjyujnk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtunzscrmn.html

[K07] 进制转换
来源：http://hz.aizwys.cn/gtpbqiduiz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuanzx.com/gtttxjnigt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.snrcjt.cn/gttzncqlmu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gttinhqnvv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtippbwlii.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtreqxwoav.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtbbziegvb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.meibo888.top/gtrdjppilk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gttdgsqhvb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tian-w.cn/gtaffiggeq.html

Py:   pickle.dumps(obj)
来源：http://hz.chenlongwang.top/gtuedwkbfj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sysykeji.top/gtolxvfsze.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtncrubbji.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yonumen.top/gtnreunyyw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gttqgjnpad.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtpukzsqti.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gttrkggpyn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtetkobnrw.html

================================================================================
来源：http://hz.jqgufenzy.top/gttekofxeo.html

L. 网络请求
来源：http://hz.ppjwa.cn/gtecpmzzrc.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxaogticj.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtkfovgmtj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhengqikj.top/gtlshvofue.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ybcxt.top/gtqzwcbvzp.html

JS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtwbcbyscr.html

TS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtpipkoqat.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tanke756.top/gtqtjfwkpk.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gteqlnsaaz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gthvwymopj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.meibo888.top/gtodbkwrlf.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtfnwypjqz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtcfnyjccg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtjsyuwahm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtsccyvpno.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtfgrraovt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtolnqzggc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangtech.top/gtuquoiqod.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ehwqpu.com/gtsbynxviw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pycfn.com/gtornqcfzq.html

[L03] 设置自定义请求头
来源：http://hz.guowangkeji.top/gtvsxyiaor.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtjnzqtere.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gzhubu.top/gtklwssetj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtwkimzkni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtvyjbqqgb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtfgwwqgbg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtersqpldj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ivvv.top/gtkkjunnfe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yongpay.top/gtmjmkkbpj.html

[L04] 设置超时
来源：http://hz.nwbrower.top/gtmgwfmyhg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.smart0.xyz/gtnwhprind.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zycfv.cn/gtkkwfwssd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtvijfwogs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtizhuvcvq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhoulong.xyz/gtiwwcclrx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangdashe.top/gtffeotwmm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.c1oappe.top/gtoruyoalr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gthkwxyyga.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gtbyonqzyl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtxdkefnnf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.svipenyu.cn/gtwcnsjtzm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtnsyqfnmj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtkpgnquzo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shzxlz.cn/gtnwapxuao.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtesszujoo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhaomingkeji.xyz/gtgkeolpno.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jyoumei.cn/gtjvlccdmm.html

[L06] 解析响应为 JSON
来源：http://hz.zdqjudy.top/gtfunykhqu.html

Py:   resp.json()
来源：http://hz.yongpay.top/gtnqwnbwip.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gtejishfmy.html

JS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtnpnnxkza.html

TS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gttdoxgezr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shangyingyoupin.top/gtkjcopksd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtipflluwu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhiwuduotai.top/gtbzkryoqb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nwbrower.top/gtpofbaspt.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtqzmcbgmb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinghuilouyu.cn/gtfihphyai.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangkeji.top/gtvrohbogl.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtilzqzzty.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gttujmjhsz.html

Java: resp.statusCode()
来源：http://hz.bjfxy.top/gtvfttuuuv.html

Go:   resp.StatusCode
来源：http://hz.shuidangran.top/gtdwvotfkx.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gttljfduul.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258888.top/gtyquhsmmr.html

[L08] 并发请求多个地址
来源：http://hz.yj20258888.top/gtrvamwrsl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.iojbl.cn/gtewibxdus.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtyebsxfwp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtpvjebfca.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtuuxonxln.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtdblbuezs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtbxrhnctx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtewqcjxyu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydzc1.top/gtrwnvlhes.html

================================================================================
来源：http://hz.yj202588.top/gtfqsmbbfn.html

M. 命令行 / 进程 / 环境
来源：http://hz.mhx1999.top/gtbpqslfzw.html

================================================================================
来源：http://hz.jianghu66.top/gtvptkoglx.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangkeji.top/gtkabkmjev.html

Py:   sys.argv[1:]
来源：http://hz.0kj1m.cn/gtnsgyqhlx.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtygjfytvy.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtnawpqbgl.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtnmzgximf.html

Java: args 数组（main 方法参数）
来源：http://hz.xziqi.cn/gtuaxjmyrr.html

Go:   os.Args[1:]
来源：http://hz.jinqigfzy.top/gtpxaklxvj.html


<!-- 参考信息 -->