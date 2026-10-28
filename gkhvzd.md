代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sxryk.cn/gtdlooslwg.html

TS:   /error/gim
来源：http://hz.hywenlv.cn/gtalgfmean.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtldznpzld.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenlongwang.top/gtboribvwd.html

Ruby: s.scan(/error/i)
来源：http://hz.hongshengwenyu.top/gtuxwkcxbf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gtqqltrbzw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhaomingkeji.xyz/gtmitjhldw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuanzx.com/gtvgnhmdbn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtqduqcjxi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtzveeqvfr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtffykuagt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtulnlslkg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtipghvwem.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangdashe.top/gtdopzyfjr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtpokcueal.html

================================================================================
来源：http://hz.sysykeji.top/gtfjorsuco.html

J. 日期与时间
来源：http://hz.ivvv.top/gtwwqzndtl.html

================================================================================
来源：http://hz.smart0.xyz/gtzstfxlow.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtljaengsj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtsctmkjoz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gtrllifdxz.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtnoqczekv.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtzojamzom.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhongyouzk.top/gtiwyjuubb.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gtkcaxntie.html

Ruby: Time.now
来源：http://hz.yuanzhike.top/gtwlnvygbo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtfekpewkv.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtvewmkglb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtchkeolue.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtcgrjkkxl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cqqwz.cn/gtehjxmkua.html

TS:   d.toISOString()
来源：http://hz.nanxinkj.top/gtpdwjurub.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zycfv.cn/gtujjictvh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.c1oappe.top/gtvenlslhz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtkrbladle.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtqnhncbrz.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtfaqbugrv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jiagoushi.top/gtoogmykyj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.meibo888.top/gtctjtodld.html

JS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtszcckocd.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtllfuoyvc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtovsfoqjo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtrjioedmi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtseaixpap.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtpkidtprf.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gtsrgjganv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.feifeiyinyue.top/gtybbzmcla.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgufenzy.top/gtqwsewibv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yvedp.cn/gtvxionpms.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.bjfxy.top/gtbagrpxfz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dianchejie.cn/gtxcpyvysy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.haohaochexian.top/gtdseipizp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.havefunace.top/gtwocokgkw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gtnojvzqwd.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenzaomai.com/gtoszjzdgv.html

Py:   now + timedelta(days=7)
来源：http://hz.dianchejie.cn/gtifawuyfk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnqzz.top/gtzsarhqbs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtkmktqbfx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gttbhemqqk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.smart0.xyz/gtusjostxv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gtxtywdqxz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hfpthk.cn/gtmwmhmuwg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangdashe.top/gtluyssbwr.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtvbtrkesu.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtjxtgifhs.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtglliutox.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gogol.net.cn/gtjhqytvul.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gtjfyeqczf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jiagoushi.top/gtyjirhhie.html

Go:   end.Sub(start).Hours()
来源：http://hz.snrcjt.cn/gtkgwprmhe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cucudq.cn/gtxfofgmzt.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtzgdizfub.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gteoovmrqj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtcvvhzyql.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtevihmmsp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtvqdiyank.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtjocramth.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cheryme.top/gtfmacgilr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnqzz.top/gtrfkcdeco.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtkjlxncbc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gttolocmbg.html

[J08] 提取年月日与星期
来源：http://hz.quarkkingdee.top/gtwyotzpsc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shuidangran.top/gtjtjzzuif.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fengsongda.top/gtymqrznpy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xylfe.cn/gtibfhppht.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtegbnotgk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gthftenzky.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtbqpjftxo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtpkdfgrml.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gthpeaerbu.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtplaqwfwx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gttplokxno.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtuaideqef.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtvjxpblbs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtiutvihps.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtrunlubip.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.snrcjt.cn/gtwjyigasl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtppczbjgr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtncigpfwr.html

[J10] 取今天 / 本月第一天
来源：http://hz.cqqwz.cn/gtlbqposuf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtmmufcitq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aizwys.cn/gthvrnzrtf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dashuyun.cn/gtbrasgqqv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gtxmugzoht.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gtnsnkmjgo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtpirrygqg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.iojbl.cn/gtlpcplryc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sxryk.cn/gtxeydxghy.html

================================================================================
来源：http://hz.quarkkingdee.top/gtplpvwaaa.html

K. JSON 与序列化
来源：http://hz.gaohongyu789.top/gtrtngqtxr.html

================================================================================
来源：http://hz.jinqigufen.top/gtiuwkrftg.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangkeji.top/gthblxownr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhongyouzk.top/gtpkrrtkci.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtkwqxurow.html

JS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtyvgviily.html

TS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtxdbgyddw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnqzz.top/gtymvctfhk.html

Go:   json.Marshal(obj)
来源：http://hz.yanxiufei.cn/gtemfmlubs.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydzc1.top/gtcfowwwma.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.andypj.xyz/gtmievlojp.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gturlkzqdu.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtcmaucxin.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xinyue.icu/gthkmrmzwo.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtbyavchwx.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtkwjouoly.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yangfankeji.com/gtuwsvvqrv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtsxwaznuk.html

Ruby: JSON.parse(s)
来源：http://hz.yongpay.top/gtfrxiaaqo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtwomrwrqz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtzfkkcnmu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtqudvwood.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtewtkvegr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtftjilcsb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtkumnrxim.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.52xcode.cn/gtyovhedgw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gtpofjqdne.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtctcyozto.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gtelbhgmoa.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gtjolgdhvk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ppjwa.cn/gthrfwxhss.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtnntfpbhd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtggxuoiqn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydjk.org.cn/gtlcbhvwlw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gotoacloud.top/gtcoxntiow.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtuktdichs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtkxhiqmgi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cheryme.top/gtlnjnlvil.html

[K05] 深拷贝对象
来源：http://hz.chenjidiqi.icu/gtfrkipgme.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhengqikj.top/gtluqpfuln.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aibaodan.cn/gtpdrrbqqs.html

JS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtqfdychad.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtqnfzpoef.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.0kj1m.cn/gtxhpgpkdv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtulyftjoj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhiwuduotai.top/gtdjbgvamx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gtrympzovr.html

[K06] 解析 URL 查询串
来源：http://hz.haohaochexian.top/gtxpzgxkiu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydjk.org.cn/gtdfopjqwn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigfzy.top/gtmuaejlys.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtbwurbapt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtsosjquhf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtmjvpifwq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtvfqphfbf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtofhsdbjy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtaylizzwa.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtrdkubsuy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cheryme.top/gtptbcpjjr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtauwairyj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtjngfdfsh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtuubpakdl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangdashe.top/gteqvmizgj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtilmkftrf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ybcxt.top/gtytkfqlcy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.mhx1999.top/gtkeswapxk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.andypj.xyz/gtleczuprt.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtbeuylbio.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtgxytdmhh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtkvqtreuz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtxuadhrfs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhaomingkeji.xyz/gtbtzfcagu.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtmwrvaquj.html

Ruby: Marshal.dump(obj)
来源：http://hz.yvedp.cn/gtaxalaqef.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuanzhike.top/gtuvausvrj.html

================================================================================
来源：http://hz.guowangkeji.top/gtbwecaesd.html

L. 网络请求
来源：http://hz.jiagoushi.top/gtdesvboll.html

================================================================================
来源：http://hz.ehwqpu.com/gtibqbccpy.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtocvdsudo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtiqbkoczy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jyoumei.cn/gtkramqkte.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtehvgwnwe.html

TS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtbjzobcmi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fzhhl.top/gtjstrxxsu.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtdxpinjid.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.haohaochexian.top/gthitgrdru.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gttwrqkzmk.html

[L02] 发送 POST JSON
来源：http://hz.ydjk.org.cn/gtqkimhwry.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.316326.xyz/gtmszadrbm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtlleipgyh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.kuanghao11.cn/gtpwzmvzic.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtdlhqoodl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtogcewnhg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj20258888.top/gtvcvuejea.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zycfv.cn/gtsbtbieom.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.52xcode.cn/gtykinlyyx.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangtech.top/gtoyqptmbs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtzvrphrxs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gthtbvkyfq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtyirjlqvd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gttmbstdas.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtkiiwmoxh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtprdfozze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtvbinnxbb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtnostpsjd.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtuigvkbvm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aizwys.cn/gtdlfevntc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhoulong.xyz/gtkkkdkwrc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtrwspnkth.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtniatnavs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtmmkocyow.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangkeji.top/gtbsibpxhf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gzhubu.top/gtrqsreiih.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tanke756.top/gttttehbbd.html

[L05] 上传文件（multipart）
来源：http://hz.cheryme.top/gtgnmpwktw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sweek.top/gtokpboqih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtmyyhmpox.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtapdgmqxf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtypffzffp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yongpay.top/gtiwmgxefh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hammf.cn/gtfcfzcsxf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtsnauqkbh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtkqwshcav.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtyootjdfi.html

Py:   resp.json()
来源：http://hz.yj20258.top/gtqhlfohfe.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtmhxawefo.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtnpuiolyg.html

TS:   await resp.json()
来源：http://hz.bjfxy.top/gtvrtwnokt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fzhhl.top/gtlmyjkaua.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hammf.cn/gtydckjbjo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jianghu66.top/gtufynbyug.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuetiantiany.cn/gtnhiymyms.html

[L07] 处理 HTTP 状态码
来源：http://hz.dianchejie.cn/gtisbtoswi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtklpxhvcd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtrrltcror.html

JS:   resp.ok;  resp.status
来源：http://hz.jiagoushi.top/gtpvjjjbwd.html

TS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtkqjikhob.html

Java: resp.statusCode()
来源：http://hz.zhaomingkeji.xyz/gttmcpankv.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtyytvurdv.html

Ruby: resp.code.to_i
来源：http://hz.yvedp.cn/gtnrjllvmj.html

C#:   (int)resp.StatusCode
来源：http://hz.zhixingplan.top/gtvahzeuyb.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtzlvveuin.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pengpengdd.cyou/gtkunqgkpq.html

PHP:  curl_multi_init() 系列
来源：http://hz.yonumen.top/gtljjiswak.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtmvxhjmxe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtdmqmxhhg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnqzz.top/gtosrjogis.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtyxraamsu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtydaajkql.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gtwdxswjwi.html

================================================================================
来源：http://hz.sufxvd.cn/gtfmytqzxo.html

M. 命令行 / 进程 / 环境
来源：http://hz.daxiang520.top/gtcgbhfrpl.html

================================================================================
来源：http://hz.ehwqpu.com/gtstgixnqy.html

[M01] 读取命令行参数
来源：http://hz.yvedp.cn/gtieoiveal.html

Py:   sys.argv[1:]
来源：http://hz.316326.xyz/gtrzunnmxr.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtgrmdpryz.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtzrroonvn.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtbxqnankd.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gtuuzygtag.html

Go:   os.Args[1:]
来源：http://hz.bjfxy.top/gtfbjhecvt.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtxexazsop.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtwrfphved.html

[M02] 读取环境变量
来源：http://hz.nwbrower.top/gtkfjuqorb.html

Py:   os.environ.get("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtahaivkci.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xylfe.cn/gtfxmcufhz.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtrnqshzef.html

TS:   process.env.HOME
来源：http://hz.yj20258888.top/gtgyfnlbyx.html

Java: System.getenv("HOME")
来源：http://hz.yanxiufei.cn/gtxnfmsupb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtubwzovlc.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gthqsdfjgn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtyyfxzjfk.html

[M03] 执行外部命令
来源：http://hz.vqdsnc.cn/gtfqxrcljr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnqzz.top/gtbwbyasxg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gtuqpnxvip.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtqkskwdiu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnqzz.top/gtyxfmsamh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.quarkkingdee.top/gtngdtvasn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydjk.org.cn/gtswaauotr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangkeji.top/gtkmtpcgqy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtlmblkuxq.html

[M04] 获取当前工作目录
来源：http://hz.yvedp.cn/gtoopytlro.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtqockxput.html

PHP:  getcwd();
来源：http://hz.tian-w.cn/gtfalmizwf.html

JS:   process.cwd()
来源：http://hz.haohaochexian.top/gtrtsekudw.html

TS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtujmztenq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ppjwa.cn/gtcvjpbxfn.html

Go:   os.Getwd()
来源：http://hz.0kj1m.cn/gtyjzvtpvm.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gtythtbhkw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.0kj1m.cn/gtclmexdiz.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtkpmywonx.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtvdopxwyd.html

PHP:  exit(1);
来源：http://hz.xuetiantiany.cn/gtkplxghzj.html


<!-- 参考信息 -->