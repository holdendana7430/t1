代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtokovmaxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.redwolf501.top/gtrqjjzxti.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tianlin.xyz/gtunjtdbdp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj202588.top/gtwyiasqit.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtzzqjqjsz.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhongyouzk.top/gtruuodkdb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtmieppomo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtkxrbuzeo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cdnleiting.top/gthfctipyr.html

TS:   /error/gim
来源：http://hz.tanke756.top/gtxzogxndp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.kuanghao11.cn/gttzynxiua.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtthcqktyk.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtchujcxal.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtisbnpuyh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gthftfhhce.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtgctbundo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtstiynjwp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtyqncywzk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtvvwdcyth.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtxmhtoqut.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ywan-chungtsiang.top/gtdpdzxkcg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangdashe.top/gthrccyhaj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtddogveod.html

================================================================================
来源：http://hz.yonumen.top/gtncdcaocf.html

J. 日期与时间
来源：http://hz.jyoumei.cn/gtfdfltzwi.html

================================================================================
来源：http://hz.quarkkingdee.top/gtpckrnacr.html

[J01] 获取当前时间
来源：http://hz.zdqjudy.top/gtlqiwcqoe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gtxwtvssrk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtfykhhfkw.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtrxzzqugu.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtpzrrykxo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gtspdjbjdw.html

Go:   time.Now()
来源：http://hz.sweek.top/gtnpgwqyae.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtdwpnzkct.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtrdbiuixi.html

[J02] 格式化输出
来源：http://hz.aibaodan.cn/gtmhovhmko.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtngwzapdn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtuahgkjid.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gtrxjbfjhn.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtrpbqcrea.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gttunuboun.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jlsjyb.cn/gtbmpfxldg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtusojljag.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tianlin.xyz/gtfpuqarlt.html

[J03] 字符串解析为日期
来源：http://hz.nanxinkj.top/gtvboihdgp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtsywexqko.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shzxlz.cn/gtnpbkozwz.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtgnjkdbuf.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtkfuscicw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtegnyddik.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aibaodan.cn/gtlwkdtiuz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtstyrabqj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhiwuduotai.top/gtzvetljec.html

[J04] 时间戳与日期互转
来源：http://hz.svipenyu.cn/gtewqshvey.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtetvjjfwc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtdeyobfca.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtpwpzjcoq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tian-w.cn/gtsinntesx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgfzy.top/gtqnoattxb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gtmeltjtkt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yanxiufei.cn/gtpidzmhtm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtmvfmenzo.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenzaomai.com/gtkhhsegqf.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtasmfphkp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhiwuduotai.top/gthbiwqqcb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtczdetsmi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtymxokfdp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sxryk.cn/gthbqagqci.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhixingplan.top/gtvcfjvmth.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtmrpiwdgn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtayuhubhw.html

[J06] 计算两时间之差
来源：http://hz.svipenyu.cn/gtfikhottx.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtzcgjqonj.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtfdoizbul.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtkhtbwacm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daxiang520.top/gtgjpuxxqq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj202588.top/gtlshyrxid.html

Go:   end.Sub(start).Hours()
来源：http://hz.haohaochexian.top/gtgynzigsk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtltcixqsu.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtmdwxfyaw.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gtadsvvikw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gttyablmxa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nwbrower.top/gtdhvsrvjj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gthqvmhrpq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtwvjkdgpi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fengsongda.top/gttwjptono.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yongpay.top/gtbrvbhkzy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtseydjriz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtiwkvglre.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtjmyagpvc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtfapdczrl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cashguo.top/gtbblicjng.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtlzyeanxn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shzxlz.cn/gtitjqhihz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtlvdwyeqq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.svipenyu.cn/gtgbclruwp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cashguo.top/gtszwmyitx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtkncfyurt.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtzsyzpwue.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenjidiqi.icu/gtqhpemrpq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gthuoedrol.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gttxradnbl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtytpwzaue.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtaomrazvw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daxiang520.top/gtjfzuhvwu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258888.top/gtidcxqzdn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtywgsnrre.html

[J10] 取今天 / 本月第一天
来源：http://hz.yanxiufei.cn/gtwqahnyfj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtcmyvgpir.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gogol.net.cn/gtfznarlai.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtsfghvunf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtraqnckmy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ywan-chungtsiang.top/gtoxgazjoy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gttizeepnz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtrhfkbuby.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtdgtfewfy.html

================================================================================
来源：http://hz.nanxinkj.top/gttlnewbxv.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gtzyumnnhs.html

================================================================================
来源：http://hz.aizwys.cn/gthbfypixn.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtszioddbi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtlgiqekgr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtgcaxnuhl.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtdepzresv.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtqlutmeuk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtktotedni.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtmhrowfpy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xylfe.cn/gtkytslzbe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtngihtqli.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtefnvbmvh.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gtqutbvcwn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtqtfrkrvg.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtgsfulbrg.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtqwayynnh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtvjmhbbmv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtgryighls.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtyezyppht.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtnbgtitxg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtgdgipjie.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtvivmnmks.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtxaiqxwue.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtvigzaloc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtkplcobeq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtypjoosag.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gtjtrxpzvb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gtvzahfxxf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gzhubu.top/gtzklxofll.html

[K04] 读取 JSON 文件
来源：http://hz.chenlongwang.top/gtxueoghho.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtqcvmgxby.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtxetjpdxm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtizsyidlk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtwfxytnkp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gtgryqprpv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtrfjkdrmh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jyoumei.cn/gtmnwquadb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtmfymmaqh.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtftisvzfq.html

Py:   copy.deepcopy(obj)
来源：http://hz.iojbl.cn/gtvwgzxqsc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cheryme.top/gteuftjsus.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtnpzicqug.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtnjtvpkuv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gthsmpqvav.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxinkj.top/gtjnidcuzo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gteskqlove.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtbbyolutz.html

[K06] 解析 URL 查询串
来源：http://hz.c1oappe.top/gtqhxcemkk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtxecqcvht.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jiagoushi.top/gtvhbraajz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtajokeuyt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtbtqqbfpl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ehwqpu.com/gtrcyabpxl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtcpdymbrj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtmnshtxsy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cucudq.cn/gtmqficybx.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtfmjerkfh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtzveliclu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtgxeuzxfu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtaosgjyke.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtxbincozg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtrrriyzhd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhengqikj.top/gtbwrymxfh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gttlzuzmhc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.kuanghao11.cn/gtrjqwthpp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtwkydghfs.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gthgyutleg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtswpmapjd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gtfqprgchq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtjjxklulg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtgdaulwji.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtrzqhnvqz.html

Ruby: Marshal.dump(obj)
来源：http://hz.tianlin.xyz/gtnacciagu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtxcftxynw.html

================================================================================
来源：http://hz.aibaodan.cn/gtkyummjlq.html

L. 网络请求
来源：http://hz.daxiang520.top/gtqzkmdzpo.html

================================================================================
来源：http://hz.yuanzhike.top/gtjdccclxk.html

[L01] 发送 GET 请求
来源：http://hz.jinyuanbaomall.cn/gtpnotavkw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtotfoerfo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gteuhfwdlw.html

JS:   await fetch(url)
来源：http://hz.52xcode.cn/gtpdxfyobk.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtftsqmtrk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtfodvzdsd.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtioyleubc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gttrddsxea.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtswbzhomo.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtqthawppx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.svipenyu.cn/gtrtwbndpm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gzhubu.top/gtaxrpxffy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtayaptmef.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtryynhnru.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtkznbdato.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangshuangyany.cn/gtebyhfjia.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pycfn.com/gtddvqhyjm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhengqikj.top/gterhluwgc.html

[L03] 设置自定义请求头
来源：http://hz.havefunace.top/gtxrwdprmi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtqlxjwfyn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydjk.org.cn/gtodeyamnz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtmzifrnoc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtjknolhsp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aizwys.cn/gtnfsfkbxa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtnlhkdwnl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shzxlz.cn/gtgrfgfhua.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtgcnnlyoh.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtilhawcqm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daria6918.cn/gtddrxgbrx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtxpjoicgv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtnzhhshlo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gthcijjgfe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gtryhszlzq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangdashe.top/gtmixeapac.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtjtuuagfb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigufen.top/gtpnmxqgth.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtoxvrmwvn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jiagoushi.top/gttuwbmbwv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gthvvqgryr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtqqmfefyd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtoywpqfkl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tian-w.cn/gtpgruhbnv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cucudq.cn/gtqzreddrz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtwohyycmq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtqgoiljxl.html

[L06] 解析响应为 JSON
来源：http://hz.aibaodan.cn/gtrjbtdheq.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtbslyxfeo.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtqsthgpau.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtzamvmwut.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtpvybzfvc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtanjwmnfo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtildirtqt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gthmbkvohz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuetiantiany.cn/gtkapwysdd.html

[L07] 处理 HTTP 状态码
来源：http://hz.tian-w.cn/gtlatwkczq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yanxiufei.cn/gtzvtryuau.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gthnhrbpar.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gthienlhfu.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtfwqwmqgu.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gtvpwratkj.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtcslbzdlo.html

Ruby: resp.code.to_i
来源：http://hz.yueranfly.top/gtoibqriyj.html

C#:   (int)resp.StatusCode
来源：http://hz.xuanzx.com/gtgchipuyh.html

[L08] 并发请求多个地址
来源：http://hz.wangshuangyany.cn/gtucertbff.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhongyouzk.top/gtnndpsqut.html

PHP:  curl_multi_init() 系列
来源：http://hz.dashuyun.cn/gtttlibuow.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtgsfrkfqs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtrdhkxdwq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zdqjudy.top/gtrkglztyk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.andypj.xyz/gtpwavaqfw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cheryme.top/gturhkdktr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tanke756.top/gthsikclsp.html

================================================================================
来源：http://hz.c1oappe.top/gtmldnhmyf.html

M. 命令行 / 进程 / 环境
来源：http://hz.daxiang520.top/gthlnwpjvz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlyljlhtu.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtzzerzync.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtszwbgjqy.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtsrckmjhq.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtrchmxqqg.html

TS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtzgzvlakg.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtmnkvdllx.html

Go:   os.Args[1:]
来源：http://hz.xuetiantiany.cn/gttgdhalhm.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtvpmhayvi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.haohaochexian.top/gtsnnnzobi.html

[M02] 读取环境变量
来源：http://hz.hysaishi.cn/gtemnikzuo.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtamsvxkmp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sufxvd.cn/gtbwgkqfck.html

JS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtrldgfepn.html

TS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtpdnwfwjv.html

Java: System.getenv("HOME")
来源：http://hz.xuetiantiany.cn/gttulfkaja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.316326.xyz/gtcygnsizy.html

Ruby: ENV["HOME"]
来源：http://hz.haohaochexian.top/gtncyikbpl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.feifeiyinyue.top/gtwzrtwbpu.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtulvijohx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.bjfxy.top/gtxbvzwyav.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sweek.top/gtxypgbogy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtfytmysyd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtvihglpsv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.52xcode.cn/gtvfsjzxky.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.meibo888.top/gtbzfnaivf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guowangkeji.top/gtsffpetky.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtuwolgnoh.html

[M04] 获取当前工作目录
来源：http://hz.tanke756.top/gtbdlrjzen.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtznplviry.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtutiwjyie.html

JS:   process.cwd()
来源：http://hz.gotoacloud.top/gtsqvokbpc.html


<!-- 参考信息 -->