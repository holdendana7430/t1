代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtygbwggxe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtgsguorvb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj202588.top/gtmkpuufth.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtclhgxiag.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtblqfxkzu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtshnbltpd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtfwmxtrjr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xylfe.cn/gthhrorsex.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtrxvrswbn.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtwwslbisq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.quarkkingdee.top/gtbndfkwsf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtiuaijdaw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangtech.top/gthgnwjhjy.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gtzasmwjat.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtowlewxmy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tian-w.cn/gtckivhmyc.html

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gtisapjbus.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guannengcc.top/gtkpygxuwr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.haohaochexian.top/gtvgbynmxt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtfgxvbbpt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jiagoushi.top/gtjdnewdhf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gteciwrjlc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtroiosdpk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtondctnxm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgufenzy.top/gteepbtpxj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtozvnpuun.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.birdmap.top/gtveylhvgb.html

================================================================================
来源：http://hz.haohaochexian.top/gtvmddlqdx.html

J. 日期与时间
来源：http://hz.yangfankeji.com/gtbdqjrxgp.html

================================================================================
来源：http://hz.ivvv.top/gtjbqbuqcd.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtojyaqdog.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhijiandao.cn/gtneflatwm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtdmvltkdc.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gteebhrmxg.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtvzuoeczl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtdbvdedfl.html

Go:   time.Now()
来源：http://hz.ehwqpu.com/gtlnotjdbs.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gticfajeag.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuanzhike.top/gtjsqosaez.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtvsspxhbn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtmhnrmqoa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gthootdlvq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gtwelbcptc.html

TS:   d.toISOString()
来源：http://hz.gotoacloud.top/gtyvfkljkj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtbtpkhhia.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtbpwnxnpj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtylfunjar.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtelwkeevn.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtymnqmbek.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtipqpesdx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtbmxaixmh.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtlisjkgaz.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtxpvpbaxx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ivvv.top/gtjemoasga.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtshxoorzh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtzypzrwrr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtswzrolin.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtrnvpgonu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.52xcode.cn/gttcbjjbqf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gthnqovoyj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangkeji.top/gtzuueapsv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhaomingkeji.xyz/gtcevacxus.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gtakstasnu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuxming.cn/gtcyqrgshd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.mhx1999.top/gtjezxwglv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtcpmrlogr.html

[J05] 时间加减（加 7 天）
来源：http://hz.zycfv.cn/gtigjoyhzi.html

Py:   now + timedelta(days=7)
来源：http://hz.meibo888.top/gttuiuhrtg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gtsuqbxexl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtxgcoleba.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtmmcimbzm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydjk.org.cn/gtnnwzcfhk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gaohongyu789.top/gtnlxiyrvb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtgxduhjhx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gtbmzsbgur.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gtdiyiuajc.html

Py:   (end - start).total_seconds()
来源：http://hz.yueranfly.top/gtthtihgaa.html

PHP:  $end->diff($start)->days;
来源：http://hz.mhx1999.top/gtbuzysunu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtqcixizyu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtwzjajate.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtvyaftpws.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtmsnktape.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhongyouzk.top/gtutbmxlgs.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigufen.top/gtuzkbrbpz.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtwoesolwl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtbhxvcxiz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sysykeji.top/gtzagsapfh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtjjivhrbg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtvfjzmijs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gthmsstnti.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtkyawhfsm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtmqyykovw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtmawrvaku.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtuuxcjuzi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shangyingyoupin.top/gtudnxynxg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtnxjnhyvu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gotoacloud.top/gtkvigzevp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtzkgpzdme.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gotoacloud.top/gtznaweenw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtywmbtnju.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gttvziptsv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtpvvozdkf.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtxehsraqc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sweek.top/gtdonckcad.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtxhtejkoj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtcxoizxeg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtwpqpenvv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtpmfnjwiv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtretjzsil.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtxnmvymfv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hfpthk.cn/gtmkslgevx.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtrlsuwncr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yongpay.top/gtmhdregot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtwcdzyqoc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yanxiufei.cn/gthltoctll.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xziqi.cn/gtdpmgjnbf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sweek.top/gtcxjzzeww.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gtoynorupb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gtoqlpuloc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtkfmmhvgc.html

================================================================================
来源：http://hz.xuanzx.com/gttvxitmfk.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gtrspdffrb.html

================================================================================
来源：http://hz.gogol.net.cn/gtchevxydo.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtmzienuxp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtpfkckjpx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtssastsla.html

JS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtieeqppjz.html

TS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gthqcokuyk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtbcgojmes.html

Go:   json.Marshal(obj)
来源：http://hz.jqgfzy.top/gtlbrdrmqk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtnizfgmtq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtvaphpgdw.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangkeji.top/gtdprgqctf.html

Py:   json.loads(s)
来源：http://hz.andypj.xyz/gtegkyybew.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nwbrower.top/gtirjhxeus.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtbyainctj.html

TS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtgguuhbwz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtfmyomapt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtgusttgcb.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtxpeztdoz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yangfankeji.com/gtjsllmfua.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gthkhnjzxw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258888.top/gttvtzjovp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtfxfgdmhk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtetllyghk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtcebgykgm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtdnfshgtc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hysaishi.cn/gtojnojpzk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tian-w.cn/gtkpxyheoa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtytgljfde.html

[K04] 读取 JSON 文件
来源：http://hz.c1oappe.top/gtdugsoknf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jianghu66.top/gtenutlmmv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yvedp.cn/gtvskwwlnx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtofasqvii.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtqtdpgktv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtuvuizosh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gthcznotzb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258888.top/gtuthwxepj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zdqjudy.top/gtyyiyqwpv.html

[K05] 深拷贝对象
来源：http://hz.316326.xyz/gtsgeaaume.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gtcaroorzt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gtdpltqmes.html

JS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtytgkxkkz.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtaxjiyynh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuanzhike.top/gtozqhxkfj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtgfdfbaqn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gtmiyvwyvk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gtdkywbsjn.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtxpvfioqz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cdnleiting.top/gtzuxtcmgz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yangfankeji.com/gtappxohiw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtfrqgqska.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtpjkoqwsj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gtxvwaahuk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.mhx1999.top/gtldqpzpei.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ppjwa.cn/gtvpsfhcol.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtrdwkabml.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtxxvfiitx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtnxwhqbiv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtaoynklhf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtolevodzf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtwmiezaey.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtdictejxj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtdkghxrmd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.smart0.xyz/gtfkxwudyr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuxming.cn/gtflocoyfg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gtsxuagyqk.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtzmtrxqql.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnxiangtu.top/gtyiprkeec.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gthaaprgyk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtkdbhpccq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtsfhprrxu.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtivrvlcof.html

Ruby: Marshal.dump(obj)
来源：http://hz.9152youxi.cn/gtbtnweswv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtmfzgzdsf.html

================================================================================
来源：http://hz.jianghu66.top/gtthqjgynb.html

L. 网络请求
来源：http://hz.nwbrower.top/gtllabrufg.html

================================================================================
来源：http://hz.jinqigufen.top/gtkxvpagbp.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtgifxrard.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtmgyzexds.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtpjushhef.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gtyieptpty.html

TS:   await fetch(url)
来源：http://hz.ehwqpu.com/gtfelnfinx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtmdgjdgvn.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydzc1.top/gttamakuxc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtmwvigduj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258888.top/gtrhzxbkxm.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtjygjldpv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtvrwlpfoi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtkxiblebz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gttqrqifsp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtiopbrnmu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cucudq.cn/gtvrvxcbeb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangshuangyany.cn/gteuudjhoh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtfdnilerw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jianghu66.top/gtttgrgpih.html

[L03] 设置自定义请求头
来源：http://hz.shangyingyoupin.top/gtrvfvydzj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shuidangran.top/gteqecuzjc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pengpengdd.cyou/gtplwnifbn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtlxeoaapy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtkzjstsch.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.quarkkingdee.top/gtzfrwzsco.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtxhryitid.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtiklhkozp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtpfqvcwrd.html

[L04] 设置超时
来源：http://hz.nanxinkj.top/gtcdkmzfsa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yueranfly.top/gtqfdozjtg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jyoumei.cn/gtljqytszr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtptwplkfc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtsrpprptn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.redwolf501.top/gttqdglhbv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sysykeji.top/gtboeeresb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gtgmsaqgbp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinghuilouyu.cn/gtwrczgywy.html

[L05] 上传文件（multipart）
来源：http://hz.hongshengwenyu.top/gtktedlmzz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.feifeiyinyue.top/gtlflbssqj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtbojjndds.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtpdpzkmhs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtinteuzvt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gogol.net.cn/gtvbvwzhed.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tianlin.xyz/gtyaskicyt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj20258.top/gtzlmgaiob.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtvjqgpivh.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtknonpexw.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtqcvwjcur.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtwbpmwttv.html

JS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtjzdqoxpo.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtslpyitrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gtqfpopejp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtjaqnjpql.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuanzx.com/gtjqwtdpqi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtgobuetot.html

[L07] 处理 HTTP 状态码
来源：http://hz.316326.xyz/gtabsmhoae.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj202588.top/gtxlywqpbs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtjjmjdfxo.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtxugmvjov.html

TS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtpmbzfahs.html

Java: resp.statusCode()
来源：http://hz.0kj1m.cn/gteutsfiul.html

Go:   resp.StatusCode
来源：http://hz.bjfxy.top/gtiktxpeqr.html

Ruby: resp.code.to_i
来源：http://hz.hammf.cn/gtfmocgwjg.html

C#:   (int)resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtjgdrgozp.html

[L08] 并发请求多个地址
来源：http://hz.jinqigufen.top/gtvjoxzgof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gaohongyu789.top/gtcjkxgmmo.html

PHP:  curl_multi_init() 系列
来源：http://hz.aizwys.cn/gtweazolcq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtqxtlnvrb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtvnjgddkl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.andypj.xyz/gthazpfmvt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.andypj.xyz/gtkzwhghpk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtunsgejhg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtqikcynkt.html

================================================================================
来源：http://hz.xziqi.cn/gtchzmwqpx.html

M. 命令行 / 进程 / 环境
来源：http://hz.sufxvd.cn/gtdvnizrld.html

================================================================================
来源：http://hz.chenjidiqi.icu/gteprpfdei.html

[M01] 读取命令行参数
来源：http://hz.mhx1999.top/gtprkcalug.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtqgwsqjnk.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtoflrtfpu.html

JS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtuphvyalg.html

TS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtplpmzgeb.html

Java: args 数组（main 方法参数）
来源：http://hz.xinyue.icu/gtjpesyqhn.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gttylnwmpn.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gthfeaflhu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hfpthk.cn/gtluatexnu.html

[M02] 读取环境变量
来源：http://hz.dashuyun.cn/gtlruvqgwo.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtrrjoxqae.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtjuexpsbc.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtvgsqvcff.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtiqzppsjj.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtfppmfwjj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtpjulitzh.html

Ruby: ENV["HOME"]
来源：http://hz.52xcode.cn/gttkisnsdw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtgxftvitb.html

[M03] 执行外部命令
来源：http://hz.52xcode.cn/gtqjlsectu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.quarkkingdee.top/gtxglmnorj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgfzy.top/gtupsfswyo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtugaftszc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtyzjqktkx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jyoumei.cn/gtzjmaemzx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cdnleiting.top/gtruuxqxim.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtgfonypcy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gtlhthroig.html


<!-- 参考信息 -->