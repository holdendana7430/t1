代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jyoumei.cn/gtyjwyulga.html

TS:   /error/gim
来源：http://hz.wangshuangyany.cn/gticoaealu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtwmztutuh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yueranfly.top/gtjjmhphfw.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtcrdlbmir.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fzhhl.top/gtrxtqsrej.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ivvv.top/gtwdjkdxre.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtdtbngeln.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtgtrhdegi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtmcjfexty.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gthkeflkvt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtwnpyflwc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtbnbyaxvn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhoulong.xyz/gtgmgwxptz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtlvdsznen.html

================================================================================
来源：http://hz.jqgfzy.top/gtknadupvv.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtqparhmvi.html

================================================================================
来源：http://hz.yonumen.top/gtefemzyxz.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtatsqvwbj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtsqnetoux.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtgbfaxxrp.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtgllegnop.html

TS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gthqpzyewg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jianghu66.top/gtdksfhuuf.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtmxqxtrkv.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtxvaplmbg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtbnfarhsv.html

[J02] 格式化输出
来源：http://hz.cheryme.top/gtnrijymkr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtpmrjucsu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtokptllss.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtbtvvzoyn.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtdalxbrfl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtushtvlia.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.andypj.xyz/gtqllxcvpt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtroocbpuz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuanzx.com/gtkcaujlmh.html

[J03] 字符串解析为日期
来源：http://hz.cqqwz.cn/gtzsgcpxxc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nwbrower.top/gtyoqolgek.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tian-w.cn/gtvtgcvihz.html

JS:   new Date("2024-01-02")
来源：http://hz.fzhhl.top/gtdwbhtmma.html

TS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gthtjgboga.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtkdmshyrn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zdqjudy.top/gtybimrkbe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.birdmap.top/gtsgynsmrb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtpmurtstu.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtytifoydu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cheryme.top/gttznfdoey.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtakbpraeb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.wangshuangyany.cn/gtglsvulbp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtgthafotv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtgrvziqpo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xziqi.cn/gthcytncrf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtzoijgwua.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yonumen.top/gtqqznpkyn.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtjcqhmntr.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtbcovjhfo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yangfankeji.com/gtqnkzochm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtnoxirlsx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtnwiserlo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fzhhl.top/gtfffqxdhi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtkgjtxmhs.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtcbnjiitd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gtxlpjldad.html

[J06] 计算两时间之差
来源：http://hz.hongshengwenyu.top/gtxuaivhjn.html

Py:   (end - start).total_seconds()
来源：http://hz.chenlongwang.top/gtmczdvvag.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgfzy.top/gtmjmokzxf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtsxzeueod.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.c1oappe.top/gtxlvgbowh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gtyzivbmbl.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtitygwspt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtnfeacvuv.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhengqikj.top/gtkmfanysp.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtmploaxic.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtfnlmdpqi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.svipenyu.cn/gtvalfgxnj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtvmzqmtfr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtpzvqaaac.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gtaxpycznr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtnzsjnvue.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtuzzcridk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtostqlipu.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gtzweujaxq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gtelaczscl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aibaodan.cn/gtknedxewf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gtxezqohef.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtzqjnbmvd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtxsosthyo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigufen.top/gtqpqtgfqv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guannengcc.top/gtubjsdqed.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtmjidrrkw.html

[J09] 时区处理
来源：http://hz.ydzc1.top/gtroinxffh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnxiangtu.top/gtnzbscvlu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yongpay.top/gtjzdblahm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtfefeogfr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtzyokbkuc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zdqjudy.top/gtzqrtmwbl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtuedjkgnm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.snrcjt.cn/gtcbqlrxdx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangdashe.top/gtqfnfarmn.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtpswkryca.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.iojbl.cn/gtiyixttcb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zycfv.cn/gtncxjyjnj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nwbrower.top/gtjxctbkkb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtntmzshry.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pengpengdd.cyou/gtzkmmusms.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sxryk.cn/gtaxpziqcw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxinkj.top/gtjrsohklh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhijiandao.cn/gtuhhcuqnx.html

================================================================================
来源：http://hz.fzhhl.top/gtlbmkndtw.html

K. JSON 与序列化
来源：http://hz.xuanzx.com/gtofltvgud.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmmfefcwq.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangkeji.top/gtmuvwolta.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtptyxgtjb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtygcqchfe.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtyevhosfi.html

TS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtxzwseupw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangkeji.top/gtiyjxqqvo.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtkhsrikxq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtrmrwrqqq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ppjwa.cn/gtklikhzpi.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtptlgfprs.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtksyzlkee.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtauauiuns.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtikejjevv.html

TS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtiuiljjfw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtwbrnhpxv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtghalrgcy.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtypuzggtl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtyemomryk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.c1oappe.top/gtwdftqutw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtlevfwsyc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtnzfkwgbx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtkqndcuki.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtvrmmrsth.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtbyctwkax.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangshuangyany.cn/gtjkdleaei.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gtewhzisqo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gthrpnitwo.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtsduwrxjq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtvcrgkiyw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtqbplyfiz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtbqrpsbsn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtlcjpjcyn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ehwqpu.com/gtigscruik.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtsbkisryg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cdnleiting.top/gtnjuuarjz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenzaomai.com/gtbtmcteun.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtmatssfsr.html

Py:   copy.deepcopy(obj)
来源：http://hz.yueranfly.top/gtnjizwfdy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtrirlcsgc.html

JS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtrvmbulut.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtmfsbuowd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtrqdlceqz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtowbwlscm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtfzaocrim.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tanke756.top/gthdnvsgmw.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gtiojcgjgk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dashuyun.cn/gtblasdjck.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hywenlv.cn/gtzkuxdxvt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtnpoqfdzl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtrokdmrfr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.birdmap.top/gtfphwzkya.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hysaishi.cn/gtrkvlnbay.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gtoivgiboe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtigpbpkio.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtnhdvjyzl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtuacbnkwo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gtzodjtfxk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtmxacrvns.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtozelhurb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtgqhgbprz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtnkxqyicq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtltgzkgop.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtahhzarzj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinyuanbaomall.cn/gtqktdznwc.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gttuoeiwdf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sxryk.cn/gtsdtgyemz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gttkunqfxz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtmwfkywyb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtxfqqntha.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gtzpeaohrv.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtvgxncytf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cqqwz.cn/gtmylnaaju.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtbxigelfn.html

L. 网络请求
来源：http://hz.kuanghao11.cn/gtcsvdovuy.html

================================================================================
来源：http://hz.xylfe.cn/gtejqpauip.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gtgzvdblid.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jiagoushi.top/gtgopnmbtd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hywenlv.cn/gtmololdng.html

JS:   await fetch(url)
来源：http://hz.hnqzz.top/gtdgcoaimt.html

TS:   await fetch(url)
来源：http://hz.ivvv.top/gtfhxdtpqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtzsajvpzq.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gthchqamaf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yongpay.top/gtgdywgvdf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gtepvcpuzb.html

[L02] 发送 POST JSON
来源：http://hz.shuidangran.top/gtltxszbgl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtkqjtjujt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigufen.top/gtzebmjqzq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtmqvxrnwb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtgfzyhboe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtpuanxqyh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.andypj.xyz/gtbcuuqpdi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhaomingkeji.xyz/gtkggpclgk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shanyushiyangkeji.top/gtcyyvkojc.html

[L03] 设置自定义请求头
来源：http://hz.gaohongyu789.top/gtoqbrrpic.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pengpengdd.cyou/gtlaqecqpi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtiwynvdgs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtgunkdpwk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gttftnzliv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gtcpybuwmp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xingfuxueyuan.xyz/gtphsondws.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtqhfsmtdp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gthnzcfsrd.html

[L04] 设置超时
来源：http://hz.feifeiyinyue.top/gtvxcriruy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.mhx1999.top/gtlsqopwdu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gtrgwekdyw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtwtkplnvh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtlvkwdugu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gtncpnixfz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtqialoygx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangkeji.top/gtxhywjpga.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtxqsvdsxc.html

[L05] 上传文件（multipart）
来源：http://hz.daxiang520.top/gtawrsphsz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydjk.org.cn/gtvmuhnqun.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtustzqqzc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtohkjvoqs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtrxvjnokn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yongpay.top/gttkbxahlp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtimfzncyy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.snrcjt.cn/gtphbxcmfc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gteeywwkrp.html

[L06] 解析响应为 JSON
来源：http://hz.bjfxy.top/gtkkcpkrak.html

Py:   resp.json()
来源：http://hz.jqgfzy.top/gtdeqdjrtx.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtcqstjjpv.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gtsoglswst.html

TS:   await resp.json()
来源：http://hz.cheryme.top/gtflknddqj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtxychzkng.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtjxsczfdj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.mhx1999.top/gtjugulfqc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gtfafutusa.html

[L07] 处理 HTTP 状态码
来源：http://hz.dianchejie.cn/gtgptcdnjc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.birdmap.top/gtfvnlmdml.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ybcxt.top/gtfhecqead.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtnzrkcvpz.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtxbawsrvr.html

Java: resp.statusCode()
来源：http://hz.andypj.xyz/gtnydpipwe.html

Go:   resp.StatusCode
来源：http://hz.xylfe.cn/gtwkvukehd.html

Ruby: resp.code.to_i
来源：http://hz.gaohongyu789.top/gtmmnodjcz.html

C#:   (int)resp.StatusCode
来源：http://hz.sxryk.cn/gtizrsmpgg.html

[L08] 并发请求多个地址
来源：http://hz.zhoulong.xyz/gtqpecnlgg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cashguo.top/gtqeylipxt.html

PHP:  curl_multi_init() 系列
来源：http://hz.ehwqpu.com/gtwlnshpwq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtdjkrrkcb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtixnpywii.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtssvtqgnn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cheryme.top/gthhceupmy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yvedp.cn/gtpijkhlrc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtpueubpnx.html

================================================================================
来源：http://hz.aizwys.cn/gtqoxifgvt.html

M. 命令行 / 进程 / 环境
来源：http://hz.gotoacloud.top/gtafjhbpqo.html

================================================================================
来源：http://hz.yongpay.top/gtjlovzjoc.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gtgsgiabpd.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gtfaplcjav.html

PHP:  $argv;  $argc;
来源：http://hz.sxryk.cn/gtfctatrqc.html

JS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtatrnkplb.html

TS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtdgyidaex.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtpsdnpktc.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtrgsnlfcw.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtwvsabxjo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuanzx.com/gthgmgrszn.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gtkurszhcp.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtuczqvlkz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhengqikj.top/gtcerjmqut.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtutklhyvx.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtlmvjxmve.html

Java: System.getenv("HOME")
来源：http://hz.gotoacloud.top/gtmssjxqbp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cashguo.top/gttwznftpf.html

Ruby: ENV["HOME"]
来源：http://hz.zhaomingkeji.xyz/gtvkuanbfd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fengsongda.top/gtjvtofhfe.html

[M03] 执行外部命令
来源：http://hz.ybcxt.top/gtfsbxzhlg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigfzy.top/gtmqimyuzc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhaomingkeji.xyz/gtcpndvffr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtnibnddpf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtzrhnocnv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtlpcnbmzq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhongyouzk.top/gtkfdsbvif.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.fzhhl.top/gthxdagrvv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtgbthoabv.html

[M04] 获取当前工作目录
来源：http://hz.xylfe.cn/gtsmbvtofp.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtvgmqucjb.html

PHP:  getcwd();
来源：http://hz.snrcjt.cn/gtlhuguxcf.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtsuxnzbkb.html

TS:   process.cwd()
来源：http://hz.tanke756.top/gtbikpfejh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gogol.net.cn/gtjrpgbvxp.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtfhecyhnl.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gthaabqwao.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.meibo888.top/gtaamzigmk.html

[M05] 设置退出码
来源：http://hz.nanxuanxn.top/gtqvgjqkco.html

Py:   sys.exit(1)
来源：http://hz.iojbl.cn/gtgxtpimyj.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtulhbcmyy.html


<!-- 参考信息 -->