代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtosvlbxof.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.andypj.xyz/gttyjthwuw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtcztihaiu.html

[I05] 按正则拆分
来源：http://hz.kuanghao11.cn/gtrwrxfjrt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenzaomai.com/gtymyltnme.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.aizwys.cn/gtbmbwfloz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtbgtdeglm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtesuggcjs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gteivzywoc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtmiygkdbt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtnnuujlax.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuxming.cn/gtlamwjlby.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtfqqpnmmr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gthpniixpr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xinyue.icu/gtcsmtmfyd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtrerybjik.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtczaktdna.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hysaishi.cn/gtbodyfmib.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cqqwz.cn/gteoobggsg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydzc1.top/gtnnpfijnu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtwzbntnxw.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtakwqyjag.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cheryme.top/gtzalsdwja.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigfzy.top/gtaizimpea.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtppzetoqu.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtunqvcvfk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gteuwkdtlu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gotoacloud.top/gtabtgouqt.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gtkaufursq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.vqdsnc.cn/gtkynmnijt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtqlslvqna.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtipgadrju.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhengqikj.top/gtzdtmekuq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtmculhizq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtnmucfxzn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtaqidtxts.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtqysfoesp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gttvmbtdsh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtjlddofvl.html

================================================================================
来源：http://hz.sufxvd.cn/gthwzwlpyh.html

J. 日期与时间
来源：http://hz.hysaishi.cn/gtpeygswui.html

================================================================================
来源：http://hz.hnqzz.top/gtczkkxwtv.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtwglvqxbq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtnpwadnvi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtwgvjvluw.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtlrijzudr.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtnycrtzty.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtiqrthpsu.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtatwlsosp.html

Ruby: Time.now
来源：http://hz.jiagoushi.top/gtilejutuv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.redwolf501.top/gtyfemblue.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gtpbiqchis.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtoclbummu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtccazrouu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtzdbsshnm.html

TS:   d.toISOString()
来源：http://hz.xingfuxueyuan.xyz/gtxivshurh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtpjxnavbg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtyxmzkkvz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtqehuflbk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtgqdwndhs.html

[J03] 字符串解析为日期
来源：http://hz.hysaishi.cn/gtamyljqph.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtumzhjenx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daxiang520.top/gtqlvqycag.html

JS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtetbhmcdo.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtwbsuqcft.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtzrecxfvf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtmhoqazzs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtupqbrfnd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.birdmap.top/gtcmplzvgp.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtvenreopm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gtfbbejjdz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangkeji.top/gtifdfehdb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zycfv.cn/gtdxrpyokh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangkeji.top/gtwuhkqgsx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtyjwpskqy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtwtdslpjo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hammf.cn/gtugdyobku.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gthkvyonpy.html

[J05] 时间加减（加 7 天）
来源：http://hz.cqqwz.cn/gtpkozdpfu.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtoleuskzc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gthlqhkvta.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtqjjltjbf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtlklaxcoh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gtdzgbchne.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnxiangtu.top/gtqifdgrjd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenjidiqi.icu/gtdwexqzhb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtiwdijqzv.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtnvnnhlzm.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgfzy.top/gtzxznszkr.html

PHP:  $end->diff($start)->days;
来源：http://hz.iojbl.cn/gtiawkmuor.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yanxiufei.cn/gtbckkilsp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtwmckidyk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangkeji.top/gtbrdwhdnr.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gthdirzkts.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtsvpccyzz.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtwiahrjnu.html

[J07] 比较两个日期
来源：http://hz.aizwys.cn/gtuwsvvuqk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtluscbqnm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtvzicyjlk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gtrynlvswb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtnhzplvvg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtvoauggth.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.52xcode.cn/gtqocquywi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtdxhvmflw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtarodauio.html

[J08] 提取年月日与星期
来源：http://hz.chenlongwang.top/gtuaryftkk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gthcwphkvr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gaohongyu789.top/gtxxjpshom.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgufenzy.top/gtyohipruo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtbutscyuf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtouiqhclf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtumuofbec.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtnfmojszp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtzvofyaue.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtfpopdudh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtjqiwijoc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gtlcjralej.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtnbzkuocd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtsnqkteqq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinghuilouyu.cn/gtatksbzmx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtoivwfqjp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.smart0.xyz/gtrjmemake.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.c1oappe.top/gtrciohtko.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gttxckbydk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gtzmfbfpxm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gtvpepqrvg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.mhx1999.top/gtgeesmype.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtqorfmsdj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cheryme.top/gtuyiiiomc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangtech.top/gtetroaewx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtgmmwnhko.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtlyktmppp.html

================================================================================
来源：http://hz.zycfv.cn/gtgqigletn.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtriwrnnim.html

================================================================================
来源：http://hz.tian-w.cn/gtfxqvothb.html

[K01] 对象转 JSON 字符串
来源：http://hz.yanxiufei.cn/gtxplfsnbp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtbosydxmx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gthwkbjrzx.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtgtbqhuth.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtvzksguwa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtjgyqymrl.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtzdgarimb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.0kj1m.cn/gtzlxoykxi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtgtvpyvln.html

[K02] JSON 字符串转对象
来源：http://hz.gotoacloud.top/gtxojrnfpz.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtapgazzqp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.quarkkingdee.top/gtrhoozeov.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtmzaidfle.html

TS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtncrndwxz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtdcfqxdho.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gteclnxdfa.html

Ruby: JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtdtvmlfxc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jianghu66.top/gtuhmffrti.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuetiantiany.cn/gtctoinbio.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtikpfxmtl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtukivbtfs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtexeottqz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtcgzlopnb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydjk.org.cn/gtndmrozrl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258.top/gtyumhwnps.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.9152youxi.cn/gtnhqkejtv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtffivhjah.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtyqltvqkm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtksudqekh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtwaanuhmp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtivfrpmuj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtokdwzjfo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aizwys.cn/gtayypldhd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgfzy.top/gttxqpxdzp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtjdctgxto.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yangfankeji.com/gtcblglbsd.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtylobeovv.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gtejqmzbbx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daria6918.cn/gtivhqmwrw.html

JS:   structuredClone(obj)
来源：http://hz.sufxvd.cn/gtsvcbqshy.html

TS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtfivvmmbi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dashuyun.cn/gtakbemisq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxinkj.top/gtyaeiqtby.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtnayldogb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtxvospwbd.html

[K06] 解析 URL 查询串
来源：http://hz.316326.xyz/gthzgmimef.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.meibo888.top/gtrcabpkhj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtcokofusc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtydfikjah.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtbethzodb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtyhgoyfob.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtgjfuervr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gthnirsphk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jyoumei.cn/gtpzanrlsd.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtpspeqemd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.vqdsnc.cn/gtarlptfdf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtqzuqtepo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtmcwxilnb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtegddhwnr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtawjcaioz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgufenzy.top/gtxsnkqioj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtclhikzxg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gtzvdpjdsv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtzryojrmi.html

Py:   pickle.dumps(obj)
来源：http://hz.quarkkingdee.top/gtcrnjytlp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gtwuxbzyew.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtmudezlnt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtphngyguf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cheryme.top/gtzwyfnzbh.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gtcyiedseo.html

Ruby: Marshal.dump(obj)
来源：http://hz.xinyue.icu/gtortjnajb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtfotdpmwp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwitzrcvl.html

L. 网络请求
来源：http://hz.yj202588.top/gtrfcqcels.html

================================================================================
来源：http://hz.xziqi.cn/gtindzpguy.html

[L01] 发送 GET 请求
来源：http://hz.xylfe.cn/gttffcznyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtsmsuoomx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtpeuoephf.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtynooaaxx.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtziuzifqh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuetiantiany.cn/gtgrvgfsxr.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtfvnzzhhn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.52xcode.cn/gtivqpsxik.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.haohaochexian.top/gtytuxxoxw.html

[L02] 发送 POST JSON
来源：http://hz.sufxvd.cn/gttrtsorps.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.iojbl.cn/gtsrwdjubb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtpyarsvgt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtppmrixnt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtelvwrpso.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nanxinkj.top/gtdappynqw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hywenlv.cn/gtdofhpcvw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnqzz.top/gtkzgwstnt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shuidangran.top/gtsnoayoiv.html

[L03] 设置自定义请求头
来源：http://hz.tianlin.xyz/gtalzfpdli.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtrfmwyhhy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhijiandao.cn/gtorzuvdeb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtfhchjuxo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtkgyfnlep.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ppjwa.cn/gtfxbplkil.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tian-w.cn/gttwxkrpef.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtagajskqw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gtilnkokwk.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gtkhdllwrv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.redwolf501.top/gtfzwhlghc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtcsjutmsi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtjrckmnea.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtzsmpzpjn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gthqsstuvr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aibaodan.cn/gtgnuxjwwm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ivvv.top/gtrpodqxum.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtoljtjoyw.html

[L05] 上传文件（multipart）
来源：http://hz.svipenyu.cn/gtktpzmqfg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ywan-chungtsiang.top/gtuupukbel.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gaohongyu789.top/gtmsraubja.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtigfzfxfk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtymsjvqpp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.feifeiyinyue.top/gteochwewh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gtxyutblee.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.9152youxi.cn/gtkygoepyw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gtnznvctst.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtpbnbeqrm.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtpfxomqjd.html

PHP:  json_decode($body, true);
来源：http://hz.yongpay.top/gtggtzrasr.html

JS:   await resp.json()
来源：http://hz.fzhhl.top/gtnnzlnuqi.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gttdfpnups.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtfvcvyudm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yvedp.cn/gtgorageha.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nwbrower.top/gtdfqolxbi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sufxvd.cn/gtsadvvqaj.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtgdytwgla.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ehwqpu.com/gtacbujtzu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtfcolobzf.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtmjvikjpp.html

TS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gthtrypaul.html

Java: resp.statusCode()
来源：http://hz.havefunace.top/gtplhylqjr.html

Go:   resp.StatusCode
来源：http://hz.aizwys.cn/gtslzpxngo.html

Ruby: resp.code.to_i
来源：http://hz.daria6918.cn/gtivpobtoi.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtsmyledsw.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtvclcdiml.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.vqdsnc.cn/gtyduguyow.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuxming.cn/gtieshsfab.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtfypthroi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtzwskroom.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tian-w.cn/gttxfylvfe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtqdozviwe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gtgtzdembf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtwswccfnh.html

================================================================================
来源：http://hz.sufxvd.cn/gtsvdhcohv.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gthyjhtgrs.html

================================================================================
来源：http://hz.ehwqpu.com/gtfiaqhtzs.html

[M01] 读取命令行参数
来源：http://hz.jiagoushi.top/gtgoszseqh.html

Py:   sys.argv[1:]
来源：http://hz.9152youxi.cn/gtbikishiu.html

PHP:  $argv;  $argc;
来源：http://hz.yangfankeji.com/gtrstvytsc.html

JS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtbnsnvwsd.html

TS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtkgdgziqp.html

Java: args 数组（main 方法参数）
来源：http://hz.ydzc1.top/gtlbbdydep.html

Go:   os.Args[1:]
来源：http://hz.gogol.net.cn/gtqjhexmem.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtqktjjzhz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gzhubu.top/gtsqjiqkzr.html

[M02] 读取环境变量
来源：http://hz.dashuyun.cn/gtpaptfgnz.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gtrwnqnoxd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtlwrjemjp.html

JS:   process.env.HOME
来源：http://hz.mhx1999.top/gtssmfnanf.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtwfqjqsdz.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtjqxnsitz.html


<!-- 参考信息 -->