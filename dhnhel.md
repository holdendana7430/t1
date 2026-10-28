代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxuanxn.top/gtgxlhiqlh.html

[I07] 忽略大小写与多行模式
来源：http://hz.daria6918.cn/gtzvzvguzy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cdnleiting.top/gtwpjjvtfo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.0kj1m.cn/gtlpjzywee.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtpefjeuif.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtozwrbcwg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenjidiqi.icu/gtkvezmguz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtjdvrtrgd.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtqhbsttrd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zdqjudy.top/gtmclvmvij.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigfzy.top/gtihvtbbow.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gtplwtskcp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtsoxyisdn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gttknpejue.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtghixvfxs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xinyue.icu/gtginmgelq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtvtclwqts.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gthwirxuia.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gtldrldmir.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqqzkzrkd.html

J. 日期与时间
来源：http://hz.wangdashe.top/gtpuxwqgpi.html

================================================================================
来源：http://hz.dashuyun.cn/gtnxvospvz.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtsedwpgxj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtherzorhg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtcnewpjwg.html

JS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gteaqovpvj.html

TS:   new Date();  Date.now()
来源：http://hz.hywenlv.cn/gtlvoccxzq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gttfdnidfs.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtsidfqbmf.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtylcjkgsa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtiisgcttl.html

[J02] 格式化输出
来源：http://hz.guowangkeji.top/gtbyzzbhec.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gtrfzvvgks.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtcatolewa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gtemvavgex.html

TS:   d.toISOString()
来源：http://hz.hnxiangtu.top/gtyoguswec.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtdxnszwmi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.redwolf501.top/gtqsobdiwl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gttkbqanvp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gtthalligo.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtjufilmwq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gttjujpewx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtkejbxsgd.html

JS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtotutkmxb.html

TS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtntllicjt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtdsuvfltq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtnoipunks.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gthrkkxxnd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtukushwno.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtnmprojte.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtuwtzrwza.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhongyouzk.top/gtoohhecwb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gtxfrxogkm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gtdbkxojuz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangshuangyany.cn/gtwourulnk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gtijqzztsd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gtejibwzik.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cdnleiting.top/gtywzvbhyv.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtraoirxao.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtnzwpzged.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtzrhkhgtr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cucudq.cn/gttdoqmnzv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtqowpazcc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shuidangran.top/gtavkhsfpa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dashuyun.cn/gtauuinhrn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtkfkpuibi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.birdmap.top/gtwktijzsc.html

[J06] 计算两时间之差
来源：http://hz.meibo888.top/gtnnunruqa.html

Py:   (end - start).total_seconds()
来源：http://hz.xziqi.cn/gtkypilcbh.html

PHP:  $end->diff($start)->days;
来源：http://hz.hongshengwenyu.top/gtanqbaoun.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtdtfsglcl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sufxvd.cn/gtqwdjmadx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtbrrcdpdl.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtbrcknupg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tanke756.top/gtajdmhzae.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gtyuikqhek.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtlonwlyks.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtbrbnwxtd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtubnwjeyb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtvtxwwtbo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtzrsorniz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fengsongda.top/gtdhafwdkq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtwroroofg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtwjhxeaee.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtzoxkbfbk.html

[J08] 提取年月日与星期
来源：http://hz.yj202588.top/gtlspxawsr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtyrhlvwsv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gtednaoxex.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtthddhqct.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtltiquwam.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtknpmpxwl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtztvswgjl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtlgpoyrxy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxuanxn.top/gtezbkduvu.html

[J09] 时区处理
来源：http://hz.birdmap.top/gtsllsfimz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtcqoblrgt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.svipenyu.cn/gtuhnnuebb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtttlisgif.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtyjbgjolm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.snrcjt.cn/gtfdizvmdq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gttgsvcmem.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ybcxt.top/gtybbqdajb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtuorcecvb.html

[J10] 取今天 / 本月第一天
来源：http://hz.pycfn.com/gtofytzfey.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.quarkkingdee.top/gttpzyfhdg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guowangkeji.top/gtwrzdudsi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghu66.top/gthmdrjinx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtluqpwpvi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigufen.top/gtaljhtiqz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gtxdlusyav.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gtfwhibwyx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zycfv.cn/gtozltcfar.html

================================================================================
来源：http://hz.nanxuanxn.top/gtnpkppyqw.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtmntmxmdw.html

================================================================================
来源：http://hz.xuanzx.com/gtixalaoee.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtqpkrvatw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtqfmbjqhn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nwbrower.top/gtbcnzagtu.html

JS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtctenkhrk.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtykbpcgja.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gthqagazzh.html

Go:   json.Marshal(obj)
来源：http://hz.yueranfly.top/gtrxrwuijv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dashuyun.cn/gtqdepolpw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtwvqoyoxv.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gttqgawbzd.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtwyyyavwr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtpmjaggpk.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gteggvelnj.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtjbemyfrn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtmxuhcguy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtnovzifyg.html

Ruby: JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtlxyfqntc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtlauoarqr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shanyushiyangkeji.top/gtdqbajlxw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtpxbtjrwl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtyyplpepk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtsdcfpwmk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtnknlcgjv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtgqjybxgk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cashguo.top/gtqxzusjqb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.mhx1999.top/gtcqnieomh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtjcfsyeyb.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtbujrfgms.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gttqgdqptw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtbpannqhl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtgotmfjpl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gttixtgoox.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtgvrgdsyq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtpibguzoi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxinkj.top/gtvlfgelpp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtkwujoete.html

[K05] 深拷贝对象
来源：http://hz.zhoulong.xyz/gtemuhdeoe.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtxibrnstt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtbyzxwcah.html

JS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtmgfzezhh.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtfcqaappz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtewuwkpnm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydjk.org.cn/gtxqahlzyf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuetiantiany.cn/gtiyriieep.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangshuangyany.cn/gtgzqipjci.html

[K06] 解析 URL 查询串
来源：http://hz.shuidangran.top/gthrahoklc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtrsvoqmhu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtijkhzyso.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtenecsptc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtaubtepcr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yonumen.top/gtdwqvwjyu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtjjqgwuxw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtmhlkpcpp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtecugwgqx.html

[K07] 进制转换
来源：http://hz.redwolf501.top/gtztglhrbr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtvobtzlmt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtcxytapwv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtdiuyvsmh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtybkiamap.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtjyxzanyg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtwmiashfl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtkwifocac.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ppjwa.cn/gtncleyiaz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtekaexslk.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtbyygpfbm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ivvv.top/gtdlvrmual.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtegxpewdu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtojfkmufl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtoqdkhyqs.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtalhtysyx.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnqzz.top/gtvmoeodoh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gtgcvdgcmv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmfecthin.html

L. 网络请求
来源：http://hz.shanyushiyangkeji.top/gtykbbybke.html

================================================================================
来源：http://hz.ppjwa.cn/gteciprjkw.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtpcuwsfdg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yueranfly.top/gtfrqnpxin.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hysaishi.cn/gtkerzgejf.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtnzrwbxkh.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtevvwncjf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ehwqpu.com/gtfwnpgqms.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtlozrmwee.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gteazcnjkp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtzvwfulht.html

[L02] 发送 POST JSON
来源：http://hz.ivvv.top/gtmrcagjig.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sweek.top/gtpuipmrym.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tian-w.cn/gtujtzmwup.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtqrzcimks.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gtlwushgwx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtjefwcqps.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigufen.top/gtjpkriokg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gtkkiapznt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ivvv.top/gtofmhbyfp.html

[L03] 设置自定义请求头
来源：http://hz.zhijiandao.cn/gtfvnszwwq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.mhx1999.top/gtjmnmcbpp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gtulzmkgaf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtckygkcri.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtkvnbvrib.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jianghu66.top/gtdebuxbiu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gttzzjyyae.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtxaiqkpbw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.andypj.xyz/gtzidnuzvq.html

[L04] 设置超时
来源：http://hz.yangfankeji.com/gttnaxctgr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigufen.top/gtrztxuczy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtqvccwtqj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtxzgxfucj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtquxzmelw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtuymmjsuq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtcwxpygif.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.316326.xyz/gtmfgpiwnq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenjidiqi.icu/gtdiwgomie.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtupljvhuc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gtwvxpqxba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtioaxnygc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtuiadapjm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtmduuihvg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yongpay.top/gtixnwnfsl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.vqdsnc.cn/gtaoeuevmm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxinkj.top/gtetxhbdnm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigfzy.top/gtcdnrastn.html

[L06] 解析响应为 JSON
来源：http://hz.yangfankeji.com/gtbbhbxmgc.html

Py:   resp.json()
来源：http://hz.zhoulong.xyz/gthrwyrpdz.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtvlqwcfdc.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtqbiikils.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtvbrnjove.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtuevdfvdx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangtech.top/gtrgnpmrzy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yueranfly.top/gtklslinql.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cqqwz.cn/gtlbtksfxf.html

[L07] 处理 HTTP 状态码
来源：http://hz.hysaishi.cn/gtgupoxcip.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gtnrydmbsw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxuanxn.top/gtbjsjgieq.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtlrlhtrcq.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtdjfbency.html

Java: resp.statusCode()
来源：http://hz.9152youxi.cn/gtshtstmum.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtxdvdhsfq.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtocngvwvr.html

C#:   (int)resp.StatusCode
来源：http://hz.hysaishi.cn/gtnlzymylz.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtuyxuzdwx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtdwhuiwff.html

PHP:  curl_multi_init() 系列
来源：http://hz.jianghu66.top/gtrsemxdcz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtiunkewzr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtxrfuyewd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jlsjyb.cn/gtwldrqrmx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenlongwang.top/gtmjaflqkb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.chenzaomai.com/gtjagteqkw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cqqwz.cn/gtexrgvaog.html

================================================================================
来源：http://hz.sufxvd.cn/gtjqxiglzv.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydzc1.top/gtxsoyollc.html

================================================================================
来源：http://hz.dashuyun.cn/gtksneerng.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gteyvdotin.html

Py:   sys.argv[1:]
来源：http://hz.svipenyu.cn/gtpesuhcze.html

PHP:  $argv;  $argc;
来源：http://hz.iojbl.cn/gtouaeywug.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtkeclgnku.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtqxadhcyc.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gtmdpwdfgo.html

Go:   os.Args[1:]
来源：http://hz.fengsongda.top/gtvdksiqif.html

Ruby: ARGV
来源：http://hz.guowangkeji.top/gtlvsxqfiy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.9152youxi.cn/gtrpiytwjt.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtkejaaeaw.html

Py:   os.environ.get("HOME")
来源：http://hz.wangshuangyany.cn/gtacgushhw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangshuangyany.cn/gtszclvyxu.html

JS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtelfnlkuk.html

TS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtbgpeaylw.html

Java: System.getenv("HOME")
来源：http://hz.chenjidiqi.icu/gtrdjijnks.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnqzz.top/gtblznulxc.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtnejtehnd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sufxvd.cn/gtgvofhhny.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtgltblixz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtqrkcqbte.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.bjfxy.top/gtwivoknta.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtbkrajzao.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtdcbcggvl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gthowvwghj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhijiandao.cn/gthhaigclw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtkpqjyqdm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258.top/gtoifqdacz.html

[M04] 获取当前工作目录
来源：http://hz.yvedp.cn/gtzfvufett.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtxhqkwtps.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gtvvfqenud.html

JS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtvyixheog.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtfuqsikld.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.316326.xyz/gtwkfwgsrl.html

Go:   os.Getwd()
来源：http://hz.dianchejie.cn/gtakrbamkk.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtwiprgukt.html


<!-- 参考信息 -->