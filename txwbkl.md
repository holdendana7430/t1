代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtubmddesc.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtcvzfczrf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtmiyobskm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtbuuudueb.html

Ruby: s.scan(/error/i)
来源：http://hz.birdmap.top/gtjkmucwor.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.redwolf501.top/gtxfcjdrug.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gtkynjuewe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gtsvehjkso.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtozfaqldx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtuuojylog.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtrrsqdiia.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtydrcggrm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtgbconobw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gthvacixsu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtnrrrkxip.html

================================================================================
来源：http://hz.zhengqikj.top/gtpkvabbbm.html

J. 日期与时间
来源：http://hz.havefunace.top/gtvwotrvnh.html

================================================================================
来源：http://hz.vqdsnc.cn/gtexseuazh.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtskprgvze.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtugpowymk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtdtvzdfxl.html

JS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtqyndrknv.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtpcjgrclc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenlongwang.top/gtpyimjpcd.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtjefdyqgx.html

Ruby: Time.now
来源：http://hz.sysykeji.top/gtafarwkkr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinyuanbaomall.cn/gtwqzeifoq.html

[J02] 格式化输出
来源：http://hz.andypj.xyz/gtvgugsxjs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtgouxcrdp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtrvnncddd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.mhx1999.top/gtnaznwagb.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtguykdflx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jiagoushi.top/gthasfsvfs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtdqorenif.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtbileuvae.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daxiang520.top/gtrngyiufi.html

[J03] 字符串解析为日期
来源：http://hz.cdnleiting.top/gtjlpiulpx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangdashe.top/gtcldbcfwq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.havefunace.top/gturlyfnjp.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtjrneoyop.html

TS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtheohtqoj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtzarokrhw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gttxchcvbp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtscfgivrz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cdnleiting.top/gtwhiybyno.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtpcdtfljn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hfpthk.cn/gtboovcyaz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtewjccpar.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtkpzuctui.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtstqsctkw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtcceclxeq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtzovtctun.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gtyggksysu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhiwuduotai.top/gtgehtfysz.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtjvtfjoeh.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gtylazxdue.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.iojbl.cn/gtzrlppaid.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtjfkbxssu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtsmrgfmcp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.quarkkingdee.top/gtvlvrlttl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtnluushmx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gtlwlwrwez.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtvqtbfida.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtakpthvwr.html

Py:   (end - start).total_seconds()
来源：http://hz.cheryme.top/gtkftzngqb.html

PHP:  $end->diff($start)->days;
来源：http://hz.quarkkingdee.top/gtmewjlrir.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtpeeswzmw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtiqoyahfa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.316326.xyz/gtvikzhfvt.html

Go:   end.Sub(start).Hours()
来源：http://hz.yvedp.cn/gtmqogjrto.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gtvluwksho.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangdashe.top/gtxdortvgr.html

[J07] 比较两个日期
来源：http://hz.jinghuilouyu.cn/gtglfvnmso.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtzgvuhxfi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.52xcode.cn/gtbmauulor.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtcbhwzazg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtqpsoczdd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gtizljydul.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtobxrjbav.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtcdnplgqd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtrgkphvdk.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtslwsvvzv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gthxrlkyvb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtesfmdasv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtsiqzchxa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtaoarwpdg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenlongwang.top/gtgkjzgydv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtpnkrlmzj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtwrbvngyq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydjk.org.cn/gthphjjebf.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtgwmaxtyh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.mhx1999.top/gthaaookqx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj202588.top/gtscvvdrcm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtyhxlehet.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtwtsaiqdy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xingfuxueyuan.xyz/gtmcpgsuzu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtiewoscfm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtjtlsroax.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gttynhgnbx.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenzaomai.com/gtkzuwqhau.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aibaodan.cn/gtrmixbpwu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tanke756.top/gtewifwren.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cucudq.cn/gtpylntppq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gtqobhprnw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.haohaochexian.top/gtohtbsckh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtedmcnwvz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yueranfly.top/gtzvdxwpah.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aizwys.cn/gtyostqnlw.html

================================================================================
来源：http://hz.jlsjyb.cn/gtunxermpg.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gtntbsvsjy.html

================================================================================
来源：http://hz.hywenlv.cn/gtklezzzmr.html

[K01] 对象转 JSON 字符串
来源：http://hz.fengsongda.top/gtbiqfqbld.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtvvlbosyb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtyzgbkltd.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtlowvghtd.html

TS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gthuvsbgor.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinyuanbaomall.cn/gtezoewvth.html

Go:   json.Marshal(obj)
来源：http://hz.c1oappe.top/gtzumtztpo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtjkcqalep.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yangfankeji.com/gtoosucgqw.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtcsgputpe.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangkeji.top/gtfdbyfret.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtcpvxnhoq.html

JS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtkxeqaczw.html

TS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtjmddgwms.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtqlfkmdns.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gthdhyyanb.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtotwpnrxp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtgatzmfbo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gotoacloud.top/gtyraudrzc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258.top/gtcdktryzw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtymoumynb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtksrrxoqj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtaqesgkoy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtffvfvbon.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinyuanbaomall.cn/gtkmpehmeo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ppjwa.cn/gtjbfkkrog.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtytuugbym.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gtikyzkrvb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtdvsiqcgj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gtbsumoyyx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtedeluihe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtdoaixpyv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtpobzwfnr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtyxifvrcr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yonumen.top/gtnuiksohr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yanxiufei.cn/gtdvduexvy.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gtlxoditzu.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gttnvqjulw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yonumen.top/gtvepydufw.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtefslqxhw.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtesgxqmho.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shzxlz.cn/gtvqmxahfj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtmmdnmtab.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.quarkkingdee.top/gtmffofcit.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yueranfly.top/gtziypepdu.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gtptegdopt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gtrmoqzgqx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jyoumei.cn/gtunmzicrs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtdtvlejcv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gttejnjdln.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ivvv.top/gtmpojsbrp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtkltjnftx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtdcxzywfn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtijsgjmaw.html

[K07] 进制转换
来源：http://hz.svipenyu.cn/gtnzggpdjn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtyrihvpyk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aibaodan.cn/gtiyymcsym.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtquolxwft.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtuzojppxi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtjiyurkto.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtlssbsjhc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gtcntdeboh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtskuaoibh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtcabliejo.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gthpipyclj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gtbwifwfjf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtbikpdany.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtpdonllsm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtxmxeeiur.html

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtqgczgbsm.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtaaksbisw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnqzz.top/gtxivmndln.html

================================================================================
来源：http://hz.tanke756.top/gtjcvdawfb.html

L. 网络请求
来源：http://hz.sysykeji.top/gtamhkhweu.html

================================================================================
来源：http://hz.fzhhl.top/gtmrzduxct.html

[L01] 发送 GET 请求
来源：http://hz.9152youxi.cn/gtgisnvxfi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtuqgireko.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gthezefuhl.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtuunxtthq.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtmnnjireo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sysykeji.top/gtebaymixh.html

Go:   resp, err := http.Get(url)
来源：http://hz.yonumen.top/gtnggfwjea.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtixgufgaf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gtywabrffr.html

[L02] 发送 POST JSON
来源：http://hz.sweek.top/gtkoqbqsfe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gteijkkdyn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtebubdjqe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtbknfftaj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtxxycijtw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daria6918.cn/gtnnvhggex.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinghuilouyu.cn/gtenngkzxx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.9152youxi.cn/gtkbwvvgmc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dashuyun.cn/gtvhuqmshu.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtobjjwmwu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.meibo888.top/gtpnmtpvro.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gthnqubuiw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtlwgtthrx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gtbdptlngh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gtyitywmfv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtpnjgdeez.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangtech.top/gtfzerdukx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cheryme.top/gtffppslsa.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtsdpgdveu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhijiandao.cn/gtrlqkllja.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtdxohaapm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gthulyxejs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtqqpmudgm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtdrfolkib.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtjemhwlkg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gotoacloud.top/gtmcytiydq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gtgqlytvch.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtxrozqzkj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuetiantiany.cn/gtmxbhlzpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtdkfcdxng.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtygftgaez.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtfokzwyup.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tian-w.cn/gtrcmgsruo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.vqdsnc.cn/gtmfunukin.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cheryme.top/gtbhdmhzik.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhiwuduotai.top/gtzruljhcz.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtdpbejuqe.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtrcxrlxmd.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangtech.top/gtztjcyrhc.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtvculqufw.html

TS:   await resp.json()
来源：http://hz.zhixingplan.top/gtlwaaqwwf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtxdeytjjs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtbhjbzaic.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gtfhuewdwf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sweek.top/gtnbzdyfrt.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtkepfcpkz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.kuanghao11.cn/gtpyfaekga.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gtpgspfahn.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtdokxwqdr.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtlztbrdlm.html

Java: resp.statusCode()
来源：http://hz.zycfv.cn/gtsbbahmla.html

Go:   resp.StatusCode
来源：http://hz.aibaodan.cn/gtgyoqvxla.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtmhytshkt.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtqwshqzww.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtrpdygdfk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gttlmdbjgp.html

PHP:  curl_multi_init() 系列
来源：http://hz.gaohongyu789.top/gtxdebksgu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtnbiacasa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtoqcmmmkk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.aizwys.cn/gtpovwipoc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258.top/gtkkndbkhl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gttkptyzli.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sysykeji.top/gtbygzdzbz.html

================================================================================
来源：http://hz.bjfxy.top/gtaynevrre.html

M. 命令行 / 进程 / 环境
来源：http://hz.vqdsnc.cn/gtnwpgejis.html

================================================================================
来源：http://hz.jlsjyb.cn/gtwpucyadl.html

[M01] 读取命令行参数
来源：http://hz.guowangkeji.top/gtycszwgdf.html

Py:   sys.argv[1:]
来源：http://hz.svipenyu.cn/gtzahrecoy.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtdephwsyx.html

JS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtknqjqerp.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtrdwqmfpe.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtknsufoqs.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtpwmpdtll.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtezqhtxhp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtgidqhvxb.html

[M02] 读取环境变量
来源：http://hz.nanxinkj.top/gtmizssven.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtkebudycg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtcrhsphyq.html

JS:   process.env.HOME
来源：http://hz.yuxming.cn/gtjywgcsrb.html

TS:   process.env.HOME
来源：http://hz.c1oappe.top/gtproejlvx.html

Java: System.getenv("HOME")
来源：http://hz.shuidangran.top/gtycopzasd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtblejwlpi.html

Ruby: ENV["HOME"]
来源：http://hz.xingfuxueyuan.xyz/gtaatpnzwo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtylsijcjf.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gttbeaowwh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sweek.top/gtptvmnlir.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.mhx1999.top/gtzcnlgdiq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtgvkbcaik.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gttmmmhovu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gotoacloud.top/gtbhliatua.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.mhx1999.top/gtkvzqozkx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cqqwz.cn/gtpyphdkxj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtmnnqjbgo.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gtnaziiwty.html

Py:   os.getcwd()
来源：http://hz.wangdashe.top/gtpzvbyuic.html

PHP:  getcwd();
来源：http://hz.pycfn.com/gtfshyfccm.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtosrnabnl.html

TS:   process.cwd()
来源：http://hz.hfpthk.cn/gtayieusvk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gtakoyyiau.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtdqmxhetp.html

Ruby: Dir.pwd
来源：http://hz.birdmap.top/gttygvtikf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shzxlz.cn/gtvhvqbdia.html

[M05] 设置退出码
来源：http://hz.zhaomingkeji.xyz/gtdilatojb.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gthxzxcksg.html

PHP:  exit(1);
来源：http://hz.yj20258.top/gtqweejchh.html


<!-- 参考信息 -->