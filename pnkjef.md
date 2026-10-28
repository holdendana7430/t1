代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtkxuywuwm.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtbvdwbtkp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gtrnstiwvm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hysaishi.cn/gtporobshw.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtoafdhcez.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtzbzroyeq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtlypueldd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtpkwqtkwg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtxpcnpybn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtuiifythv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtkmcdnjvt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtvbcbzksw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gteaxeyguy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtljfqovig.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gtpjnlopea.html

================================================================================
来源：http://hz.jlsjyb.cn/gtqsvcikdb.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtlcdrndcb.html

================================================================================
来源：http://hz.guowangkeji.top/gthnszkedv.html

[J01] 获取当前时间
来源：http://hz.zhiwuduotai.top/gtvftjgrkf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gttalgjanl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtokggocpw.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gteqfrxevc.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtbthinwqz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtysdqefjs.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtjokgadbc.html

Ruby: Time.now
来源：http://hz.ehwqpu.com/gtpwslulqj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtigxfqodo.html

[J02] 格式化输出
来源：http://hz.ppjwa.cn/gtsjkllunz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtwveoxlat.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtqjwfofgw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.kuanghao11.cn/gtwceqkwzh.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtwuthziew.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cheryme.top/gtpvxxiewf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtitpvkksb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtowxixyqz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shangyingyoupin.top/gtdeufmczs.html

[J03] 字符串解析为日期
来源：http://hz.quarkkingdee.top/gtycbrsmzz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtkgutjxkw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gtuvyxegjv.html

JS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtczeznprm.html

TS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gthmnabgnp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sweek.top/gtwizwkdop.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnqzz.top/gtditzkrvo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtxexvzsja.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtaqvmbhcj.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtsqlxqnmx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cheryme.top/gtljjjfsxs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtbbfhqyvj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daria6918.cn/gtbpjokkcm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gotoacloud.top/gtiurbrxyz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtnulwytrs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtsmhyzlvh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtbzuanghh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.aizwys.cn/gtvnqbpahm.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenzaomai.com/gtxpmsxvao.html

Py:   now + timedelta(days=7)
来源：http://hz.aizwys.cn/gtdqfbraoa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shzxlz.cn/gtiyaxmrcq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtyekmiygf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gthqvtlode.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydzc1.top/gtrasufoql.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtgbhustor.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtwpuhokcm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.bjfxy.top/gtgcaixyla.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtiulfbyos.html

Py:   (end - start).total_seconds()
来源：http://hz.yuanzhike.top/gtgiagiafl.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtudmtvnez.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gtldinckzv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gtkllalwmi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigufen.top/gtngizjtxl.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtxanvsvpl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gteroxheph.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gthlimeiqz.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtpadaokrc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtkggqhafu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gtahhtdbkp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtsivybuvd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtuqwynzku.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtngifnmfj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xylfe.cn/gtptpaqjux.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtneopjxst.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtvtiueeya.html

[J08] 提取年月日与星期
来源：http://hz.gotoacloud.top/gtrdsjvmga.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtfmidbuvb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtwfegnmzb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ivvv.top/gtvcdzvzzt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cqqwz.cn/gtpwajjmru.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtgexizyvu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigfzy.top/gtkujzgwvv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtmmkybqre.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtcqvkvhjc.html

[J09] 时区处理
来源：http://hz.svipenyu.cn/gtgiancthi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtcnnomsdl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shangyingyoupin.top/gthwwtapgr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtxmvzjpmr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtecvwdles.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhongyouzk.top/gtxvnulskb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtxzavhqse.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtmzecfgmn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dashuyun.cn/gtsgoprerk.html

[J10] 取今天 / 本月第一天
来源：http://hz.jyoumei.cn/gtgexxtmrw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtzjwiirhu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtbclhjghn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtmxbpwfvz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xylfe.cn/gttnsrxkcp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtilbjvoik.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aizwys.cn/gtoyiakalr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangkeji.top/gtbaymmwjh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gthncsdbpy.html

================================================================================
来源：http://hz.tian-w.cn/gtsprferdm.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtmochissh.html

================================================================================
来源：http://hz.ehwqpu.com/gtqkplyllg.html

[K01] 对象转 JSON 字符串
来源：http://hz.xziqi.cn/gtuwrnrzoj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtrliisubb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtxcuwvdyt.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtqkrjtmce.html

TS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtkdklyrow.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtncmhbvxv.html

Go:   json.Marshal(obj)
来源：http://hz.chenjidiqi.icu/gtgfvcotwq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhaomingkeji.xyz/gtspbrmclq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtwykmjngb.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtqdyxngpv.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtmmfqwlxf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.9152youxi.cn/gtlamdbvzj.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtopglyxub.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtlhjfpjhr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jiagoushi.top/gtehvydlfu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtfwjtgefp.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtyjerwmid.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhiwuduotai.top/gtlmkkcbmf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtgsrbsuww.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtarhwvams.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtcxplawef.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtlqqpqfpn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtsauzivub.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhongyouzk.top/gtciblusog.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gthhnvfhyb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hfpthk.cn/gtophunfxe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtvtodjdzm.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtzmudtxzc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shuidangran.top/gtewsqgqrv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtxhvywzai.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtxyrhwtsp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtdygaufny.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gtgndnlcui.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtrqzmsvxx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtvnrinakw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hongshengwenyu.top/gtysvrtddy.html

[K05] 深拷贝对象
来源：http://hz.cashguo.top/gtywvnissi.html

Py:   copy.deepcopy(obj)
来源：http://hz.cashguo.top/gtulmussyc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtqdenopsl.html

JS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gttrdmbeyw.html

TS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtzhsxwqxf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ppjwa.cn/gtihfhygfj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtagwshnuu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jiagoushi.top/gtplrqcbhu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aizwys.cn/gtxqdorddz.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gttpswmzjj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gtbpbflqlp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gogol.net.cn/gtcmsarupi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtenyhxrqi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtsvcbldzi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtpxpvfkns.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtuseuggrl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daria6918.cn/gtcxgogebf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtxzponyiv.html

[K07] 进制转换
来源：http://hz.yonumen.top/gtqnwuvdqc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtqeyhohyr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtlxxadcio.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtwjzbaepx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtssoyruov.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtxzvtlhhu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtlzlrlgan.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hysaishi.cn/gtsnqolncu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gttyrqcotl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtyaxarlsc.html

Py:   pickle.dumps(obj)
来源：http://hz.bjfxy.top/gtxraiyhfn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gtlgvcdeqe.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtlohvqpgt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtwzlhpzos.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinghuilouyu.cn/gtjxtrulug.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtdjfrzijl.html

Ruby: Marshal.dump(obj)
来源：http://hz.hysaishi.cn/gtclqswgvw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sweek.top/gtrdpraqob.html

================================================================================
来源：http://hz.cashguo.top/gtqnojsygs.html

L. 网络请求
来源：http://hz.guannengcc.top/gtzwqezbjf.html

================================================================================
来源：http://hz.haohaochexian.top/gtkrhvgloo.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtkoruiigc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgufenzy.top/gtqprfcgho.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gtayyixynd.html

JS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtrvxgpjca.html

TS:   await fetch(url)
来源：http://hz.zycfv.cn/gtqayoouxs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtpcnwpvun.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtapqcsvbf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tanke756.top/gtbidueasf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtvbuiaowc.html

[L02] 发送 POST JSON
来源：http://hz.xuanzx.com/gtutayqrtm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.redwolf501.top/gtxeuttvxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtdadlfkfk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtlnpjhlcc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tianlin.xyz/gtaaztpnla.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtvoigxbue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sufxvd.cn/gtyyjjivwb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yvedp.cn/gteneewzll.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gtkcsdjviv.html

[L03] 设置自定义请求头
来源：http://hz.tianlin.xyz/gtdfwyilud.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gotoacloud.top/gthadbcwnu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtssiakcxl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gtudbwaits.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtubfqvvlk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtyiscgarr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtplhilxte.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtmfnjqlbv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gzhubu.top/gtwykjzssn.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtzuqcxohu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtdixmvtim.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xingfuxueyuan.xyz/gtfljhffqg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtsyfgwadt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtxlstyxxw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gotoacloud.top/gtjbjmhlqm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtdddxoyph.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhixingplan.top/gtcfapsjrg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hammf.cn/gtnzdelcqw.html

[L05] 上传文件（multipart）
来源：http://hz.jianghu66.top/gtjpfprpwx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pycfn.com/gtyxibvptu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.quarkkingdee.top/gtavkpuuev.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtfwqvsuju.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtstgohhzt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtyekdxidq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aibaodan.cn/gtvvtzbkzo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtypclyzgi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gthqkplsxl.html

[L06] 解析响应为 JSON
来源：http://hz.jqgufenzy.top/gtahzwdazi.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtkyslspgo.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtbypdgdeb.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtqfcpeqao.html

TS:   await resp.json()
来源：http://hz.zhixingplan.top/gtsfwkjycu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtuzhthnbf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aibaodan.cn/gtkhvdglpp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.quarkkingdee.top/gtdyfhejib.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.316326.xyz/gtxbhbdxlu.html

[L07] 处理 HTTP 状态码
来源：http://hz.tianlin.xyz/gtbgyfdhxp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtcrnjdmzp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gtartthfju.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtxdrfbcie.html

TS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtdlyscavw.html

Java: resp.statusCode()
来源：http://hz.cheryme.top/gtrjeqxwdk.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtjoujppoc.html

Ruby: resp.code.to_i
来源：http://hz.yuanzhike.top/gtiqzfcsan.html

C#:   (int)resp.StatusCode
来源：http://hz.yj202588.top/gtuvwgmbke.html

[L08] 并发请求多个地址
来源：http://hz.jiagoushi.top/gtsytpsful.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtksklnozl.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gtctoeudge.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gturkmlrlx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtwetgxvhg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.feifeiyinyue.top/gtwssokhgy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.meibo888.top/gtizjbxqej.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dashuyun.cn/gtspoaxrqh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jlsjyb.cn/gtmugkajgq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtdcpcpdrf.html

M. 命令行 / 进程 / 环境
来源：http://hz.9152youxi.cn/gtlnxgrqgc.html

================================================================================
来源：http://hz.yuxming.cn/gtnnijhtus.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtdtvosaog.html

Py:   sys.argv[1:]
来源：http://hz.yvedp.cn/gtxrkxiumn.html

PHP:  $argv;  $argc;
来源：http://hz.xingfuxueyuan.xyz/gtjawkcukw.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtkstgkhla.html

TS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gttujrytqt.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtqfnxzjqy.html

Go:   os.Args[1:]
来源：http://hz.xziqi.cn/gtwjcwvaua.html

Ruby: ARGV
来源：http://hz.jlsjyb.cn/gtyskcnulq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtrzwldipm.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtpdardyhf.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtsonvshtt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenzaomai.com/gtbdgbcyto.html

JS:   process.env.HOME
来源：http://hz.fzhhl.top/gtmgtgdnky.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtjlxtatpw.html

Java: System.getenv("HOME")
来源：http://hz.nanxinkj.top/gttdriqekn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shuidangran.top/gtyqjsohmz.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtizblkyuf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tian-w.cn/gtyqbnobux.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtburedces.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jyoumei.cn/gtglpxnmvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtukxgcfqu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtinuofrcx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shuidangran.top/gtzrhyvfrl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtvzlctqly.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtdmqkuraa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtphuyuxtw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhoulong.xyz/gtqtyxipyd.html

[M04] 获取当前工作目录
来源：http://hz.yuxming.cn/gtpcwpymnq.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtrskkjslq.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gtkkinqwxw.html

JS:   process.cwd()
来源：http://hz.redwolf501.top/gtqzkfpmsa.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtyphkwcme.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nwbrower.top/gtnhabsgcd.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtkgiqmpii.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtooonjvvj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhijiandao.cn/gtxzjykgty.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gteyqolkpv.html

Py:   sys.exit(1)
来源：http://hz.zhengqikj.top/gtnsgnrlgy.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtjnyehguo.html


<!-- 参考信息 -->