代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gttbvmkjll.html

[I07] 忽略大小写与多行模式
来源：http://hz.cdnleiting.top/gtesabekvk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydjk.org.cn/gtxchwjtmc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtsaixeaai.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ppjwa.cn/gtphettruo.html

TS:   /error/gim
来源：http://hz.yuxming.cn/gtbyvjgdnb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtvsfdfayw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtdlmpvgnq.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtkhqhostw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtgvzavnwx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtfbstrpic.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gtuqmdqikc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zycfv.cn/gtngqvpwch.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtzgeltpbi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtpjylmnir.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtzzyxecrw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xinyue.icu/gtzwxtobli.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtzclagoqo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtpeafmcrr.html

================================================================================
来源：http://hz.dianchejie.cn/gtiubggodp.html

J. 日期与时间
来源：http://hz.xuanzx.com/gthvxcpesh.html

================================================================================
来源：http://hz.zdqjudy.top/gtvggebxze.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtyvosjbme.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgufenzy.top/gtraihvmmb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtoqsvtfbw.html

JS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtvggvhlwp.html

TS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtzcfmwkge.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gtcjzunqnb.html

Go:   time.Now()
来源：http://hz.hysaishi.cn/gtiwovcpwe.html

Ruby: Time.now
来源：http://hz.zhaomingkeji.xyz/gtmsbwafdo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yvedp.cn/gtvbmdiltk.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtaqkdfyuv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gttmtiippl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtnftfgngl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtnpswkmrm.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gtfirtvydj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuanzhike.top/gtuyryvrum.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtopisrohx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtqqrbokki.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cucudq.cn/gtqyupczdi.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtydkgcefe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtxdajkhbo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.smart0.xyz/gtekrphviv.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtfaoohpow.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtsqhlilqs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtkynvanir.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtqrafxxkx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtobvurjrz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtkkzzgluo.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258.top/gtqqdxielv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gteqyyhwdx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ppjwa.cn/gtahiifigy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.feifeiyinyue.top/gtunxmqiys.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhengqikj.top/gtjulsjivv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pengpengdd.cyou/gtmooxmpzr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gogol.net.cn/gtfovzkibl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gthhqlaznv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xinyue.icu/gtvdsiafso.html

[J05] 时间加减（加 7 天）
来源：http://hz.0kj1m.cn/gtiixsqgtw.html

Py:   now + timedelta(days=7)
来源：http://hz.jyoumei.cn/gtghzxxvlu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.birdmap.top/gtnwcxktlg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gttocozkmv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtoflonrec.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shangyingyoupin.top/gtlmbemevw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtjvpyoukp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtlsboengs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.havefunace.top/gtklfibzih.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtihknshez.html

Py:   (end - start).total_seconds()
来源：http://hz.ppjwa.cn/gtxyokhsji.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gtosuqwaxj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dashuyun.cn/gtijiyfmig.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtmehctuyb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gtoqeanidh.html

Go:   end.Sub(start).Hours()
来源：http://hz.jlsjyb.cn/gtyauornzy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gtcromhfrh.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuanzhike.top/gtwnvdljsf.html

[J07] 比较两个日期
来源：http://hz.chenzaomai.com/gtsoumiraf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtpnesgryh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gttyyahmqi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtlltmmlej.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtoydzcxga.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jiagoushi.top/gtcehtfypg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtubukpvcc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtdfqvayci.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtrjxzuakc.html

[J08] 提取年月日与星期
来源：http://hz.feifeiyinyue.top/gtvaqrkwzj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jianghu66.top/gtugapiqxe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tanke756.top/gtjvcytxwm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtpxgaefrf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hfpthk.cn/gtsnlyngsx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gtcykadgwv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhiwuduotai.top/gtyzcqileh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cqqwz.cn/gttilmjvzj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtacejejqp.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtxparigah.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gttvqrbkec.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gtfxpkjhtb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtzdgikuas.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtmuktvyvu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gteklwjxpn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gtsjitcgym.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yueranfly.top/gthtvtyqsm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.vqdsnc.cn/gtdejyqohc.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gtdzvurbih.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yuanzhike.top/gtnfirpoii.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nwbrower.top/gtotozjufj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtnqkavwbz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtyolkzxzo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cdnleiting.top/gtakdesojo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gtkcjafsdj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gtnbgvivzw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.quarkkingdee.top/gtgncrizpx.html

================================================================================
来源：http://hz.smart0.xyz/gtvvyqerbd.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtdctdqeuj.html

================================================================================
来源：http://hz.nanxuanxn.top/gtunrericf.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gttlakdkuj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtjlfccrqy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtauxtyxif.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtwmthcdop.html

TS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtgfjsjgvg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gthrsncrvh.html

Go:   json.Marshal(obj)
来源：http://hz.yvedp.cn/gtannyyshm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenzaomai.com/gttkzisyio.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gtnhayrmpq.html

[K02] JSON 字符串转对象
来源：http://hz.fengsongda.top/gtjgoxztyd.html

Py:   json.loads(s)
来源：http://hz.wangshuangyany.cn/gtfrmiyjdo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtwvgpnacz.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtlbdmrufz.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtqwmcnkrq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtaahfnqka.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtziczagcv.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtmarjnldl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gthpqwwpou.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtfxyhqtov.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtbczjyunn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sufxvd.cn/gtckrjqhrt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtsgsmjxaz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtqxzviccm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gthcbonnzl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtqjygnhnn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gticuvokfj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtgbshixth.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtpcpumqog.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cqqwz.cn/gtnnpxttct.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gthcuocixd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtxxahggng.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtbzywijku.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cqqwz.cn/gtcjffyply.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtyqcnepgn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jlsjyb.cn/gtjnzdiwcq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtnmubiqqs.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtvdsacybx.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gttwzedynb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtkheuskzj.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtcnnbkecr.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gttffcpkpi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhixingplan.top/gthwazmoob.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtbstoghtu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtqfbnpbez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtirbdlwoe.html

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gtpguzqmyz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtykwywvwd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhongyouzk.top/gtevgoozvf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtobbfydog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtihflvkpe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtphfywybe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ehwqpu.com/gthcjjxycx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gtrtjamhzr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gzhubu.top/gtutazdttg.html

[K07] 进制转换
来源：http://hz.smart0.xyz/gtncelfalh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jyoumei.cn/gtgwawhgyj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtejtlbrou.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtsvqafztd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtkdptdfwm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtvxxpimjz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigfzy.top/gtdlzuavbu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gtsffphrlc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.kuanghao11.cn/gtyxfeoozc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtivcswnud.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gttafcytsa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yvedp.cn/gtpxcajkdc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtyltyxabf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtnmuypybx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jlsjyb.cn/gtimugiagj.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtwxqlbuhe.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtxzowkner.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtuvkdooqk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtqclundqk.html

L. 网络请求
来源：http://hz.zhixingplan.top/gtpnebyqid.html

================================================================================
来源：http://hz.jiagoushi.top/gtjzovlfgj.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtfddmtwzl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtiwfjwkiq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtdjtabavz.html

JS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtbzckhqkx.html

TS:   await fetch(url)
来源：http://hz.sysykeji.top/gtkzxdiapq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhengqikj.top/gtkkoqwlpd.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtavgxmhqc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pycfn.com/gtdgloxvyd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtdqlxywbe.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtaqyxqbhw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtmicchcfi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtjheaytrj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtofpqxciq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtcamkibik.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhiwuduotai.top/gtmityvgip.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtfyrxlegr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.bjfxy.top/gtbfbupylx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtqkvcdskw.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtbmypzrrz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cucudq.cn/gtpyeaqwwb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtyrerzouj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtpaomqrup.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtptycvutf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtngsrxtbh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtxtmdbuaq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.smart0.xyz/gtrtjnevrw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gttxamnrzy.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gtjqcjxhxk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtdaieiice.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gtdtqjvbyf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtwjeecvrk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gttyqmyway.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cashguo.top/gtimvnensq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtpbcvslhf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtzmkprvnw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtjrdnwlcp.html

[L05] 上传文件（multipart）
来源：http://hz.jlsjyb.cn/gtlnbsbdxk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtqswtqulj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.vqdsnc.cn/gtkcrnlzqs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtufixtwzf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gttzrjwcos.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtzggeslmr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.mhx1999.top/gtefsjmgaz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gtssqakgby.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtuhjtgdaj.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangkeji.top/gtwdlghqhi.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtkoarxvzx.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtgtjczajh.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtsyxmbuxj.html

TS:   await resp.json()
来源：http://hz.ydjk.org.cn/gthfkvnyhl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tanke756.top/gtiegqxqol.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shzxlz.cn/gtlkzyrtoj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.redwolf501.top/gtpxqvadeo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtvwvnctqy.html

[L07] 处理 HTTP 状态码
来源：http://hz.bjfxy.top/gtlrgzrvfo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtjnacvyfm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhaomingkeji.xyz/gtjiuudotw.html

JS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtaqoqopdy.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtbfguufti.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gtrqsapfod.html

Go:   resp.StatusCode
来源：http://hz.ppjwa.cn/gtcsvtpnbo.html

Ruby: resp.code.to_i
来源：http://hz.nanxuanxn.top/gtblqxryza.html

C#:   (int)resp.StatusCode
来源：http://hz.gotoacloud.top/gtgkxecamz.html

[L08] 并发请求多个地址
来源：http://hz.jinyuanbaomall.cn/gtvbassoug.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtbgsnpeco.html

PHP:  curl_multi_init() 系列
来源：http://hz.ehwqpu.com/gtrmmgukxa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtoxyobrwv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gttequijzy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtcmllmbrx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtuwdykcme.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sysykeji.top/gtzrejtykd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.mhx1999.top/gtmgmiccjh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtfjhfzqwz.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gthoqyicqn.html

================================================================================
来源：http://hz.nanxuanxn.top/gtwziecoot.html

[M01] 读取命令行参数
来源：http://hz.nanxinkj.top/gtncurrqev.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gttdsxvmeb.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gtazvzxnch.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtobgngxjz.html

TS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtupoeqyzc.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gttdmfqddk.html

Go:   os.Args[1:]
来源：http://hz.yuanzhike.top/gtwzgkzahs.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtypwblmgo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.mhx1999.top/gtyahizrtd.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtkznxllmd.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtcwochzdi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtvelvqcql.html

JS:   process.env.HOME
来源：http://hz.daria6918.cn/gtunpepanw.html

TS:   process.env.HOME
来源：http://hz.jqgfzy.top/gteblqcgqw.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtstsblmxk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtinhnvmhw.html

Ruby: ENV["HOME"]
来源：http://hz.dashuyun.cn/gtszvlcgxm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgufenzy.top/gtzqcwwgiv.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtameoqmbk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtuefdkxne.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hysaishi.cn/gteetzdvmy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.quarkkingdee.top/gtowoibfbd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtijyzmuxs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gaohongyu789.top/gtjsadnjyq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtwpbjqkmd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtrrdfagoc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gtbntluryf.html

[M04] 获取当前工作目录
来源：http://hz.daxiang520.top/gtnieyslue.html

Py:   os.getcwd()
来源：http://hz.daxiang520.top/gtaloxzjny.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtdegdfafq.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtdqmeeagl.html

TS:   process.cwd()
来源：http://hz.hywenlv.cn/gtbesybhmn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aizwys.cn/gttgmuchjn.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtdruekwed.html

Ruby: Dir.pwd
来源：http://hz.cqqwz.cn/gtzkzujals.html


<!-- 参考信息 -->