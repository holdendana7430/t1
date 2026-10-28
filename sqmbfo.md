代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtmyswuvqh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.316326.xyz/gtsxcvsaiv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtsuyubpvo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.havefunace.top/gtmvllevjd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtcdwfmhuw.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtvfafskhu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtcmjnvlfk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtktwxjswy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtnkxjexck.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtibaxvdqr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sysykeji.top/gtwsrxiatf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.andypj.xyz/gtfrasrhzq.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtpgvhmsje.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhongyouzk.top/gtsehoxafu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtiluauzts.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtrodobdiw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aibaodan.cn/gtklyoivbq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtlnmrkiri.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtfmuvagum.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtxpjjgaih.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangtech.top/gtcjdfnufg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuanzx.com/gtvcgthgwv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinqigufen.top/gtrdauidvu.html

================================================================================
来源：http://hz.zycfv.cn/gtoywcgqft.html

J. 日期与时间
来源：http://hz.daxiang520.top/gtlrgkynui.html

================================================================================
来源：http://hz.gogol.net.cn/gtnkjhgkvv.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtakkqgctl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtgryeypnu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtbkzzxttv.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtyarpocil.html

TS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtwaooinnt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtsawonbxz.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtsgjavhqt.html

Ruby: Time.now
来源：http://hz.jianghu66.top/gtcgrhznkd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtghrmqkbb.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtfqjcedge.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtgufkzuov.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gteznamcyh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gtbpnatbnk.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtwyntbsqj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jyoumei.cn/gtmeakatss.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jianghu66.top/gtkykikxaa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtqpmoidic.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tanke756.top/gtzudlaujf.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtrdhqgetv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gthfcvwmpl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgfzy.top/gtvgpxgzmj.html

JS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gttvkjgnje.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtpeeglwgy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtnwyagyld.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtuykigdcz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtrnoqwjoi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtmjtvtzay.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gthcvdmoxn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenzaomai.com/gtquadkogp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ywan-chungtsiang.top/gtvwdpkjtf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhixingplan.top/gtdmvdblmv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangshuangyany.cn/gtastlxrzz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtikrvfrge.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtxuealpxp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtojtlsyjt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gtxkxsgrcq.html

[J05] 时间加减（加 7 天）
来源：http://hz.c1oappe.top/gttvkmqiry.html

Py:   now + timedelta(days=7)
来源：http://hz.zhijiandao.cn/gtlwhpolpu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtlppeuwfy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtaqeogvcy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gttsrwhzni.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtksucddrt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigfzy.top/gtvwioowea.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xylfe.cn/gtlcrbcwhm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gthfwyczap.html

[J06] 计算两时间之差
来源：http://hz.yonumen.top/gtnuectfbh.html

Py:   (end - start).total_seconds()
来源：http://hz.cucudq.cn/gtsthofefg.html

PHP:  $end->diff($start)->days;
来源：http://hz.havefunace.top/gtzdpbatgg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgufenzy.top/gtflbbgtcv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daxiang520.top/gtalhwuzwm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gtmyruemun.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtvawkjyfb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shangyingyoupin.top/gtlednzmoh.html

C#:   (end - start).TotalSeconds
来源：http://hz.0kj1m.cn/gtmcphhgie.html

[J07] 比较两个日期
来源：http://hz.yongpay.top/gtihffliir.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtzgoxepyu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtvyjtfzkc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtpvybfqdg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.9152youxi.cn/gtexcqdiqz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtfevdxpkf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.redwolf501.top/gtuoeioiet.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtuxptqnqx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtcgatejhr.html

[J08] 提取年月日与星期
来源：http://hz.yanxiufei.cn/gtjstbxbjo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.vqdsnc.cn/gtvwjgrisq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtmpmuqmpe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gtphdddaav.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zycfv.cn/gtpllbwker.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxuanxn.top/gtdcuxumhr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtjqrhomec.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fengsongda.top/gtecwcobkz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jyoumei.cn/gtwfdidxse.html

[J09] 时区处理
来源：http://hz.sufxvd.cn/gtesglvzqb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.0kj1m.cn/gtjrgwhxdh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtiukjwesz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtmvumfqvs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gtwwyhzkyt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtpygbuhpx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.feifeiyinyue.top/gtenpqjody.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtokzccuzu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gtedbpmfpx.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtbjuuyxea.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gtidjzeekc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtapfrseop.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtanngwrqd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.vqdsnc.cn/gtpzsopirb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gtyugaeyfn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtdfjirfxq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gthbrnbdse.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtgnddgapb.html

================================================================================
来源：http://hz.redwolf501.top/gtzxygxsvq.html

K. JSON 与序列化
来源：http://hz.yj202588.top/gtxazjdmpb.html

================================================================================
来源：http://hz.zhixingplan.top/gtyoflxisx.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gtyxugywbh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtgtieefwr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gthzgahosi.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtquobunxm.html

TS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtfjwyushx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtdpldwwxc.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtszixfipk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtaxvedsfb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yonumen.top/gthwqubavl.html

[K02] JSON 字符串转对象
来源：http://hz.shuidangran.top/gtheencvnu.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtxhjulbmh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtztkanouv.html

JS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtasbcrbqx.html

TS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtjifqiwkn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtpvjatvvv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtxlhxjhof.html

Ruby: JSON.parse(s)
来源：http://hz.316326.xyz/gtjyjssgcz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtbzruseau.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gthhcnmnhb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtfkxeldyd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtitxribbh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtuzautveh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gttjmgzjsh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtcwzvwzat.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gtxqicrgkf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.vqdsnc.cn/gtygbajlyc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gtsjlmtovp.html

[K04] 读取 JSON 文件
来源：http://hz.cheryme.top/gtxrolopap.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuanzx.com/gtmiybcpwg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtrkaaranr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtogejlcws.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtsrykejic.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258.top/gtvzbuqjwd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtqxledmxe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dashuyun.cn/gtttngpbmn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenjidiqi.icu/gtlvtquqsb.html

[K05] 深拷贝对象
来源：http://hz.jqgufenzy.top/gtuihaulcx.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuanzx.com/gtgpwoeswu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pycfn.com/gtgafvzkeo.html

JS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtwlvrqilg.html

TS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gteecaehma.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtvzkmizki.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gtrxuueuth.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhoulong.xyz/gtexbaflsr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.c1oappe.top/gtxvvfnngh.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtsduwffdj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.haohaochexian.top/gtnwqdnlie.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gtpofdrdbn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtvodhksrz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtyfmtepyp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtisthjpil.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtpypevxbk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtkjaempux.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guannengcc.top/gtvwefmonj.html

[K07] 进制转换
来源：http://hz.tian-w.cn/gtaeeccbvu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtigwxpkoc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtoivjbdty.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gthbyszuag.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtiziuegcn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtynsnzald.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cheryme.top/gtkexopacy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtzglihjiq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhiwuduotai.top/gtimvnpctu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtkmhhdequ.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtrzdglqkn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sxryk.cn/gtwxwconhs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gttffibpya.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtlvizogcg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuetiantiany.cn/gtwqvwzqqs.html

Go:   encoding/gob
来源：http://hz.zhaomingkeji.xyz/gtukrjoszn.html

Ruby: Marshal.dump(obj)
来源：http://hz.gaohongyu789.top/gtikgirxxy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gzhubu.top/gteiahunsg.html

================================================================================
来源：http://hz.xuanzx.com/gtwtqmfumg.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtzlkhpdpx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqxnfgzyp.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtlrvnyatu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtpifjjzot.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pycfn.com/gtpskxlwbj.html

JS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtdgxctfff.html

TS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtjckxvsnb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cqqwz.cn/gtnemrjxcu.html

Go:   resp, err := http.Get(url)
来源：http://hz.andypj.xyz/gtrhsorhur.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtxvfnudsr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtrwmfxmfl.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtcuftgxaa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhoulong.xyz/gttwvdokze.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtgphmeukk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtwvercyvq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtmujiqxpl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtkanfkzwi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtjijemome.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtktbmfcsw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhixingplan.top/gtzqffmdus.html

[L03] 设置自定义请求头
来源：http://hz.birdmap.top/gtjooxcomn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gtmstrocef.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.smart0.xyz/gtfvfhvbkb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtwkuwpkps.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtzpcjboem.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pycfn.com/gtqlndixcq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtyhdhtxng.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gtgdzdbmjp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenzaomai.com/gteptozmjj.html

[L04] 设置超时
来源：http://hz.jianghu66.top/gtnqywnbce.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj202588.top/gtoblemxjb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtamlqictp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtbjqpdbyd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtvqpciyer.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtxlxlegkk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxuanxn.top/gtijkjgaqm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cucudq.cn/gttesuvemu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtzciisnxa.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtjpvdpqcm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtlghkuyng.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cdnleiting.top/gteeoarubq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtlmpmrmwg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtgwkewzve.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hysaishi.cn/gtlkmvotto.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtftggkbki.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtwqhoixci.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gttcojmcwa.html

[L06] 解析响应为 JSON
来源：http://hz.yangfankeji.com/gtrujkexbu.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gtbhxjbzfv.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gteusyrkrp.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtxwmxviee.html

TS:   await resp.json()
来源：http://hz.redwolf501.top/gthtsdsvgn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.52xcode.cn/gtwlkzibnw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gtxqchoiaf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.iojbl.cn/gtapsgsbjs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gtslwqxpys.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenzaomai.com/gtbjnfxqgs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dashuyun.cn/gtqytnwcjb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.quarkkingdee.top/gtjudbazaz.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gtsxbaoevb.html

TS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtdraixppp.html

Java: resp.statusCode()
来源：http://hz.yuxming.cn/gtwtoaokeh.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gttdlmvovs.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtfxbmhiqe.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtchsadpjq.html

[L08] 并发请求多个地址
来源：http://hz.xylfe.cn/gtaixpohzi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fzhhl.top/gtbnunrsye.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtpotqyzsa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtbadhvduy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gttabosntb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtshnknuom.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtsdruhkdt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtjjvaslxw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.haohaochexian.top/gtjuxbipsa.html

================================================================================
来源：http://hz.meibo888.top/gtjomakrmn.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj202588.top/gtvqnmeybp.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxfdlfvqf.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtcyyxegax.html

Py:   sys.argv[1:]
来源：http://hz.iojbl.cn/gtbfzuluvh.html

PHP:  $argv;  $argc;
来源：http://hz.zhoulong.xyz/gthamdqkcg.html

JS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtgvcbodnd.html

TS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtienchnuz.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgfzy.top/gtlmdzoogb.html

Go:   os.Args[1:]
来源：http://hz.tanke756.top/gtckqzmoet.html

Ruby: ARGV
来源：http://hz.hysaishi.cn/gtsubuxqql.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtngegvkkl.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gtmhulxiab.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtjsfgtdex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.aizwys.cn/gtbjobotfj.html

JS:   process.env.HOME
来源：http://hz.cucudq.cn/gthbucbfqy.html

TS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtfdbokowm.html

Java: System.getenv("HOME")
来源：http://hz.shzxlz.cn/gtzpvkvqvo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gtjcplefjk.html

Ruby: ENV["HOME"]
来源：http://hz.yueranfly.top/gttevmrocx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.svipenyu.cn/gtqqrtkfbw.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gtchjbolmp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guowangkeji.top/gtzomwnqjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtpmkpnopz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtxqsebmoi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtgvclmgnz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtpzkfentc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtifyxheeg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.c1oappe.top/gtcdngeqfc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtwgscfobn.html

[M04] 获取当前工作目录
来源：http://hz.bjfxy.top/gtgkoqqafn.html

Py:   os.getcwd()
来源：http://hz.zhiwuduotai.top/gttligtxqy.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtaydywzga.html

JS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtnjscochc.html


<!-- 参考信息 -->