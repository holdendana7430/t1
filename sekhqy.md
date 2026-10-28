代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtlnwuygkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtzoipdjrv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtwtchvzhb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.bjfxy.top/gtmvdbelfb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtifhdiimf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtajxkdefh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gthsirbpyh.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gtetrnallf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtjrvwzsnk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shangyingyoupin.top/gtsututyrt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtswmnmsok.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtvnizrrar.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtahibnreu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtymhftdto.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gthsbqcpzk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigufen.top/gtuadalfle.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yueranfly.top/gtjbtfxvhj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtgtvealzg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yangfankeji.com/gtllpjhace.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtxyewjwsp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtrjuwzkbb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtsfexgmfd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtnarzmffr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtczhnhhhm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtfwwfiape.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenlongwang.top/gtzfuvvsvi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hammf.cn/gtecytrtfx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hfpthk.cn/gtclqozovs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtpwqmtbnz.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtsgzjlysa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fzhhl.top/gtefezpfzk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pengpengdd.cyou/gtjtdflxwo.html

Ruby: s.scan(/error/i)
来源：http://hz.zhengqikj.top/gtnjngyimi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.redwolf501.top/gtxlrdegkp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gtalafrsvu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhoulong.xyz/gtycwfwinx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.andypj.xyz/gthhufgncc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtfwciwagf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtplxfutoi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtwagmoqbr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtuvcmngoq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtfflkrelw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtenptyihf.html

================================================================================
来源：http://hz.zhongyouzk.top/gtebozedvh.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtrvvgceyy.html

================================================================================
来源：http://hz.smart0.xyz/gtohwbxmts.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtmwngtrws.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtjvudjibt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtppxfpwzw.html

JS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gttesimfvs.html

TS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtffqfvdvf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtvmcwbbjh.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtiiyjgofh.html

Ruby: Time.now
来源：http://hz.zhijiandao.cn/gtxcxbwrzp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtpzycugye.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gtdxwbatoc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtbxjlbuae.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtpvgoshss.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtbfplrdwe.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtbhubkdov.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtfyunrdfe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.svipenyu.cn/gtvhstmdjl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtghazebwr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtyoepvgph.html

[J03] 字符串解析为日期
来源：http://hz.hysaishi.cn/gtfvowntfi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtbjirwttu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuetiantiany.cn/gtpxjaqgbf.html

JS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtouiqoonr.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtaemvrlzt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtgccbwvzc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuanzx.com/gtducqchel.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtluxrwgoz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sxryk.cn/gthsgmpbjr.html

[J04] 时间戳与日期互转
来源：http://hz.iojbl.cn/gtcgizwfze.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gtmorrfqdp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuetiantiany.cn/gtjurutadl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jiagoushi.top/gtsosrymyj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtekaicivm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtqnqhivdw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangshuangyany.cn/gtuygaxyzj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ybcxt.top/gtrnvnvesd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sweek.top/gtcbsfopqe.html

[J05] 时间加减（加 7 天）
来源：http://hz.c1oappe.top/gtkifbnpdd.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtytulimtr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtppkixupn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtnlqusmph.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtjjdzipus.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtbyhcgwuh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtpnviryrq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ivvv.top/gtvbksohol.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtfvwntazt.html

[J06] 计算两时间之差
来源：http://hz.daxiang520.top/gtooyfmptk.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtbdgwzpjr.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtayvdvumt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yonumen.top/gtfnuodedg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gttgjxdlpy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hfpthk.cn/gtuoxeearp.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtyyskjyjq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtrfgdhjxi.html

C#:   (end - start).TotalSeconds
来源：http://hz.guannengcc.top/gtjctoaipq.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gtqiuhzzfb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtftvdtcwp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yanxiufei.cn/gtizqgfuuz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtsxnpumkw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtyzdflcdx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuxming.cn/gthtdqpydu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gthbpnqwpm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gttryegxwz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtgcjnkaak.html

[J08] 提取年月日与星期
来源：http://hz.quarkkingdee.top/gtdqmwjzgo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fengsongda.top/gtckwokcgh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gturlsdngo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.redwolf501.top/gtvssvgfub.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtjzkticcv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtzqtrhjic.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtlppgipys.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xinyue.icu/gtfhtdoyep.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xziqi.cn/gtfaeqodzf.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtkboilpoe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yonumen.top/gthwctzgxx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hongshengwenyu.top/gtymknmbai.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtfmtqdeib.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtxowlkhom.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xinyue.icu/gtizdkyajn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtmaxqsjxe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtbnvqjdfj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtqzqfgfhk.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgfzy.top/gtndrcqmry.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yongpay.top/gtgacwxxvr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtgeuyzeyy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yueranfly.top/gtudzrbiuo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtszpljqmc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangshuangyany.cn/gtqqabhcwa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gtgoycelvr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cucudq.cn/gtspvbaqlv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guowangkeji.top/gthsdhqlwc.html

================================================================================
来源：http://hz.jianghu66.top/gtggncnvgj.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtcjmemncj.html

================================================================================
来源：http://hz.gzhubu.top/gtwjrymqfk.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtnqfgjixi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtkkivnzcm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtkcqdfkhd.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtpnwnmqjp.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtpjpofvwl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtbbjevaly.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtqsrkjzbr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtkhyeulud.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtttgpjjkv.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtgzkqvxwq.html

Py:   json.loads(s)
来源：http://hz.kuanghao11.cn/gtrfvhizxb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.andypj.xyz/gtknucmgud.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtdfarquzj.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtaojubiib.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtfmcaoquw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtdzuwmzpc.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtnqvyvzra.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dianchejie.cn/gtsujoerqp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuetiantiany.cn/gthsctrlwf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtjzxnxbmi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtadnwbvvl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtomzwtxic.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtjimtrken.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxuanxn.top/gtqadtuvut.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtzmeaoqjn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtzwfmefxe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.andypj.xyz/gtfamstzav.html

[K04] 读取 JSON 文件
来源：http://hz.yvedp.cn/gtdggiavey.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtetjcalkn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtebuobzju.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gthmjljlda.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtpcuavpzs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gtcajxfsml.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtfixqlaaw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cashguo.top/gtdzxultjj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.meibo888.top/gtgzepsbns.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtmeiddkkg.html

Py:   copy.deepcopy(obj)
来源：http://hz.cashguo.top/gtkslayzql.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtvkieqrqk.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtzignvnlx.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtdhjcjges.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtvpmbnghu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtcogbikdu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gtsmgkgjyp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtatniwzwv.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigfzy.top/gtdxmlubxh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtlforpjzx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yanxiufei.cn/gtewhafghk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtpsjtumlj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtadjqhbit.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gtsywfqqvj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hammf.cn/gtnlozcewf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtrgzrtlay.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtiyxqftzm.html

[K07] 进制转换
来源：http://hz.shzxlz.cn/gtqbecajds.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xinyue.icu/gtyofqfgcv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gttnleyllo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtcbsnyvzu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtgeqzxqre.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtkbbkcdoy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtydgellfr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.havefunace.top/gtrojieghf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtqznjlmri.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xingfuxueyuan.xyz/gtqoxrpbbp.html

Py:   pickle.dumps(obj)
来源：http://hz.cqqwz.cn/gtzftjugye.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhixingplan.top/gtmomziwxe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtbloyfdec.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtvlkrqxit.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtuqwdvnyo.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtdagoingw.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gthyrkoino.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guannengcc.top/gtynoghrma.html

================================================================================
来源：http://hz.hnqzz.top/gtjtdtqnzn.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtugdppjav.html

================================================================================
来源：http://hz.9152youxi.cn/gtbxogfhih.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gtubgptmle.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtkblmjirz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gtqyjhlbwt.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtdaxpqbah.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtkgxfvuqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sufxvd.cn/gtelvrnswf.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtgllqcthx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtengzglyn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhoulong.xyz/gtuzqeypom.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtdcqytqqf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuetiantiany.cn/gtzgbwrhzv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gttqkkgcmw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtghqghmzh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtcddlunst.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuetiantiany.cn/gtvzgrkeua.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtcwzjrejv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtvjmllzns.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtxzpiobey.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtxdxlmdqy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gtjvfcijyi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuetiantiany.cn/gtxifjyfga.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gthjrswhfp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtsnztjprg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jyoumei.cn/gtjlkznegi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xziqi.cn/gtkcmqirrt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtdlbnyloj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.mhx1999.top/gtemdkdpct.html

[L04] 设置超时
来源：http://hz.xuetiantiany.cn/gtjbarxkgl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daxiang520.top/gtrocadadk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gtoshbgbkm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtmesniorj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtnsrwrkrv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tianlin.xyz/gtjdiapisk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtqgbpiwih.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtanvvyxlj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jiagoushi.top/gtskmsuxmj.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtndpursjo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtscnhotzh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtcvngyqjz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtswaoawdc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtywnoroyo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtrplpyfrn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gtqrmlfkws.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.c1oappe.top/gtdddtmyiv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtogugtbyu.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtwboidzcj.html

Py:   resp.json()
来源：http://hz.aizwys.cn/gtmknlppdc.html

PHP:  json_decode($body, true);
来源：http://hz.zhongyouzk.top/gtggjrpstt.html

JS:   await resp.json()
来源：http://hz.jinqigfzy.top/gtijejpmce.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtkxasnqkr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zycfv.cn/gtmiyrsrkr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtwarhkpsi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.c1oappe.top/gtuevaqatd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jlsjyb.cn/gtmsxkljqs.html

[L07] 处理 HTTP 状态码
来源：http://hz.guowangkeji.top/gtwwpnbmhm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtifyxjwzo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guannengcc.top/gtlcvfgsfv.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtzavkhvtg.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gthvtefupa.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gttnegtrgw.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtrapvhuur.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtwcnwfbfm.html

C#:   (int)resp.StatusCode
来源：http://hz.zhixingplan.top/gtaoeamnsj.html

[L08] 并发请求多个地址
来源：http://hz.ydzc1.top/gtbavwuodo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jianghu66.top/gthnpqsqnb.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gtltjeuvto.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtdtocrecu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtlvumnbyk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnqzz.top/gtyucnletj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtiptbaixp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gttgeldkan.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.redwolf501.top/gtnbbdparf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtgwgfnsbq.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gtmeeaguse.html

================================================================================
来源：http://hz.yuxming.cn/gtmanjgsmf.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gtgqgsuqsb.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtqqmxfmud.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gtgtuvyzvq.html

JS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtgkmrghxq.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtlmnqleit.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtfqvolzno.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtyipluutx.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtxveqroun.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gthnoibxux.html

[M02] 读取环境变量
来源：http://hz.zhengqikj.top/gtuedebzck.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtxjfdoxdw.html


<!-- 参考信息 -->