代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtkfpneays.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtcguozmit.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zycfv.cn/gtojxlazlu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hfpthk.cn/gtxrsetnki.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gtemycwdej.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtnvbbjqmd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtrgpkkejl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cheryme.top/gtvfzmpmdw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtapkwklsj.html

TS:   /error/gim
来源：http://hz.52xcode.cn/gtgygwwrsx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zycfv.cn/gteutdlddh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.316326.xyz/gtpovklrbo.html

Ruby: s.scan(/error/i)
来源：http://hz.zhiwuduotai.top/gtkpkexizu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.0kj1m.cn/gtlgtvwfov.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtvctcvmwv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinqigufen.top/gtwxixxmgs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtxzfaejza.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtmwerjnvk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtcrkpyjup.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtfbjdhgha.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxinkj.top/gtpcandcoc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhoulong.xyz/gtxkjajksm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtwhhwygax.html

================================================================================
来源：http://hz.yj202588.top/gtwlzclsaq.html

J. 日期与时间
来源：http://hz.zhiwuduotai.top/gtvkhwjmrm.html

================================================================================
来源：http://hz.jianghu66.top/gtuumuaycz.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtrobctjkk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtwmwtkibz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtvqnyukna.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gttptgtyen.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtkpfsqghl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sxryk.cn/gtgmjudais.html

Go:   time.Now()
来源：http://hz.yvedp.cn/gtohtebnsf.html

Ruby: Time.now
来源：http://hz.316326.xyz/gtzpetexbj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hammf.cn/gthdawwdsr.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gttbziuhbs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gteynxiygf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtfawykjti.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtxkqahsca.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtutkmbfef.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtbipvypli.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hysaishi.cn/gtibfshbns.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtbsowlmrb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtiwsjnhxd.html

[J03] 字符串解析为日期
来源：http://hz.hongshengwenyu.top/gtcoobmpsq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangdashe.top/gtkeucqoss.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtpwpndggy.html

JS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gttaraqquh.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtrccltrlg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtpmtsmshb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtlzxmkryo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydjk.org.cn/gtkivyllmr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhoulong.xyz/gtmzigfjgo.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtabkptmse.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jiagoushi.top/gtptpyuync.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.redwolf501.top/gtoxgvxlhs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jiagoushi.top/gtwjerovhf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtdlhjceup.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtzoeypvwu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gtoztbjmwt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtaxmdsbpn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtztgtttpz.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gtifkfumoc.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gttpnzqdxw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtsibwawdv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtoktbrfbz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtimdpnpcj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtsmnregkt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtdlmbzran.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtcelttpci.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gthpgirxpr.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtrqoqqlqq.html

Py:   (end - start).total_seconds()
来源：http://hz.mhx1999.top/gtldhasgml.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gtwijilfqk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtecigqtzj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtplfzreob.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtiqxpbxwr.html

Go:   end.Sub(start).Hours()
来源：http://hz.sweek.top/gtnmxgggka.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtlfwtygoi.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtbchbmkxc.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtzyyyarqa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtzgpuiaqm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtdxpusjsd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtenwfskcb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtlzrrymbz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.vqdsnc.cn/gtssdomzlu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sufxvd.cn/gtvfihfhcd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtooabnyto.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtqenwrxto.html

[J08] 提取年月日与星期
来源：http://hz.pycfn.com/gtsadacdtf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtegeitllx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnxiangtu.top/gtckvfikxx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fengsongda.top/gtiescduso.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtnshrdmxy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhijiandao.cn/gtnjehpqhi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtwtapxzhz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenlongwang.top/gtfphysysp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gtulpvbeze.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtjlzwklpq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtdvxijrih.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtnoawggmi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtataaqppv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtoqidosox.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gthliveaeh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtuubyyqec.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtiyxvwzyo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnxiangtu.top/gtypbscgxx.html

[J10] 取今天 / 本月第一天
来源：http://hz.pengpengdd.cyou/gtjcbnwsxg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtphecfrdi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.52xcode.cn/gtlnrystkr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtlcqfacpg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtgxsoimbu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtpzikulpa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtpspmrkfd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.iojbl.cn/gtcfzmpqzq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtddhkqkjo.html

================================================================================
来源：http://hz.jiagoushi.top/gthqmtwwbf.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gtnxqoranr.html

================================================================================
来源：http://hz.52xcode.cn/gtpuhumnoc.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtwpsycems.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtouzzahep.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gttdihzwjb.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtflekndaf.html

TS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gthrylsext.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yanxiufei.cn/gtgrrscsvq.html

Go:   json.Marshal(obj)
来源：http://hz.aibaodan.cn/gtrnadpqwo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gthahgfyxr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtcsyjpbmj.html

[K02] JSON 字符串转对象
来源：http://hz.shuidangran.top/gtbvmjjqry.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtydysyzug.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guowangkeji.top/gtuouhadtv.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtixwldoka.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtrallquxc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtqzbipbpc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtwhetdehr.html

Ruby: JSON.parse(s)
来源：http://hz.0kj1m.cn/gtipepnfkg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gttvsvzxgq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tianlin.xyz/gtnbxklhib.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gticfmmvzm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtwfqtlggl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtffeuhkus.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtoulujphx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtgyeybhtu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtlwvfcxyi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yonumen.top/gthwvpcuqj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxinkj.top/gttxnowjlg.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtkicqefps.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.feifeiyinyue.top/gtfoitcfca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtjrqdhtpa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtbuutektn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtgzvjjldb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhoulong.xyz/gtcyiutkzv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtvstyogoe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtpqnddsmo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nwbrower.top/gtqvafadka.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtjsvjmfem.html

Py:   copy.deepcopy(obj)
来源：http://hz.ywan-chungtsiang.top/gtmcxigyrg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.9152youxi.cn/gtfrjebhxf.html

JS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtruuoxmuy.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtrfsotjmm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.meibo888.top/gtfdprscif.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtfdtqgwhd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtzrftvrlh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sweek.top/gttemyvvgq.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtibxuygxl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sysykeji.top/gtrxbxsepu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtytqpxjzp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtfpppuskh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtdmdswhib.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gtqokkvqzu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtzmijgywn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtafwjydby.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gtxqgozmmx.html

[K07] 进制转换
来源：http://hz.xuetiantiany.cn/gtiofxjnjn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gotoacloud.top/gtqpfwxouz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ivvv.top/gtupdkexmm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtudvmdpgi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtagyhbmwj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gthlvyurmq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cdnleiting.top/gtekgjdrvl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinyuanbaomall.cn/gtfhkkxlsw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xinyue.icu/gtmhuadxsu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.vqdsnc.cn/gtifmmrxyu.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtjstldjxd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.feifeiyinyue.top/gtvjksqlqe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtyfsjrzki.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtfxqvvqow.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gthcdwuwxq.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gtqxdtohzn.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtntidvqlw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnqzz.top/gtlacuodqw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtzcwgimcj.html

L. 网络请求
来源：http://hz.cashguo.top/gtdjpqewtc.html

================================================================================
来源：http://hz.sweek.top/gteewacafg.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gtydfrzfge.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtbizczwyl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtcbyziruk.html

JS:   await fetch(url)
来源：http://hz.daxiang520.top/gtxnkzqqvg.html

TS:   await fetch(url)
来源：http://hz.pycfn.com/gtdqzkyrxd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.meibo888.top/gtnjcbvtnr.html

Go:   resp, err := http.Get(url)
来源：http://hz.daxiang520.top/gtcqttfywg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtozztvnom.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gtpgbgxsvs.html

[L02] 发送 POST JSON
来源：http://hz.smart0.xyz/gtzablpwop.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtytjwctxd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtkioziatd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtbbfzmvle.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtomogsedo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hfpthk.cn/gtzjfmymfl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtpfqhnciw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtexapbwss.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj202588.top/gthnfyyilj.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtlcdwmfyb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtoawqansa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gzhubu.top/gtufyjarrd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtvxpzxlcc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtuoauxnin.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shangyingyoupin.top/gtuzfaucox.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangdashe.top/gtqvedebox.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gtbovnwtky.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pengpengdd.cyou/gtnndlsptw.html

[L04] 设置超时
来源：http://hz.ehwqpu.com/gtmgooseed.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtxqdzdrof.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gtrmrfbnfd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtptomoute.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gthvzrszzf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtxrmyopgc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xziqi.cn/gtehzikzhr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zdqjudy.top/gtbhqgjuxy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtbavixygi.html

[L05] 上传文件（multipart）
来源：http://hz.snrcjt.cn/gtmmkwimgw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtwpzdofez.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtjtzmcqho.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gttrmjqbzv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtzxygpoyu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ehwqpu.com/gtsnybqrdq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jlsjyb.cn/gtwwngkttj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jianghu66.top/gtikbbzilw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtvlmvabxu.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gttkyfzkkn.html

Py:   resp.json()
来源：http://hz.sufxvd.cn/gtcfnfgrjj.html

PHP:  json_decode($body, true);
来源：http://hz.ywan-chungtsiang.top/gtgiuzgpgy.html

JS:   await resp.json()
来源：http://hz.tianlin.xyz/gtjasxxezj.html

TS:   await resp.json()
来源：http://hz.ppjwa.cn/gtzubfbusj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtkiffjurd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jiagoushi.top/gtxvprdcys.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtdrrokazf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cashguo.top/gtagklddoj.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtrlwdjlbu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258.top/gtjlraqbys.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtaihryuub.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtlebayxxr.html

TS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtmmattrbc.html

Java: resp.statusCode()
来源：http://hz.chenzaomai.com/gtqgvkgdpx.html

Go:   resp.StatusCode
来源：http://hz.fzhhl.top/gtwnrvbfvj.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gtilefcrof.html

C#:   (int)resp.StatusCode
来源：http://hz.guowangkeji.top/gtodritqce.html

[L08] 并发请求多个地址
来源：http://hz.hnqzz.top/gtmtylyihk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtseqcatcv.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtjjpzuhrt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtyytjcqzu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtthbsihze.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cdnleiting.top/gtbangjljy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gtzxscnkzv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.kuanghao11.cn/gtlcmzccvb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtbalycqlh.html

================================================================================
来源：http://hz.hammf.cn/gtznsxfhsp.html

M. 命令行 / 进程 / 环境
来源：http://hz.svipenyu.cn/gtdpxojzzj.html

================================================================================
来源：http://hz.shzxlz.cn/gtwruqpqjf.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtffvhhnwz.html

Py:   sys.argv[1:]
来源：http://hz.fzhhl.top/gtwxvqseyv.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtvuqhskfq.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtbrzpfqcs.html

TS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtyqrhotww.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gteyiizyjh.html

Go:   os.Args[1:]
来源：http://hz.hnxiangtu.top/gttmcmyakm.html

Ruby: ARGV
来源：http://hz.yj20258.top/gtrqdaiycs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.kuanghao11.cn/gtzxlqwvip.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gttzmdnexi.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtokigzrln.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yueranfly.top/gtgedwdpsx.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gtvhdwsqyc.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtughhmsfe.html

Java: System.getenv("HOME")
来源：http://hz.chenzaomai.com/gtaploiind.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258888.top/gtliceiegc.html

Ruby: ENV["HOME"]
来源：http://hz.xinyue.icu/gtqaliifwd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhiwuduotai.top/gtfvmdvsrg.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtnzskjjok.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.smart0.xyz/gtwabhecbc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtvsfmkxpk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtvbjimbok.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gtqvsuiufx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtbyguwfzh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.quarkkingdee.top/gtaerojvak.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtgpwptbce.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtcclpyvwj.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtehuvtoxs.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtaaiwvskw.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtxoenmemr.html

JS:   process.cwd()
来源：http://hz.316326.xyz/gtpaganjxu.html


<!-- 参考信息 -->