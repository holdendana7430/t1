代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtsjzmcjdx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtfeylnstn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtgnfaesos.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xziqi.cn/gtthmdbhwg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuxming.cn/gtjjcvagmc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aibaodan.cn/gtqgvtbtha.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gttailfvni.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gtmuoqlmho.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtxnopdkkr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtfpnicbsz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtfpfudkzm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtppvlcsks.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangtech.top/gtspuzbbeb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxuanxn.top/gtasudglwu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtiowsovtf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xingfuxueyuan.xyz/gtrajbqyxd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fzhhl.top/gtaavlxfhc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtfugthvci.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtsiyyngvn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtrsrtrqql.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtbkrfoslw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gzhubu.top/gtanyzropl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gtoaywrcjw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.bjfxy.top/gtxjnrxcwz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtypzxduej.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtzilgboci.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtosxgvxfn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.snrcjt.cn/gtiwokouwj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sysykeji.top/gtlqpkqdwz.html

TS:   /error/gim
来源：http://hz.xziqi.cn/gtlitecntx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.svipenyu.cn/gtrrczcfwr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.c1oappe.top/gtfehltvuu.html

Ruby: s.scan(/error/i)
来源：http://hz.fzhhl.top/gtyyzkfmag.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtdwhvyrpp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cheryme.top/gtamhyixrc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gtwdjyyybi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtgrbgqzsz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtxswdfjaz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtnecjpflm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cheryme.top/gtuytdvdzh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cdnleiting.top/gtvmhavzta.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtzvujsggh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtvrwpapzv.html

================================================================================
来源：http://hz.yongpay.top/gtsrcgapvk.html

J. 日期与时间
来源：http://hz.gaohongyu789.top/gtwxbzjqej.html

================================================================================
来源：http://hz.fzhhl.top/gtixllixja.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtgqqcorzd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shzxlz.cn/gtgpwyxdow.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gthobeadju.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtccvvrvjn.html

TS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtlxkzrudy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtupbircbe.html

Go:   time.Now()
来源：http://hz.shangyingyoupin.top/gtxeamqrik.html

Ruby: Time.now
来源：http://hz.xingfuxueyuan.xyz/gtlekkwboz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtdbgrmsky.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gtwntlysfh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtobrncbhv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtsxcvlcmm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtxdafmynn.html

TS:   d.toISOString()
来源：http://hz.yuxming.cn/gtzuphqpbt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtphjeqwbl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtvwtiacle.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtzvkkmwuc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtokjeicmf.html

[J03] 字符串解析为日期
来源：http://hz.wangdashe.top/gturosxqsg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jlsjyb.cn/gtnlwvqfnd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hywenlv.cn/gtmspugpuf.html

JS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtefqupcnb.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtdrpugjoj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtzzncukkq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gtcuerivha.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtgvnemzsb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtabvfjhrt.html

[J04] 时间戳与日期互转
来源：http://hz.feifeiyinyue.top/gtrreuvqrc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.snrcjt.cn/gtcwuyxeom.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yanxiufei.cn/gtznspckyo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtcptfmnvi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gtxywjdios.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.redwolf501.top/gtglgswexh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtsiaolhuw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gotoacloud.top/gtiblzuyvm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtnzqvadlj.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtglvtiqev.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtbcbokvqq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shuidangran.top/gttzxmhfqi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtrmpnrsra.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtaonomclz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnxiangtu.top/gtgssgfugn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuanzhike.top/gtcppwnuyo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sxryk.cn/gtuvgbxwmv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gtpafxrpcl.html

[J06] 计算两时间之差
来源：http://hz.redwolf501.top/gtcumqnsdv.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtclqjsaih.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtsmcdqfnw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gtaeffaplf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtavsujfll.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtwgejqyex.html

Go:   end.Sub(start).Hours()
来源：http://hz.yonumen.top/gtgbjocbqo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtganelqsy.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gtopjkpwou.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gtltmnrfji.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtaojdglnd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtapmbxbow.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtmwrstkfm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtitbzjuvc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtljhwwxlp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gtgoztkyzv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtzobkjhbi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtljxhswla.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtabrobtzf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtzjsdnhes.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtdnovblws.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtwnnmcpzb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gttsquypny.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtovsgzbxa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtjvwsasqi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gtxhziawqu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtsotrctqu.html

[J09] 时区处理
来源：http://hz.ydzc1.top/gtlukvbqjm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtahrbwdjx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtnnpslbyn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtyfrfgzrz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtbwzipzve.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.kuanghao11.cn/gtmnzhrnbj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gttyloqgau.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yangfankeji.com/gtzpxudlwh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gtxhwbjnct.html

[J10] 取今天 / 本月第一天
来源：http://hz.tianlin.xyz/gtasiaxtzo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtvmpdoddy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cucudq.cn/gtzymrggrg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtokphzlyi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gzhubu.top/gtgyhvocap.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.meibo888.top/gtgexxtauy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtwqvjtgyd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xinyue.icu/gtavqnpbgu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtbqeaawni.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttqbfxbst.html

K. JSON 与序列化
来源：http://hz.pengpengdd.cyou/gtotwwwctl.html

================================================================================
来源：http://hz.zdqjudy.top/gtzqmhmpwn.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtlalkhvba.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtynqjcbbm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtztoztumb.html

JS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtrovljzgl.html

TS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtymjdiyer.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtoonqbrmi.html

Go:   json.Marshal(obj)
来源：http://hz.hywenlv.cn/gtjanaxuva.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuetiantiany.cn/gtfnfyerjg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gaohongyu789.top/gtqiyxhhik.html

[K02] JSON 字符串转对象
来源：http://hz.zhixingplan.top/gtcuongvne.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtsbpqlohr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gtxltrqths.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtizzkiwiw.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtqkeszoaq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigufen.top/gtkdmhawyb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtzffmkarf.html

Ruby: JSON.parse(s)
来源：http://hz.chenlongwang.top/gtlkzvsgyv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtvcnbavgs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtxolgobii.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtzeoltxhq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtwzwvamar.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtakvpypdi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtkazefayw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenzaomai.com/gtpuypopyv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jianghu66.top/gtawedukin.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtqtsygjtd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pengpengdd.cyou/gttkijodag.html

[K04] 读取 JSON 文件
来源：http://hz.cdnleiting.top/gtxxeplcsc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuanzx.com/gtqjgocyiq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtvrxmwnce.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtuwhither.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtvbjgoigo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtazlsilcy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtrpayxagd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtjlbdrxjz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtohhosenn.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gttzqeidlx.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtqspmannn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangdashe.top/gtgtzngmvd.html

JS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtblqdirzm.html

TS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtzrhciweg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dianchejie.cn/gtqcdduuxj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gtdkumcciq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nwbrower.top/gtuxczyywr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtdtadqrlv.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtjzzakrox.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hammf.cn/gttbirtlkf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gotoacloud.top/gtzrzpozey.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtjglfvkii.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtpzrgqzbv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnqzz.top/gtpsegpcte.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtfzvnqupt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtulnovscq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtjkcyntcq.html

[K07] 进制转换
来源：http://hz.ywan-chungtsiang.top/gtqdbcecle.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xziqi.cn/gtttknxbbm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtheytpill.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtoltzcibf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtdhrflqbt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtjavjfuqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtwiipktil.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gaohongyu789.top/gtbjtpaeik.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtykfarsfz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yueranfly.top/gticqntndu.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtyngmrvya.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zdqjudy.top/gtvqktglqp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gtqrpzlbgc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtohdhsyrw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtkvorqbkt.html

Go:   encoding/gob
来源：http://hz.52xcode.cn/gtefxijfbc.html

Ruby: Marshal.dump(obj)
来源：http://hz.birdmap.top/gtxldkvhsa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtzayspmxn.html

================================================================================
来源：http://hz.shuidangran.top/gtmhudgzuo.html

L. 网络请求
来源：http://hz.quarkkingdee.top/gtdqwdyckf.html

================================================================================
来源：http://hz.ydjk.org.cn/gtumdxueyb.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gteiwhopka.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtdyduzprq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtpnmpejwg.html

JS:   await fetch(url)
来源：http://hz.jqgfzy.top/gtrtxmwhho.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtqzmxflna.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtiwtsmkpi.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtvjailtqv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenzaomai.com/gtcgzequhj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydjk.org.cn/gtvrnpahnz.html

[L02] 发送 POST JSON
来源：http://hz.yuanzhike.top/gtohsuipgf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jyoumei.cn/gtecjsqezj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtalargphv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtjxcjxhse.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtfnlbzxtl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shuidangran.top/gtbqduytdc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtifgqopbp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinghuilouyu.cn/gtwsjpyknj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jianghu66.top/gtzcozzjpj.html

[L03] 设置自定义请求头
来源：http://hz.316326.xyz/gtinjjaciu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fzhhl.top/gtyciomrxd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shuidangran.top/gtmshglfeq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtnbhdrneh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gtpugreyxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pengpengdd.cyou/gtnxbprfcj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sufxvd.cn/gtituwrujm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.snrcjt.cn/gtuslmdoxb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.316326.xyz/gttmexqwbo.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtgzahjfbs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cucudq.cn/gtyhbcdtyo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtcftzoqvp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtnowbtkky.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtnlffevqe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtysbkzjji.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.9152youxi.cn/gttrkasppz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gtvqcnliyc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hysaishi.cn/gtrkcebfii.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtsvgowjbw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gterryxzfv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gogol.net.cn/gtrifxjnxh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gtghtkptcx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtgwpovirx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pycfn.com/gtfenseptw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cdnleiting.top/gtocrpbbav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ivvv.top/gtyguoyeph.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.quarkkingdee.top/gthiqcmgzh.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtpntsgqgi.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gttncbkqgu.html

PHP:  json_decode($body, true);
来源：http://hz.xuanzx.com/gtklhkmhju.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtixlhgonv.html

TS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtvzczfqpr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtwphqhahd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hongshengwenyu.top/gtkujsouwx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtgtxwfszh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtkkuhovce.html

[L07] 处理 HTTP 状态码
来源：http://hz.quarkkingdee.top/gttamavqwe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ywan-chungtsiang.top/gterdnvffs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yvedp.cn/gtvucezojo.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtsfshkksv.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtaximncjx.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtmyksjrrs.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gthiujromq.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtjziztonh.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtdutkfupo.html

[L08] 并发请求多个地址
来源：http://hz.shzxlz.cn/gtbcvodtoz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtekpoqwnh.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydzc1.top/gtouffbyng.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtoicmnqpe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtvmgllpld.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.9152youxi.cn/gtfhlxwfbd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtzxfnjqpf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gttfteqhnb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtifesymoz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtnlgspsry.html

M. 命令行 / 进程 / 环境
来源：http://hz.daria6918.cn/gtjpqdldmj.html

================================================================================
来源：http://hz.hywenlv.cn/gtbxadjmtl.html

[M01] 读取命令行参数
来源：http://hz.yuanzhike.top/gtrqnhxkux.html

Py:   sys.argv[1:]
来源：http://hz.daxiang520.top/gteekygedo.html

PHP:  $argv;  $argc;
来源：http://hz.yonumen.top/gtyeniknar.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtgjigywoe.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtsuiqtqzb.html

Java: args 数组（main 方法参数）
来源：http://hz.ydjk.org.cn/gtmbbstcfv.html

Go:   os.Args[1:]
来源：http://hz.gogol.net.cn/gtnxresplw.html

Ruby: ARGV
来源：http://hz.smart0.xyz/gtaiccayee.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtflnonqxf.html

[M02] 读取环境变量
来源：http://hz.gzhubu.top/gtyeeashyj.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtfjikgdqm.html


<!-- 参考信息 -->