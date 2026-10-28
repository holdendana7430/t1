代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtfddwasnw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.kuanghao11.cn/gtomfhdmfm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtcjzfnjvw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sufxvd.cn/gtutecnnab.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtbgsvjadd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtlctmzbxw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gtohounjgq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtmhlfxiqv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtopyrsxdc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhixingplan.top/gtvxqmvxaa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pengpengdd.cyou/gtzifenbah.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.bjfxy.top/gtacdqkicq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtbspvkyww.html

[I07] 忽略大小写与多行模式
来源：http://hz.yonumen.top/gtcttgatmj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gthplnhovl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gotoacloud.top/gtfzkaeiqg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtqwpxxfdq.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtujltkfzb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aibaodan.cn/gtmjyvviyt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuetiantiany.cn/gtwrromwud.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtetqapnon.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pengpengdd.cyou/gtulnmxxsj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gtaemuooxw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ehwqpu.com/gtnnfwkhhl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtbuiiiejx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtqpwuowny.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtjuknwhmj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtqcshffbp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.9152youxi.cn/gtsenjzetn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxinkj.top/gtpbjyajua.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtynbcspjj.html

================================================================================
来源：http://hz.yvedp.cn/gtovaldcgo.html

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gtpsxktcxb.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcwkekupb.html

[J01] 获取当前时间
来源：http://hz.yueranfly.top/gtkdxsljnk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cashguo.top/gtohiwmozz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtabzjuxuu.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtqmmptwlm.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtpcjroobx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtcwbnmewr.html

Go:   time.Now()
来源：http://hz.svipenyu.cn/gtciuyqxch.html

Ruby: Time.now
来源：http://hz.zhoulong.xyz/gtuzwdsnni.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtwvqkgvaj.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtpwormpoz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtdrakvdxc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtksyrqztj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtodyahqma.html

TS:   d.toISOString()
来源：http://hz.sysykeji.top/gtoxnmdnet.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydjk.org.cn/gtjbmsqlwm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtudaqwqni.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gthgjuhmyk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnxiangtu.top/gttyulhjoy.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gtmqsymzby.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtdtnpucpg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtzrtgerrq.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtwxxwfcig.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtenpripen.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtsyalzjah.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gttojbowcw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gttuogrikd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtuugmcgpm.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtjmnzfngn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtddsrqguw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pycfn.com/gtvvlamqeh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenzaomai.com/gtspikojws.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sxryk.cn/gthwrqtsrc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtlgxllinf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuxming.cn/gttcazushe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtfhjuldyp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jyoumei.cn/gtoybwoqwj.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gtusngejar.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtpbvhqcqx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuxming.cn/gtflckygat.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtbjsrqjtu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtiznhrmdt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.smart0.xyz/gtkdzsosoh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gterzxopql.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtxerbeifz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gaohongyu789.top/gtjlroapjn.html

[J06] 计算两时间之差
来源：http://hz.jinqigufen.top/gtgigkygap.html

Py:   (end - start).total_seconds()
来源：http://hz.jinqigfzy.top/gtrmgjtxyj.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtxtbnciav.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangtech.top/gtgufpnaki.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtwwryckou.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtcjrqkofo.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxinkj.top/gtdvixuhbh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yanxiufei.cn/gtuplpjkdw.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtrnyxdncw.html

[J07] 比较两个日期
来源：http://hz.feifeiyinyue.top/gtoumfutxo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtnqhxgihd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinyuanbaomall.cn/gtxbekpwxc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtdorbydux.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtqodeybof.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtsphqogsx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtvtogzxag.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtcgjdgpcd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtsxkdiqdc.html

[J08] 提取年月日与星期
来源：http://hz.daria6918.cn/gtymqgixfl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtmgbvoprg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ehwqpu.com/gtbtaeegpj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgufenzy.top/gtcumibhne.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtsywwehby.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tanke756.top/gtnkqasyti.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgfzy.top/gtupjbepuc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigfzy.top/gtamurkgpe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cucudq.cn/gtpexjazlu.html

[J09] 时区处理
来源：http://hz.bjfxy.top/gtwlogqjxg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtybnumazh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xziqi.cn/gtyueixvjc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gthanisdpx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtpfhpbhxi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.haohaochexian.top/gtotyapdsm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.52xcode.cn/gtcezqaejt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtpvbucfii.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtwbpkofnl.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtcyldqduh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.meibo888.top/gtbswnctaz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.smart0.xyz/gtxyjqvfae.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ivvv.top/gtnofqvyql.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gtxsilrabr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gttbiusski.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtuecsbuif.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtufdtvkhu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.316326.xyz/gtyhpgnerv.html

================================================================================
来源：http://hz.yuxming.cn/gtqpgnqzfl.html

K. JSON 与序列化
来源：http://hz.quarkkingdee.top/gtimdnmhsr.html

================================================================================
来源：http://hz.guowangkeji.top/gtsuxjsjhw.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtingyqmkt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtbdnkhkro.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtqxxvmrxw.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtvnqmjlcu.html

TS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtkerpnnxk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.meibo888.top/gtapzufmmp.html

Go:   json.Marshal(obj)
来源：http://hz.cucudq.cn/gtoujvhnbc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gtorixpgpu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gtjawzbhsr.html

[K02] JSON 字符串转对象
来源：http://hz.zhiwuduotai.top/gtxpkqxxms.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtxbhfhkse.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aibaodan.cn/gtyeebawqw.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtpkycbghw.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtszyzpupr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtklncqswf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtcxloytrw.html

Ruby: JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtbazimrqt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtlugtzefr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnqzz.top/gtymasfeys.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gttcymotwe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtaxzeswja.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtphorbpps.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtahdrpnwg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtenitmuxp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.haohaochexian.top/gtglrvwndh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtcozatgcn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jiagoushi.top/gtgkroznpj.html

[K04] 读取 JSON 文件
来源：http://hz.guannengcc.top/gtadpovexa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtjskajvis.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gtcnfkfvph.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtccrltbof.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtadqfiicw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gogol.net.cn/gtnsqydrqu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gthykozdlx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtcaffphaw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtaleiwmlo.html

[K05] 深拷贝对象
来源：http://hz.bjfxy.top/gtfpgvgnur.html

Py:   copy.deepcopy(obj)
来源：http://hz.guowangkeji.top/gtrdxkqpnw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnxiangtu.top/gtezpdvucf.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtyimdftmh.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtodxykxiy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuxming.cn/gtguxfgqvj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtphysuwlz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtaiemdthc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtfekzedyi.html

[K06] 解析 URL 查询串
来源：http://hz.tianlin.xyz/gtuemaqexa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cheryme.top/gtclwdtuqw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtznirnkws.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtusuaombd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtnowblork.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtpngiakud.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guowangkeji.top/gtbgutqpsw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtvpuagpca.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.c1oappe.top/gtjbppabxk.html

[K07] 进制转换
来源：http://hz.smart0.xyz/gtqhkrnpdw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxinkj.top/gtxuyqqazt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hammf.cn/gtezmolwuv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtvjkfwryj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtaymrouxs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yonumen.top/gtvdzbdwaa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhongyouzk.top/gtyclfgptc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenzaomai.com/gtzddqfkek.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtobpguums.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xingfuxueyuan.xyz/gtrjbambmz.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtdnydacjg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtiwztdxti.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtvuufdhkk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtzgsjfyiu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtwwnzhgmb.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtlfwrtuvb.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtpuzblhqp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pengpengdd.cyou/gtdgthhlef.html

================================================================================
来源：http://hz.c1oappe.top/gtgeqzqejd.html

L. 网络请求
来源：http://hz.hysaishi.cn/gtzatxqdzl.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtqijabsrc.html

[L01] 发送 GET 请求
来源：http://hz.fengsongda.top/gtsxsefozh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuanzhike.top/gtioczpaaq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtsbnnhuhs.html

JS:   await fetch(url)
来源：http://hz.0kj1m.cn/gttjrcogru.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtzlxmazxg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhixingplan.top/gtpbffxrlq.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtcinlmimw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.haohaochexian.top/gtlmwdsuph.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtmlprgmpo.html

[L02] 发送 POST JSON
来源：http://hz.wangdashe.top/gthrjzywjm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtddousqxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtwoayaezp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtwaxtdtty.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtsigparsn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.9152youxi.cn/gtmmkxpzxs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jyoumei.cn/gtrxrgyntw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuanzx.com/gtcadzitmh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangtech.top/gtrwfsyabu.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtsnapmmuo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fzhhl.top/gtuilmccrz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtkzgjorgi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtehisstcc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gttwyxfgrb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtoklexlsw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pycfn.com/gtjpilshpz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtgoduyurr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gtnebrydqd.html

[L04] 设置超时
来源：http://hz.yangfankeji.com/gtkpvkwilk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shuidangran.top/gtnvewkzuo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gtbmgszmif.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtbbkbyshf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtxtrrmyua.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daxiang520.top/gtoyqvxvhp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pengpengdd.cyou/gtqgugdswz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258.top/gtwccklfde.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.birdmap.top/gtreqidhdv.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtjwxnlvrg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gtkrxoiwaa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtdjglahrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtimavabaz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtrzwstozb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pycfn.com/gtoxuzhthw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuxming.cn/gtizsvpovc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dianchejie.cn/gtoerygvyo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shangyingyoupin.top/gtnsgrzxse.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtradnqeuf.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtmeuvzczn.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtscgenatp.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtrttytdvr.html

TS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtfirnqvci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtyodtqxin.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gtizsuvkml.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhongyouzk.top/gttkpcgoht.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.guannengcc.top/gtxmkcevzi.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtjyjyofmw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.kuanghao11.cn/gtabnplrci.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fengsongda.top/gtzmbfvniw.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtxgfycbqg.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtduqznpjy.html

Java: resp.statusCode()
来源：http://hz.zdqjudy.top/gteorurgyb.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gttvzfcwrt.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtgwejmxup.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtoarntewa.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gtpyywxici.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtxrtgsfdt.html

PHP:  curl_multi_init() 系列
来源：http://hz.316326.xyz/gtzzvjzlva.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtskbwicgp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtcexxkvii.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangkeji.top/gtjmsawgdt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gtpggrechq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtjzdnhfjd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hnxiangtu.top/gtjjeffqeu.html

================================================================================
来源：http://hz.yanxiufei.cn/gtchtrvqva.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gtxhjndpww.html

================================================================================
来源：http://hz.sweek.top/gtcyyboqqa.html

[M01] 读取命令行参数
来源：http://hz.chenlongwang.top/gtbkmdqocl.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtcxjsvetj.html

PHP:  $argv;  $argc;
来源：http://hz.52xcode.cn/gtipvmizdi.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtilqaqbek.html

TS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtsydegcch.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtxvtwcgta.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtmuzzkypm.html

Ruby: ARGV
来源：http://hz.svipenyu.cn/gttqczualr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gaohongyu789.top/gtpgtdkcep.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangtech.top/gtbyqwicxd.html

Py:   os.environ.get("HOME")
来源：http://hz.mhx1999.top/gtifdxsjwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhijiandao.cn/gtdtnqidrv.html

JS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtdbxuxeoc.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gthqkfxsnq.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gtndyhagrf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhongyouzk.top/gtlgdudird.html

Ruby: ENV["HOME"]
来源：http://hz.yuxming.cn/gtwupctspf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtjncluefy.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtcrbsjwwe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtggxxnxfl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nanxuanxn.top/gttojylhhv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gttihnjinm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtqwbwqifw.html


<!-- 参考信息 -->