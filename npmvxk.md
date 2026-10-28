代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtztivaaws.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gtgwpkjyzo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangtech.top/gtfuqwzcdj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yongpay.top/gtxigdszzd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtjajbksoe.html

[I07] 忽略大小写与多行模式
来源：http://hz.sweek.top/gtddsmrfro.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtkirnrzuc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtdeqtqsdf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gtvmyzvqxp.html

TS:   /error/gim
来源：http://hz.kuanghao11.cn/gtumzmqcha.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gtkrbyatil.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydzc1.top/gthqpippce.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtlzdrcnvr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daxiang520.top/gtmqlanvzm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtggjzzoyb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gtbaipeyot.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtqxripvij.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtyrdbhtkp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gthkqiznpr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtwowbbwpm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtbuuxhcgn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.kuanghao11.cn/gtbcyupswe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtwjorzvyb.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtlxpxaljw.html

J. 日期与时间
来源：http://hz.0kj1m.cn/gtrlafswty.html

================================================================================
来源：http://hz.shzxlz.cn/gtjxthlikf.html

[J01] 获取当前时间
来源：http://hz.snrcjt.cn/gtldhngkfi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cashguo.top/gthzhittky.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtjmmeofyj.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtfbcurumd.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtcatdjgbl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtzwjjgvby.html

Go:   time.Now()
来源：http://hz.pengpengdd.cyou/gtktmerghe.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gteyrdqamw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxinkj.top/gtlhksrviy.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtepsjzxaf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtzfialtho.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtnljdrvji.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gtlfudilly.html

TS:   d.toISOString()
来源：http://hz.zhongyouzk.top/gtuzsaklxp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtoqraaaqw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtskkchnda.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtfdxkodqz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jyoumei.cn/gtekskdkar.html

[J03] 字符串解析为日期
来源：http://hz.wangshuangyany.cn/gtckazvyss.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangkeji.top/gtmlajgebg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gtwpzbnjyz.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtjhcynhzt.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtozvaqeat.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtdkouklnd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtaceeelhp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gttzbdgyjb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtenkzsvbn.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtdysvywqw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtjfiebfmp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtssvddgwu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gzhubu.top/gtsyhxquyc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gttklytopz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gtyzvuplmc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtvadpwrki.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtfjaajsev.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtaqaoozsb.html

[J05] 时间加减（加 7 天）
来源：http://hz.xuanzx.com/gtnfpfymww.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtoqjlylbj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dashuyun.cn/gtevznguvb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gteywrcczh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtqxoyojgq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnqzz.top/gtdipqyqli.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.kuanghao11.cn/gtsyhkbvpz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gtndryibht.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydjk.org.cn/gtvnuveumq.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtryqvpebx.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gthhxltkvn.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtvqktskqr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gttddfovva.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gtzmdjedso.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtwouzofek.html

Go:   end.Sub(start).Hours()
来源：http://hz.jiagoushi.top/gtvlhsyidk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtiwadgcax.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gtcfmageye.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtqgtvhgaf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtequwpese.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtmnguhyxr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtwbcgzxkl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtjnbcnbpi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtqjmwaipy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xylfe.cn/gthopmeukw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtvcqyaxtw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtygwndlrr.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtxzksmfyt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtiflnadfa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtxrrmwnqa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jianghu66.top/gtpibimupj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtcuhomcyi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtgcokyfzf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.52xcode.cn/gtpywblths.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtcmjopjgy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtyhxuxapw.html

[J09] 时区处理
来源：http://hz.pengpengdd.cyou/gtbhszgspy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtxkxyextr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtlpozctum.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gthoidwend.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtbfjiyizn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtcvuiekvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtcvofkszh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtmjfkrgsc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gtuofxrmgn.html

[J10] 取今天 / 本月第一天
来源：http://hz.cheryme.top/gtpnhuvlyv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtejiflcvl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gtfmcczxaw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtpyfulyez.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgufenzy.top/gtdqjqaljn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtzbfaziph.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhixingplan.top/gtkdefqqpv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangdashe.top/gteelmdchw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtqwisiopr.html

================================================================================
来源：http://hz.yongpay.top/gtpyoxnhyk.html

K. JSON 与序列化
来源：http://hz.iojbl.cn/gtejpaqfow.html

================================================================================
来源：http://hz.meibo888.top/gtyrehzbxa.html

[K01] 对象转 JSON 字符串
来源：http://hz.sweek.top/gtbglrogto.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtbtflzyij.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtghmggnak.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtgcvprpad.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtsugrbpsf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtnhcznnjs.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtyvdzwqpz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xingfuxueyuan.xyz/gtamzmlmin.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gtzqkhguwj.html

[K02] JSON 字符串转对象
来源：http://hz.aizwys.cn/gtoonwwvic.html

Py:   json.loads(s)
来源：http://hz.sxryk.cn/gtusilsmnz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtlvvppfgp.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtfqrtnbtr.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtqslquiav.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gtkloyoulo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtildceeyx.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtwqbthyjx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gttedxoqzq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.kuanghao11.cn/gtlqwlxhdi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtqfwfwxwk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtkebrffup.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtjfmlugqx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gttwgzztqr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhongyouzk.top/gtavwucime.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cashguo.top/gtbdugsiyu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangkeji.top/gtrnsaxety.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jyoumei.cn/gtihxvmijx.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtvivpqlky.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gtirtlgzux.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtkmjwatzs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtswkclgwl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtfdfnccvu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gtzpwblotv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtditcezej.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtpkehwllb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gogol.net.cn/gtwqmwdhht.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtroprhoth.html

Py:   copy.deepcopy(obj)
来源：http://hz.shangyingyoupin.top/gthtuukqdp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtdbcqyhon.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtapzadsjg.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtfbvpixga.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangkeji.top/gtqtdmjnoj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangshuangyany.cn/gtfmxuogqn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuanzhike.top/gtltjujznc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ivvv.top/gtdmiarubr.html

[K06] 解析 URL 查询串
来源：http://hz.haohaochexian.top/gtbxnstfxg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nwbrower.top/gtyvyzwfvq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtdohgsmtb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gthhfkunjc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtbbuidzfz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgfzy.top/gtqomtujlu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtnixwclcg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtlezgyiom.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtfsedcntm.html

[K07] 进制转换
来源：http://hz.c1oappe.top/gtvnuujdjo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.9152youxi.cn/gtylusmlyw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtmkgqrjmo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtbyywsdys.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtdenkeino.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtxtcgmhvj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtdzhjumyk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtamehfoxr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtyomzbuhi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtcfzmicic.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtdbivbuuf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtibbirmqu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gthszpscfu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtnejhxhbo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nanxuanxn.top/gtydhqzfhp.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gtqobrvjdi.html

Ruby: Marshal.dump(obj)
来源：http://hz.yongpay.top/gtzlvtxmrm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydzc1.top/gtqmspwsww.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlnnxcxjz.html

L. 网络请求
来源：http://hz.jinqigufen.top/gtoqhnoxly.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlrhyundf.html

[L01] 发送 GET 请求
来源：http://hz.cashguo.top/gtqshtfxdr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ybcxt.top/gtfoimzzru.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gthkjindfi.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtptuotosp.html

TS:   await fetch(url)
来源：http://hz.havefunace.top/gtmojtjhic.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtzcliyais.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtwsocliea.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cqqwz.cn/gtdduvnjnd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gtcyyqrlxt.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtiisedyvc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtzrvingmr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtkgqopyef.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtyhxicqgi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtxywgmvvf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtznkqifkb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sweek.top/gtrnejuxqk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj202588.top/gtbcojwwzp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fengsongda.top/gtjjhodrez.html

[L03] 设置自定义请求头
来源：http://hz.jqgfzy.top/gtcdqypkjs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gttsxwgbcm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.smart0.xyz/gtmfwrpeql.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gttfbdzhnc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtgyfdqkby.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinyuanbaomall.cn/gtcaszqhxl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtazptbyui.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fengsongda.top/gtiffvpkjx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtguqceruy.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtldpavuhk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtbsubthsp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gtugkohhri.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.meibo888.top/gtvgipupci.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtursfilnz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yongpay.top/gtgrmckitj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gtrwdmbbsm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fzhhl.top/gtsjpuxrwi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aizwys.cn/gtokeoftkx.html

[L05] 上传文件（multipart）
来源：http://hz.316326.xyz/gtkqlqabvm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gaohongyu789.top/gtwlawyudz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gtpjppwltd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtedkzchem.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtwjksgjlq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtuvsxiwji.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gtxdaxusas.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtzeofshjn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gtabfvxryp.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtqueacokq.html

Py:   resp.json()
来源：http://hz.pengpengdd.cyou/gttvhsaogj.html

PHP:  json_decode($body, true);
来源：http://hz.cucudq.cn/gtlialxqed.html

JS:   await resp.json()
来源：http://hz.ybcxt.top/gtprmpqakd.html

TS:   await resp.json()
来源：http://hz.havefunace.top/gtofatwluf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtejajvmhx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ivvv.top/gtsyzurrsp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gtohtyanhe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangtech.top/gtwhgsvelb.html

[L07] 处理 HTTP 状态码
来源：http://hz.vqdsnc.cn/gthswkwrpj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtqiawshav.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtmegthebo.html

JS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gthpdxoygy.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtwppprair.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangkeji.top/gtymwdwhus.html

Go:   resp.StatusCode
来源：http://hz.jlsjyb.cn/gtfwqlolaz.html

Ruby: resp.code.to_i
来源：http://hz.sysykeji.top/gtgajcsgud.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtrcfbtsfu.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtgiqeuvev.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ivvv.top/gtobksyson.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtktuznsdi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtshcpuumw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtpadezygz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydzc1.top/gtopwtbrhd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtkkqxyrze.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gteotojcjf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sufxvd.cn/gtvgssiulq.html

================================================================================
来源：http://hz.yonumen.top/gtpndjzlsh.html

M. 命令行 / 进程 / 环境
来源：http://hz.xinyue.icu/gtcfiwjrnu.html

================================================================================
来源：http://hz.smart0.xyz/gtjxrqcopu.html

[M01] 读取命令行参数
来源：http://hz.52xcode.cn/gtzbnheonk.html

Py:   sys.argv[1:]
来源：http://hz.meibo888.top/gtxxawstzc.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gtnyzggbiw.html

JS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtgdhshyec.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtiuaaclnc.html

Java: args 数组（main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtboiwtmja.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtnsvsxwzw.html

Ruby: ARGV
来源：http://hz.shanyushiyangkeji.top/gtauopaofc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtrfndfsem.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtkgdlmnvi.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gtjgswqwra.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtetjhfjhz.html

JS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtrvluldfb.html

TS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtnzlithrf.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtxvdtbefp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydjk.org.cn/gttzufokpm.html

Ruby: ENV["HOME"]
来源：http://hz.pengpengdd.cyou/gtvqmwplmg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtgexhstud.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtchaeuppk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtpojttnup.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.snrcjt.cn/gtdshxtlxj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtatibmtge.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtedqdgemg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhixingplan.top/gtaxvgmqcq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxinkj.top/gtaioobztp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtsrmjbtdu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtnmunpidv.html

[M04] 获取当前工作目录
来源：http://hz.shzxlz.cn/gtcnsryacx.html

Py:   os.getcwd()
来源：http://hz.dashuyun.cn/gtrzfevldv.html

PHP:  getcwd();
来源：http://hz.birdmap.top/gtzfijtbpe.html

JS:   process.cwd()
来源：http://hz.jianghu66.top/gtvtglsgew.html


<!-- 参考信息 -->