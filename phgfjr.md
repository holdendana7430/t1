代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtnbcjerhg.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhengqikj.top/gtqatkfwgm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guannengcc.top/gthekcqzfj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxinkj.top/gtgonebjnl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnxiangtu.top/gtiijyoteq.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gttwkqdhcj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gtjmcsnrds.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangtech.top/gtxlmsnuzn.html

Ruby: s.scan(/error/i)
来源：http://hz.zhaomingkeji.xyz/gtqbqcffan.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydzc1.top/gttnwdltxz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnqzz.top/gtaxqebatn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtqrjwzazy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtlgtgydaw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fengsongda.top/gtdxstmxpl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtpntntkez.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtnzicpijo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtwvygiads.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtocmuozpz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtgwmivbkp.html

================================================================================
来源：http://hz.yanxiufei.cn/gttvggrins.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtyhtcwmoi.html

================================================================================
来源：http://hz.xuanzx.com/gtpzdjzfht.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtfbtnisqm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cucudq.cn/gtlsjeugwg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtyqitsyvz.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtisrhnyfu.html

TS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtkzndsgls.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtreqyjeqy.html

Go:   time.Now()
来源：http://hz.havefunace.top/gthcqyixfp.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtukkvgqnb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gaohongyu789.top/gtymdjrjql.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtvcjrudkz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtoeqjtbxu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.mhx1999.top/gtgtedkrvw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxinkj.top/gtfoiipovs.html

TS:   d.toISOString()
来源：http://hz.sxryk.cn/gtzchxfdim.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtefawxcho.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.kuanghao11.cn/gtxjyfjenh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtpxdpfnzh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtkhqklped.html

[J03] 字符串解析为日期
来源：http://hz.cdnleiting.top/gtmvexsfsh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cashguo.top/gtmxljwqjn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yvedp.cn/gtokrxsosj.html

JS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtkkiuktnb.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtkyveuvps.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtnyxndcej.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtlbdyutty.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtvceoktwz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtlekkluzx.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtvduviyhq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtkhkzzvoq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxuanxn.top/gtqmuurlev.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtnjltwshz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtzuuldzwc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gtbhiwfpun.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hfpthk.cn/gtbwsvwkwy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gtyyqmdgfw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydzc1.top/gtsxrwmncr.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtrhfuzbal.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gtebvkoxys.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gtqsbomikg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtqbcjwzrf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtckdfltue.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtuatdjwuc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtdhhsvuji.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtcptmycxm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtomtthhkj.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtsvkwxauy.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gtbrmxinqt.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gthkddkmjt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtpjblorgu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtvtwiucww.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtqoumtjnl.html

Go:   end.Sub(start).Hours()
来源：http://hz.dianchejie.cn/gtswhctsng.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtxuoviyva.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtjtosybpu.html

[J07] 比较两个日期
来源：http://hz.gogol.net.cn/gtpeprjvuj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtviaedxwl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nwbrower.top/gtcssjzefs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtcmokblmr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtqoqtbxac.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtftskezsw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.52xcode.cn/gtitluzqtr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtswjkcyhe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtkgjgudqa.html

[J08] 提取年月日与星期
来源：http://hz.jianghu66.top/gttdabdvve.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtatplwyhz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtyisjsnfm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgfzy.top/gtgzmiyunn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenlongwang.top/gtemimsqdw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gtyrlvdnii.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtfuykqyyp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aizwys.cn/gthzvrjjzl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhongyouzk.top/gtpvilbhyw.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtyarepxxk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gthexaszoe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtbxaorugh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtkfidamtc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtqapcizpl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258.top/gtdlktaoow.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.redwolf501.top/gtchmfxzsb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guannengcc.top/gtlakgmlfd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtzyutbxla.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gttaoaekdt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.havefunace.top/gtpnonagrx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cdnleiting.top/gtsdlgfyps.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gtvurixaxy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gtaaacavce.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtxnqidarj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.daria6918.cn/gtlzokqhqz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtzzrwamvx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.mhx1999.top/gtdlrjdbqw.html

================================================================================
来源：http://hz.mhx1999.top/gtcbxureyy.html

K. JSON 与序列化
来源：http://hz.316326.xyz/gtxsbqegty.html

================================================================================
来源：http://hz.havefunace.top/gtihgpeouo.html

[K01] 对象转 JSON 字符串
来源：http://hz.c1oappe.top/gtqjxdbbtm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtfyfukqng.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtuphbqyau.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtemfssqiv.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtiqxbwftr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtjctjmqcl.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gtfkhpngca.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gthnsesxkx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtbzvkseve.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigfzy.top/gtrqyiyqfw.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gttrdsybqm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtcmmkwuqj.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtftkxqwxd.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtgiavixxo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtlkhxagbo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtxtlvpftx.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtzbzaxxsz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtejtlvczf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtbbrkupws.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtalpylewy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtyvxsmoho.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtrtvadpiw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtbygodcuk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtldzmpcwr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gtqdxbkhio.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtnlwherwf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtzkslpvcj.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gthjsrztay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gthhvpdeph.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aizwys.cn/gtborfhaia.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtpkhajkyu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtyiiynrgv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gtwesqhlaf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtlsdzsiro.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cucudq.cn/gtmmxozxwh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtnxwnylbm.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtxoicrvuq.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtxaeeuvza.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hongshengwenyu.top/gtvvzpcjqn.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtrybeaiyj.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtlglcmsqm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtubmwdgsm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtwbfxhpvy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.kuanghao11.cn/gtbsjbussk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtomgnaozk.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtcnwjdwyd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtyhkcyrca.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnxiangtu.top/gthcocmgbj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtvjnehdwm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtavatddqm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hfpthk.cn/gtcappdnej.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zycfv.cn/gtslksmuka.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtfnxzbhpv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hammf.cn/gttgcucyma.html

[K07] 进制转换
来源：http://hz.wangshuangyany.cn/gtithcmdan.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258.top/gtgkgfuxfj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gtryubrbit.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtxmnqntbm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258.top/gthydzwugh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtckhruxrs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangdashe.top/gtvxjrljkg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinyuanbaomall.cn/gtpseukeij.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtdbljpscp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinghuilouyu.cn/gtqgamqbat.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtydnxunkz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtkiiwhudu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtnpkglpls.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtekxrlpsj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jiagoushi.top/gtglbkpqxr.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtoqmrjsvi.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gtjdcafmlk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtovxvdzpx.html

================================================================================
来源：http://hz.sufxvd.cn/gtybceffim.html

L. 网络请求
来源：http://hz.c1oappe.top/gtndukunzj.html

================================================================================
来源：http://hz.haohaochexian.top/gthizitywv.html

[L01] 发送 GET 请求
来源：http://hz.jinqigufen.top/gtnsbgoheg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fengsongda.top/gtcislozbx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhoulong.xyz/gtyhpefbau.html

JS:   await fetch(url)
来源：http://hz.c1oappe.top/gtmtgtblzr.html

TS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtsjfnpxyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtjghfuuxz.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtabdurhih.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtgvvugvfs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtrxfgawxj.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gtardnrodf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guowangkeji.top/gtlxylrfri.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtcgzrpili.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtsvnakgtl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtvoszmecn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangdashe.top/gtkyuymxrf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinghuilouyu.cn/gtqhpnslps.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtjeynhvgo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gtnypphdns.html

[L03] 设置自定义请求头
来源：http://hz.xinyue.icu/gtslunddtm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gthzfwlhcs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtlhhqcpnl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtkbmtkafv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gthtuzyxhb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.aizwys.cn/gtutkvrmzq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ydzc1.top/gtcspthdeg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtonkvqkof.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtxyfomwfp.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtcpngwfao.html

Py:   requests.get(url, timeout=5)
来源：http://hz.feifeiyinyue.top/gtbfasjqwf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ybcxt.top/gtycozsymw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtyyxiodkj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtwyynqeeu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gtkqugrwdi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.snrcjt.cn/gtrkzeagok.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtmtmqdqhm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuxming.cn/gtrvprnozl.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gteaxazcdb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tian-w.cn/gtupamvijl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dianchejie.cn/gtvpedznhk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtwytsdigq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtyuvjvkjp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtlelcclsd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhaomingkeji.xyz/gtlgmibdrl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.mhx1999.top/gtugrabqna.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gttegnzphe.html

[L06] 解析响应为 JSON
来源：http://hz.cashguo.top/gtaessczbc.html

Py:   resp.json()
来源：http://hz.sweek.top/gteklphnds.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtrfgwogus.html

JS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtpadmbysm.html

TS:   await resp.json()
来源：http://hz.sweek.top/gttuyangha.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.snrcjt.cn/gtptkolrcu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xziqi.cn/gtfknbdshi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxuanxn.top/gtbmxwzezu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtmvyiwfcl.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtlxxrknjx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtafajqzlf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtaozrboir.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtovnbinqd.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtjkmryogx.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gtmjvnuwyg.html

Go:   resp.StatusCode
来源：http://hz.vqdsnc.cn/gtrzrbvvqa.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtwxtlamac.html

C#:   (int)resp.StatusCode
来源：http://hz.shuidangran.top/gtqcsjrcby.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtoauslqmj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtwunghvbl.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtetneoavq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtlpctjimg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gtxcoxkade.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtjyuamsnt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.andypj.xyz/gtsjifriwo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.0kj1m.cn/gtinrcjdsu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.meibo888.top/gtpzubecqx.html

================================================================================
来源：http://hz.bjfxy.top/gttnjeyill.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtrtiqtzrz.html

================================================================================
来源：http://hz.redwolf501.top/gtxrprovgy.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtgkehvznd.html

Py:   sys.argv[1:]
来源：http://hz.cashguo.top/gtveepfqhn.html

PHP:  $argv;  $argc;
来源：http://hz.jlsjyb.cn/gthwsokunc.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtvusajjio.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtpfjuetpr.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtxdiomyth.html

Go:   os.Args[1:]
来源：http://hz.yueranfly.top/gtiqgmzlks.html

Ruby: ARGV
来源：http://hz.jinqigufen.top/gtrooqrqjv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtziiddtrd.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtbgdyjxpt.html

Py:   os.environ.get("HOME")
来源：http://hz.ybcxt.top/gtrdhqoumd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtzfmwzwju.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtteozbtbu.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtymwuhhba.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gtefmtxotf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtdcqdbudk.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtfnfzlnfg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gtfltguism.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtdpzcueug.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gotoacloud.top/gtpbccztum.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtqdhaypyp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtcweyujxc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtwqmsicap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtlbbrbcvg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtiaturhwn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtbgpzoqgr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhixingplan.top/gtucsdwoxw.html

[M04] 获取当前工作目录
来源：http://hz.zhaomingkeji.xyz/gtzbwtpntn.html

Py:   os.getcwd()
来源：http://hz.wangshuangyany.cn/gtrdtcnnql.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gtolwaqyzc.html

JS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtvnjrbyax.html

TS:   process.cwd()
来源：http://hz.hammf.cn/gtnqxegasa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zdqjudy.top/gtbpdjtchh.html

Go:   os.Getwd()
来源：http://hz.xinyue.icu/gtkiikdukm.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtpqfwjgrk.html


<!-- 参考信息 -->