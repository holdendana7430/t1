代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.smart0.xyz/gtbjxehswd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtcgdsnupn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ppjwa.cn/gtlekjwyvr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtemqwcybi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cucudq.cn/gtnnirzrxk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtwwdwwrow.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pycfn.com/gtcjutawjy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtzeqjdfti.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtvywmyvjh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtlmxkabvy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtjmsatghw.html

================================================================================
来源：http://hz.gaohongyu789.top/gtnanxctnh.html

J. 日期与时间
来源：http://hz.jqgufenzy.top/gtqjueiwmq.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtiqullsrd.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtiajynudr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtoldjnfia.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtpjfgqbwl.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtlsdgvcal.html

TS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtldeplcut.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gtugsqpzin.html

Go:   time.Now()
来源：http://hz.jqgfzy.top/gtzyrfgqye.html

Ruby: Time.now
来源：http://hz.gogol.net.cn/gtpimjqhtj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.haohaochexian.top/gtumplennq.html

[J02] 格式化输出
来源：http://hz.yanxiufei.cn/gtkmhwufkk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtmqwcddht.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtzvosjxyh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtwzecaoxg.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gttizllkrn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gtkauxsdyt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtfdqgqkkf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtvtbzyozi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtjciiixrs.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtvuqadfjl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gtaonmygbq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jianghu66.top/gthurjtwfm.html

JS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtgpbiymhe.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtpyfedjwj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258888.top/gtajhduubo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigfzy.top/gtmvsossug.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtxziybyoz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.birdmap.top/gtvbecoudy.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtdittrpse.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxuanxn.top/gtjmakjpzl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.andypj.xyz/gtrdgmziaz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gtgmoxzklv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zdqjudy.top/gtwjuulcqs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinyuanbaomall.cn/gtnrikmoey.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtoooqxvdv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuanzx.com/gtiullzjvi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zdqjudy.top/gthynghasi.html

[J05] 时间加减（加 7 天）
来源：http://hz.dashuyun.cn/gtkroljydm.html

Py:   now + timedelta(days=7)
来源：http://hz.jinyuanbaomall.cn/gtrwjsafqw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ybcxt.top/gtragczloi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gttzflzwtu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtvhapwdiv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtxztagzcm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jiagoushi.top/gtkmnndjdg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtohviehzv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258888.top/gtnxpikcjn.html

[J06] 计算两时间之差
来源：http://hz.chenjidiqi.icu/gtknwibiza.html

Py:   (end - start).total_seconds()
来源：http://hz.svipenyu.cn/gthcncxeir.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtbehalart.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hammf.cn/gtmlqaccws.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cqqwz.cn/gtooqruguh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gthyodclzp.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtezjctwdx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinyuanbaomall.cn/gtgiurcyyd.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtmfclffyv.html

[J07] 比较两个日期
来源：http://hz.cdnleiting.top/gticolhoek.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtfdoggsmv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtnudxrzsy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtyzfntval.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gttvnwwbyl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.bjfxy.top/gtaetyixuj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gtwicvbjqo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtwpumejbn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtqywspycj.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtqnahkdxh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtenspnwnu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenlongwang.top/gtbhhmssam.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtqhdjosyq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gtcgzhtirp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yonumen.top/gtljmgkbay.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cqqwz.cn/gtjucdhpbt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gtacdenfba.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtglzlfkei.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtbuzihuub.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhoulong.xyz/gtexvwkcld.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtsoenydod.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtkdoriqcg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtclztqblx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtafbanrmq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenlongwang.top/gtkzbjvcyl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtpvldjqdh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sxryk.cn/gtvmyqaqmt.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenlongwang.top/gtkxbtsobu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cqqwz.cn/gtyxstrrat.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daxiang520.top/gtolwrlujd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtmcsbecsz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtufycpcqu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gthezdlviv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtendpgzsl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yongpay.top/gtioxypboj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jyoumei.cn/gtlxrfxvyt.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdsotqqdk.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtsjmpjqht.html

================================================================================
来源：http://hz.snrcjt.cn/gtpxftmasc.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gttytysujl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gtaaquicwa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtqmczzhhl.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtmqbjlxth.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtiorunweu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtgsaqnbua.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtlilupwzt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtunhsrxrm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtwdxnrxcx.html

[K02] JSON 字符串转对象
来源：http://hz.vqdsnc.cn/gtjuxbulpl.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtwpnybyzm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jlsjyb.cn/gtnvrbpbfn.html

JS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtpgcielqf.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtposalnhs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhengqikj.top/gtsndhzdaf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtptyxrrcs.html

Ruby: JSON.parse(s)
来源：http://hz.guannengcc.top/gtxjdqcwda.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuanzhike.top/gtnjrfoqeu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aizwys.cn/gtniqwkwgg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtdvzpyxvc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtrxotdbqc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtxtiykqgi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtcnwnjflu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gogol.net.cn/gtnzbtqzsb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtsamzinef.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhiwuduotai.top/gtujhrctjg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gtrblgzmdw.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtqpwauomc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtajvqefpm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtavqqrnwi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtxbcbxhzy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtytnwvfqr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtcmqfihue.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtyxiaqoox.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gotoacloud.top/gtpzdqxdeu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtdnszhhbf.html

[K05] 深拷贝对象
来源：http://hz.jianghu66.top/gtthxfahdw.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtwaatuxkr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yangfankeji.com/gtmhfsjrxr.html

JS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gthrsknimc.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtdmppwzpe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhongyouzk.top/gttozjkzfq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtxyhuqspe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gtypqrpvmp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gtstnmwguc.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gthytteobk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtfnztbscn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jyoumei.cn/gtyshqtrkh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtcycvicdo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtbninqbjw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.snrcjt.cn/gttwqmjzop.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtcpgocgzn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gttunxdnox.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtymmhvbwb.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtdvlmdszi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.52xcode.cn/gtdfncwduh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtirhitfrb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtctvdaxdg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtwxbjntau.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtuumvvona.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtmtjsdxto.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cdnleiting.top/gtnwwlbati.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtwxvzwvsc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtblfcanxe.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtottbfvvk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnqzz.top/gteekhyyud.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtbtibspmr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gthldlfccy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xinyue.icu/gtfgxdgjkl.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtsjgtkuku.html

Ruby: Marshal.dump(obj)
来源：http://hz.smart0.xyz/gtjtzfcpff.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cqqwz.cn/gtvkwoitql.html

================================================================================
来源：http://hz.hammf.cn/gtrmpubknk.html

L. 网络请求
来源：http://hz.yuxming.cn/gtqnkkuphq.html

================================================================================
来源：http://hz.gzhubu.top/gtkrmbbiqz.html

[L01] 发送 GET 请求
来源：http://hz.meibo888.top/gtjbrdctfk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtfzckapux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sweek.top/gtnrhpzkib.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtcnlvsdof.html

TS:   await fetch(url)
来源：http://hz.yonumen.top/gtrmdqgeys.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xingfuxueyuan.xyz/gtachjjexh.html

Go:   resp, err := http.Get(url)
来源：http://hz.gotoacloud.top/gtlwqzkoxv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258888.top/gtpgbeyacc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtdkjkdqgj.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtoiljadvp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtyjbxlphs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxinkj.top/gtgpsakdog.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtwriooews.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtniohkqvz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtyjlivpdd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dashuyun.cn/gtukckxtou.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtlzgmeduq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.wangdashe.top/gtoepejyhy.html

[L03] 设置自定义请求头
来源：http://hz.316326.xyz/gtccsgcjfu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shzxlz.cn/gtmkospuzw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yvedp.cn/gttuneolqq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtkevocjzl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtztcleumo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtfrgjcmkv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtjuywkhdq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtoodsdqth.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gogol.net.cn/gtplpbvpuj.html

[L04] 设置超时
来源：http://hz.ivvv.top/gtsxgauzfv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtrlnvafcw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangshuangyany.cn/gtrsakoqsk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtdkitpepo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtscpqnenm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jyoumei.cn/gthlkciyex.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxinkj.top/gtwstayjtt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtfubkijyk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gtxoqtvnlg.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gtevmdsrlw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gttqbqhlqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gtikdiufif.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtgpucwoao.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtggvscvqn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gtmjolwcdc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shzxlz.cn/gtnvwvyimq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtgohekrai.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtddqvljhe.html

[L06] 解析响应为 JSON
来源：http://hz.wangshuangyany.cn/gtowidvlki.html

Py:   resp.json()
来源：http://hz.hammf.cn/gtiinpwizg.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtjwstxkkc.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtznietopq.html

TS:   await resp.json()
来源：http://hz.sweek.top/gtpdtjdstf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.kuanghao11.cn/gtnrftuhet.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jiagoushi.top/gtnplzozqs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxuanxn.top/gtxifqjqbw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtseizvhvn.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gttssedlmx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daxiang520.top/gtzneegfhq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yvedp.cn/gtuvbrbbnc.html

JS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtbyxrqjib.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtqhphnkdb.html

Java: resp.statusCode()
来源：http://hz.wangshuangyany.cn/gtrfllsslq.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtpjfyihym.html

Ruby: resp.code.to_i
来源：http://hz.fengsongda.top/gtbkyvhgid.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtxmjgekfx.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtsgmyshxp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nwbrower.top/gtbcrujumq.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinyuanbaomall.cn/gtihnjpuwe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtjcosqtoa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtoifkanyn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yongpay.top/gtqyikfvlm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtphrpbubq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtskkylyhl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zdqjudy.top/gtqhuonyti.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtqitqlopw.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtmjfxwudk.html

================================================================================
来源：http://hz.yanxiufei.cn/gttgucsfrn.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gtsegnriap.html

Py:   sys.argv[1:]
来源：http://hz.ydzc1.top/gttyeeahrk.html

PHP:  $argv;  $argc;
来源：http://hz.pycfn.com/gtviildont.html

JS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtdzqmxwvs.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtqygqlhqv.html

Java: args 数组（main 方法参数）
来源：http://hz.yuanzhike.top/gttvqrwmpb.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtvxixbiew.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtrrumssto.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gthomeavhy.html

[M02] 读取环境变量
来源：http://hz.meibo888.top/gternxbgvo.html

Py:   os.environ.get("HOME")
来源：http://hz.jianghu66.top/gtrkzrvnak.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dianchejie.cn/gtphpvvtyg.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtlrrimgoh.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtkntsiiwj.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtepuwdype.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgfzy.top/gtiumnimcw.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gtxorlvofq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gtzhkiqiwg.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtknldljzs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sweek.top/gtggdcdsgo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtjymzgzgp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtvakimuws.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtairucvqm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gttwjpkrtd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gttvyqybjc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.birdmap.top/gtrpgusvbz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.smart0.xyz/gtxnutddna.html

[M04] 获取当前工作目录
来源：http://hz.gogol.net.cn/gtkpsyuxrd.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtcxdahpot.html

PHP:  getcwd();
来源：http://hz.havefunace.top/gthqvcblhw.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtbshdcsav.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtjjohqdkg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zdqjudy.top/gtejcqhfwb.html

Go:   os.Getwd()
来源：http://hz.yj202588.top/gtvffquizl.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtjivhbeud.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtdgdvyybm.html

[M05] 设置退出码
来源：http://hz.wangdashe.top/gtayukxsgn.html

Py:   sys.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtyuyzrfut.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtuyuygwwh.html

JS:   process.exit(1)
来源：http://hz.gzhubu.top/gtvlvgxrrl.html

TS:   process.exit(1)
来源：http://hz.jianghu66.top/gtauexglgb.html

Java: System.exit(1)
来源：http://hz.xinyue.icu/gtefrgepow.html

Go:   os.Exit(1)
来源：http://hz.mhx1999.top/gtyntykwmd.html


<!-- 参考信息 -->