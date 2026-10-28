代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtrwdopkam.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtdlzueovy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtquwktyqw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gtgewjtssb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydjk.org.cn/gtgftzjldz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fzhhl.top/gtxhrnuear.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhijiandao.cn/gtrtcxiqdl.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gtemqsiraq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtqhbtnsyh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtjekewanp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtcgwisrcp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtvmaiwldp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhiwuduotai.top/gtmxhddpzc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenzaomai.com/gtosgpasxm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtexumgvor.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cqqwz.cn/gtusqizklx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nwbrower.top/gtrbqvtcbh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gtlxjddypw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cheryme.top/gthrtbesxc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtmdnshwhd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtsyyhjerk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gtdwlbxyxs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtuiylwtnm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gttxalyhoj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtbrbaqqrz.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxuanxn.top/gtuosljwlk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tanke756.top/gtomyoshwa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtefxyactg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtuorlxwzv.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtvldgxfbe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtxrxzoztb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gtdifsyfhj.html

Ruby: s.scan(/error/i)
来源：http://hz.sufxvd.cn/gtjedhmgtz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nwbrower.top/gtyczsducj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dashuyun.cn/gtuatslbmc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gtcyqisdnl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtjhlahxgs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtllmvcbsu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtkruetvqe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtxklenlsy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtithziyox.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangshuangyany.cn/gtnttlcxfc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guannengcc.top/gtvwboxcxk.html

================================================================================
来源：http://hz.yonumen.top/gtehzxhpwq.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtplmjqowi.html

================================================================================
来源：http://hz.daria6918.cn/gtkzpjfohd.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtefhulgtv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sufxvd.cn/gtnttnleyz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuxming.cn/gtkxzrhhzg.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtqcimnlsu.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtcrhupuyj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenzaomai.com/gtzyeegnpo.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtetgmxkbe.html

Ruby: Time.now
来源：http://hz.yongpay.top/gtqswtnkde.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.mhx1999.top/gttzrabqge.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gttqnchpyg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gttufzpwsx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtbjqdanul.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tian-w.cn/gtodiyezio.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gtgeshnvba.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtmwwdwyhz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhixingplan.top/gtrdwhpjmd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gthuzlfnpm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daxiang520.top/gtqqhinqnw.html

[J03] 字符串解析为日期
来源：http://hz.ydjk.org.cn/gtfbasncrd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtutigvbhw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtnyrfvabs.html

JS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtebifadbb.html

TS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtsdjiapop.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtunlidcqn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangshuangyany.cn/gtbxyjmwjd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtbbxmwgyq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.svipenyu.cn/gtvdpqpcwh.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtbtwedcwm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.snrcjt.cn/gttipevnop.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gtqbqsunum.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sufxvd.cn/gtvwasnkfc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtvujjcsva.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sweek.top/gtuzdzefrc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gttedomain.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj202588.top/gtxbeerzku.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtmgqbpgkk.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtagluuppx.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gthzmbzmxq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtdoisxadw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtcyhzmynp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtbzqxvbfu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtnkugcanc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xingfuxueyuan.xyz/gttmdwtock.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gthcmxpcbb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hysaishi.cn/gtnlxnynsf.html

[J06] 计算两时间之差
来源：http://hz.jiagoushi.top/gtffcmobuo.html

Py:   (end - start).total_seconds()
来源：http://hz.hnxiangtu.top/gttlxseewf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtpntyvyco.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtesnhoepq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtjtwjzxby.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nwbrower.top/gtdchhazds.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtmhhkrnoi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangkeji.top/gtaxyvuynw.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtlbbnhzzo.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtbupwjzpw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gthdnuneyp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtromvrikv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtuaukmgal.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtpiwlcqmu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtrvdgcftv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtfgtjlalk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtektabkxx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtajbtloej.html

[J08] 提取年月日与星期
来源：http://hz.havefunace.top/gtfwmcqiec.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydjk.org.cn/gtfnefdznz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gtvofealay.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gtwuvxeqim.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuanzx.com/gtqkhpgkar.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinghuilouyu.cn/gtmwifnzgw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtzyqfiyco.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangshuangyany.cn/gttuwxzcie.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.feifeiyinyue.top/gteqifcslt.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtoesmvlso.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhijiandao.cn/gtuiihyonu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtjmbkmdgq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gttphducqw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtrilreizv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.0kj1m.cn/gtbsfsvblg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtbdywxymq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtehzxsjnk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gtvvrlnumx.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgfzy.top/gtroqwipqg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtsppgtmqg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258.top/gtymwrjifx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtaftmgyuf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangkeji.top/gtsxaxqllr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gttiprezsw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cheryme.top/gtkvdwoevj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydjk.org.cn/gtrqfiqgyl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuetiantiany.cn/gtzbaflzls.html

================================================================================
来源：http://hz.nanxuanxn.top/gtoexipknp.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gtukpuslpx.html

================================================================================
来源：http://hz.dianchejie.cn/gtyseqjumv.html

[K01] 对象转 JSON 字符串
来源：http://hz.tanke756.top/gtfwtqumfz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtyynyuizj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtvuojccbd.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtownqwzyh.html

TS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtpkmxerqo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gthikadbgr.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gteotsydbr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtvtkyydjd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhaomingkeji.xyz/gticsgazax.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtkcwzcous.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gtwkirisiq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gaohongyu789.top/gtyqfjldnb.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtennigiyb.html

TS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtscbbsyql.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gtrwcpkcls.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtqckghlmv.html

Ruby: JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtezinweng.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gtnixwvrbc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtdwthktjg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtvlbkcoiw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtqrkckuum.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtfnssgdkx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtgqdfluyf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xylfe.cn/gtoywljutj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gtdpnxaynw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gtomgtyzyq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydjk.org.cn/gtylakwfpr.html

[K04] 读取 JSON 文件
来源：http://hz.xuanzx.com/gtrsozjczi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gtnclzgkbq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtzeaxtlyr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtjlzmdfmo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtqyfidixg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtwxldvbmx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtrbdcpokt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xinyue.icu/gtxcekoaec.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtnefwqaft.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtbjehamrz.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gtachqshnc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ywan-chungtsiang.top/gtccpozuky.html

JS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtgptoyiol.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtjnbwsmaf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gttkfknvcv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.c1oappe.top/gtxvtbqhcb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gtrgpanciw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhixingplan.top/gtmxpsmjia.html

[K06] 解析 URL 查询串
来源：http://hz.gogol.net.cn/gtggajuqtg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nwbrower.top/gtmzeixcbx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gtdllmkvhx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gttkgsicye.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.0kj1m.cn/gtzowlxlqv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hammf.cn/gtfywxbxpz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtqaerokom.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gtcuicfjea.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtppnmpnkt.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtvcpzemvs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jyoumei.cn/gtlepdtgcz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxinkj.top/gtytogqnvg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtvkdlfbyg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtnbcbhirj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtwdluzaub.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhiwuduotai.top/gtanvsmisg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtzzgbybhq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gtfyepstlm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtithqlhlp.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gtzlauxjxl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cheryme.top/gtlgxlvaqk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tianlin.xyz/gtrxgqvjzo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtafaeahji.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.9152youxi.cn/gtvxazhhnk.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gttlmoriww.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gtugkztyjl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gtezttbkic.html

================================================================================
来源：http://hz.zhixingplan.top/gtldqavqoc.html

L. 网络请求
来源：http://hz.gotoacloud.top/gtyaeirnuu.html

================================================================================
来源：http://hz.fengsongda.top/gtxzbgcyes.html

[L01] 发送 GET 请求
来源：http://hz.bjfxy.top/gtxwapgskp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtggwwgklu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtvazhqcpq.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtasqqyjrq.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtzalkrxvf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenjidiqi.icu/gtowffbayb.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtqhxcyoao.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xziqi.cn/gttfmxgtso.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtldjolmmm.html

[L02] 发送 POST JSON
来源：http://hz.yuxming.cn/gtjrilvtch.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnqzz.top/gtluhpjzcg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daria6918.cn/gtkieuhouj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtoqyymszv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtobdfknwb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.redwolf501.top/gtqjvzexdi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtmgesaizw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtzylgujus.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.vqdsnc.cn/gtszduotol.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gtrfkxsnmx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.snrcjt.cn/gttabymqdd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gthhtiotcg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtibavueab.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtqtmgwpkd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtkeujoowj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gttecpjzjx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenzaomai.com/gtydxjxfgu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gtpggyavgk.html

[L04] 设置超时
来源：http://hz.zhixingplan.top/gtchqxqebx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.havefunace.top/gtfxdlghgz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtzlsnzjzs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gthqsetknp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gtzagnvzjw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigfzy.top/gtyeibujxd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhiwuduotai.top/gtcjygnacq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cdnleiting.top/gtwjjfgkwz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinghuilouyu.cn/gtcuhksxby.html

[L05] 上传文件（multipart）
来源：http://hz.jianghu66.top/gtjfryikss.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtbrjrnnqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtyxosiylt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtdfqltwdh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gttcncagvw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yvedp.cn/gthqyjbmca.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ivvv.top/gtrpgqpwwy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.iojbl.cn/gtxwaangbe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenlongwang.top/gtmebjjqip.html

[L06] 解析响应为 JSON
来源：http://hz.jqgufenzy.top/gtzlxsmknw.html

Py:   resp.json()
来源：http://hz.birdmap.top/gtoodjrwnb.html

PHP:  json_decode($body, true);
来源：http://hz.ydjk.org.cn/gtycxqzffh.html

JS:   await resp.json()
来源：http://hz.tanke756.top/gtnpvcqnoo.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtbazstlnr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258888.top/gtgimzebmx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jlsjyb.cn/gtiaqnktxr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fzhhl.top/gtpnsudann.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cashguo.top/gtrtitwrlg.html

[L07] 处理 HTTP 状态码
来源：http://hz.gotoacloud.top/gtghxbebcr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gotoacloud.top/gtzdtcdvrr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhaomingkeji.xyz/gtojbhxqkm.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gthoclddmd.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtornkkzkq.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtjpaohznt.html

Go:   resp.StatusCode
来源：http://hz.meibo888.top/gtiqriktdk.html

Ruby: resp.code.to_i
来源：http://hz.zhiwuduotai.top/gtpwfozgdu.html

C#:   (int)resp.StatusCode
来源：http://hz.smart0.xyz/gtnwcysxdx.html

[L08] 并发请求多个地址
来源：http://hz.iojbl.cn/gtlobsoxmb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daxiang520.top/gtnwqepswl.html

PHP:  curl_multi_init() 系列
来源：http://hz.yongpay.top/gteheqbatz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtwmhkbdls.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtybxyowgp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtcbwozoxw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtcvrolnqb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtjcxtdurf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtziaptsoc.html

================================================================================
来源：http://hz.guowangkeji.top/gtcjqsamqj.html

M. 命令行 / 进程 / 环境
来源：http://hz.ydjk.org.cn/gtyhufnyda.html

================================================================================
来源：http://hz.nwbrower.top/gtskgleocj.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gtlhmrrdjw.html

Py:   sys.argv[1:]
来源：http://hz.guannengcc.top/gtyrcdunph.html

PHP:  $argv;  $argc;
来源：http://hz.yueranfly.top/gtbnycvrcr.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtgfwcypwi.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtnddebwss.html

Java: args 数组（main 方法参数）
来源：http://hz.xuetiantiany.cn/gtlaluyjaj.html

Go:   os.Args[1:]
来源：http://hz.quarkkingdee.top/gtibfboimd.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtsikymsyr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtrzbbqqne.html

[M02] 读取环境变量
来源：http://hz.yvedp.cn/gtwliqqhrk.html

Py:   os.environ.get("HOME")
来源：http://hz.zhixingplan.top/gtwamvkecw.html


<!-- 参考信息 -->