代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gtchmqgdzw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtkzncqnik.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtcubbkmco.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtvlsjxidz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gteyduhmyt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gtwjqzueua.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtematnucj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtsgwjojyd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtjxwckqgk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gttdujmuiz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gthonidkzf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtsxuypcxj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtnmuohmec.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ppjwa.cn/gtjwbzvrvf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yonumen.top/gtruqpomwa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nwbrower.top/gtvpugzrub.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtpcdbimza.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtbfdomkbx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xziqi.cn/gtvwvnyzmo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtsyujilyd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.0kj1m.cn/gtgmyfbigb.html

TS:   /error/gim
来源：http://hz.zhongyouzk.top/gtxerowvkm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sxryk.cn/gtarihxdby.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtzmnjdkcc.html

Ruby: s.scan(/error/i)
来源：http://hz.tian-w.cn/gtlequwmvg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gthxazxnlr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgufenzy.top/gtzjkmpxye.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gtbwthrnin.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtvuipftmk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtvbreeooc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtitxotloz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtjlgsqhlv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hfpthk.cn/gtgibimyms.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gtjrkotbkt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtemrqruiy.html

================================================================================
来源：http://hz.jianghu66.top/gtqhkjcbud.html

J. 日期与时间
来源：http://hz.xuanzx.com/gtjyclpogc.html

================================================================================
来源：http://hz.daxiang520.top/gtvubqolfq.html

[J01] 获取当前时间
来源：http://hz.yanxiufei.cn/gtjstbcwro.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtadgcpyny.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtllhounoo.html

JS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtdgujmtxi.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtbeomlxva.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sxryk.cn/gtrxlmqckz.html

Go:   time.Now()
来源：http://hz.yonumen.top/gtvmuqysla.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtftsacbsw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtgdbumwhl.html

[J02] 格式化输出
来源：http://hz.ehwqpu.com/gtjmmneybs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtxerimgnk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtwqalidzh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtqqhnurke.html

TS:   d.toISOString()
来源：http://hz.cqqwz.cn/gtzpqahhnz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nwbrower.top/gtmmoipbvl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtnapwpejj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtniruqgrb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtufqmjyjj.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtdfnaizfz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cashguo.top/gtlvklibyt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtylvawrqr.html

JS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtkulcxmtm.html

TS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtbjjcrdyj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtfnpcfvpl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhoulong.xyz/gtxexmentg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtpqpcvkpo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.iojbl.cn/gtnzhlilgs.html

[J04] 时间戳与日期互转
来源：http://hz.feifeiyinyue.top/gtobddriqw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shuidangran.top/gthzjfkryy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtcffmygyv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fengsongda.top/gtzesweaso.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigufen.top/gtntwgurvn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gtknvwrpvq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtogxksfgv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtmdodmulc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnqzz.top/gtcqbbreco.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtwuzetphp.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtpdzgvqhp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daria6918.cn/gtckqrlweh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtxhqmrzcp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtlvpicwtu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.redwolf501.top/gtafcpsyzh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtsefbiodh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtlyvnwdmf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guannengcc.top/gtgrbxgpnn.html

[J06] 计算两时间之差
来源：http://hz.ydjk.org.cn/gtuhckocsv.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtfbxzfuee.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhoulong.xyz/gtetwvaxwj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nwbrower.top/gtczymuzgp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtlcwmzfej.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.snrcjt.cn/gtbyagxpod.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtmcjebaia.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtzyjpnnsx.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtthyhgpfx.html

[J07] 比较两个日期
来源：http://hz.tianlin.xyz/gtiroztyhd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtxpvkyifs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gtzquwptdh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtiiaorogo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtacjkdyqn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gttsjwyjlr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xingfuxueyuan.xyz/gtfybzksge.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtjsnwduuh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtcvstqbkh.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangkeji.top/gtbzxlesoa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtwwchovho.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gteeadebbm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ehwqpu.com/gtvfzwgajs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nwbrower.top/gtkqikijuy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtrlhfrufg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtdngxfsvo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtybpnwcim.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtbftwvftt.html

[J09] 时区处理
来源：http://hz.jlsjyb.cn/gtdpmmabla.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ywan-chungtsiang.top/gtkpuivymp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtethaokdk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtiheykmkz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtxgpggkya.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj202588.top/gtxhvszwlq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.snrcjt.cn/gtujadxabt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sxryk.cn/gtjbpjhhqa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gtakcdypdh.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuanzhike.top/gtjhdtdoao.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtgoalpbgp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtggrkcxkr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigfzy.top/gtpgjwvfmk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gzhubu.top/gtbpgokkzp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtooogyktz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gteeybvrnm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.haohaochexian.top/gtowngdxqk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aibaodan.cn/gtdshbqoxj.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgvbngxgn.html

K. JSON 与序列化
来源：http://hz.jinqigfzy.top/gtlekwgdco.html

================================================================================
来源：http://hz.birdmap.top/gtrurbbwmw.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtjmtnxyip.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtqunzhuqa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtyanyvmvw.html

JS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtanmtzauc.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtxpechcrr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtugdnccek.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gtqexiatpa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydjk.org.cn/gtsynyiadj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtokxdsvys.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtdenogzcy.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtxkjljmko.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj202588.top/gtfgocvzqb.html

JS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtucuahjue.html

TS:   JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtpnzngnba.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gtdbicxajs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtqemtgepk.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtpcqcxcle.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtzivrtmrf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtisvdgqhw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258.top/gtpflskdbi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gtwnpfzmbi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtsfqkpils.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtbagoiirl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxuanxn.top/gtsmgyvqdb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ybcxt.top/gttepsmydu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cucudq.cn/gtakbsbncc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cdnleiting.top/gtdbganffy.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258.top/gtgkrhtqdq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtrhvntvuq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnqzz.top/gtywvqvxnx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtslhrlwqa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtycsopywu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtliujfywk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gteglnewap.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangdashe.top/gtdmmahxcu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gtdpszbkpq.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gtxjylxkrx.html

Py:   copy.deepcopy(obj)
来源：http://hz.havefunace.top/gtwjjmnbui.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tian-w.cn/gtdfgxvqbh.html

JS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gtfppvuzpy.html

TS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtdbvpghtz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtuwhbxqrm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gotoacloud.top/gthawqudio.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtqfkohohe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtorjfyfrv.html

[K06] 解析 URL 查询串
来源：http://hz.gogol.net.cn/gtdilwilgt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtkermvfid.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtrglanevn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtnnrfsois.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtojaopbje.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gteaaeqpub.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yangfankeji.com/gtfzdhvgld.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhixingplan.top/gtulwsinki.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gthiiqjzty.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtiundwwws.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenzaomai.com/gthkodlmmp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gtgusprpgg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtgftrgkbq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtkulremix.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtvqreutxg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jiagoushi.top/gtnvnroalb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tian-w.cn/gtbiuwejna.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuanzhike.top/gthloqfxdi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtgwjpxchh.html

Py:   pickle.dumps(obj)
来源：http://hz.feifeiyinyue.top/gtwockbwcs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangshuangyany.cn/gtzfdhogum.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtaucjisbh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtdejyjzza.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhijiandao.cn/gtfifsqpdg.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gtscgfawpf.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtgugegvlq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gaohongyu789.top/gtfxbajbbh.html

================================================================================
来源：http://hz.zycfv.cn/gtgvteayjm.html

L. 网络请求
来源：http://hz.wangshuangyany.cn/gtokfiqsqm.html

================================================================================
来源：http://hz.gotoacloud.top/gtieunnsxz.html

[L01] 发送 GET 请求
来源：http://hz.jqgufenzy.top/gtmvsqcvlr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenlongwang.top/gtcmbfsott.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhoulong.xyz/gttwbeutyx.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtyuqtaqwi.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtvdnapeyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtfuuivkzh.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gtmueasjot.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtcwhrwxpk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuxming.cn/gtmenpfsmm.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtpkdpogmp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtashmxtrg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gthjfshrzw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtehfxcuxw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtwhgfpwvw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.smart0.xyz/gtwzinfbnu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.redwolf501.top/gtvwdnexkf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtqnehxljr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dashuyun.cn/gtrgzqavue.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtpywmbzlm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinghuilouyu.cn/gthnmmsqtw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.smart0.xyz/gtquhdtsyi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.c1oappe.top/gtojufyrwb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtadafrprv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cdnleiting.top/gtlwxbccja.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pycfn.com/gtbjwqqdqe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jyoumei.cn/gtinnorspf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gthdzgosup.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtkghfdtma.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gthkpnuidt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtshwsizyj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtfwhinowt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtgltrwzhu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtthzvejcb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtawysqlai.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.quarkkingdee.top/gtmydwpgec.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtipmkxxhc.html

[L05] 上传文件（multipart）
来源：http://hz.shuidangran.top/gtnlwbyxbb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gaohongyu789.top/gtzebmrxzh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuanzhike.top/gtnowxqahr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtuvanznvp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtzfxeqzuf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtffzvnoqi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zycfv.cn/gtudbhcluo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtnebqdkco.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhixingplan.top/gtqewoyfyk.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gtwtuiyqvd.html

Py:   resp.json()
来源：http://hz.9152youxi.cn/gtwnkvccai.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtsmvevgpg.html

JS:   await resp.json()
来源：http://hz.cashguo.top/gtbkszczcc.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtilazdtjf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtfhcepjor.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tian-w.cn/gtdnsdaizt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinqigufen.top/gtjvuaemfm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hongshengwenyu.top/gtzftcpfsl.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtktalvemw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ivvv.top/gtdejnmrft.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ywan-chungtsiang.top/gthvkxghbk.html

JS:   resp.ok;  resp.status
来源：http://hz.xylfe.cn/gtdmfodugr.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gthlkdktem.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gtyqfqwcco.html

Go:   resp.StatusCode
来源：http://hz.vqdsnc.cn/gtwkxabovu.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtrgpufjfr.html

C#:   (int)resp.StatusCode
来源：http://hz.yj202588.top/gtlaheulnb.html

[L08] 并发请求多个地址
来源：http://hz.yj20258888.top/gtrbfloqof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.feifeiyinyue.top/gtajmtkkzd.html

PHP:  curl_multi_init() 系列
来源：http://hz.dashuyun.cn/gtxpulqhxr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtlmndpjmf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtxinewhcm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.dashuyun.cn/gtfzccdbms.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258888.top/gtvkchgddz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ywan-chungtsiang.top/gtrhonndsz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.smart0.xyz/gtkdrrbvrf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkcbbmmah.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gtkthvuakj.html

================================================================================
来源：http://hz.jinqigufen.top/gtococlzos.html

[M01] 读取命令行参数
来源：http://hz.haohaochexian.top/gtwmtvxpqi.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gtbucabpid.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtwtlecejr.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtkmegpvgv.html

TS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtdokdcxtx.html

Java: args 数组（main 方法参数）
来源：http://hz.feifeiyinyue.top/gtjakszhaf.html

Go:   os.Args[1:]
来源：http://hz.daxiang520.top/gtttqdkcmj.html

Ruby: ARGV
来源：http://hz.vqdsnc.cn/gtxzimcsuz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yuxming.cn/gtahvofyio.html

[M02] 读取环境变量
来源：http://hz.guannengcc.top/gtbkuajpat.html

Py:   os.environ.get("HOME")
来源：http://hz.gzhubu.top/gtxflyauul.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtowgoazps.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtonmwyxav.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtduxbuuny.html

Java: System.getenv("HOME")
来源：http://hz.ivvv.top/gtbhjnaygr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtyiphxaku.html

Ruby: ENV["HOME"]
来源：http://hz.daxiang520.top/gtdwfvmohk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hongshengwenyu.top/gtjkughptu.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtxgncmuxh.html


<!-- 参考信息 -->