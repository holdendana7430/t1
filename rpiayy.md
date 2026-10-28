代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gaohongyu789.top/gtwmliorsf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ehwqpu.com/gtuzyzrvle.html

[I04] 正则替换
来源：http://hz.jianghu66.top/gtierezilo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtehjwuoou.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtariktujm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtzrzqqssn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtgtvdqyye.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtmseiihjp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zdqjudy.top/gtfebcqoaw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtrpgvhdfh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yueranfly.top/gtcuyazgtr.html

[I05] 按正则拆分
来源：http://hz.nwbrower.top/gtogkdmalx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.daria6918.cn/gtrbawkzix.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtgbrmhttr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtrranvmmh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gttlsozdwg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yvedp.cn/gtqjatkiqz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.redwolf501.top/gtubmrwvmd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtdzfiyoia.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xingfuxueyuan.xyz/gtibgazwdt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnxiangtu.top/gtlkglylah.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gttsqlmbjp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtmwrffiqs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gtqpcuvjob.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtfugpmvca.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gtvbtprcys.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xylfe.cn/gtglelakmg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nwbrower.top/gtsyvigwrs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gthtzrhiiq.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgfzy.top/gtrxtqdxmt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtgsyuffxx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtkeavbhnu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gteljpynjl.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gtgamutqqm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtgkoephkw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtchnvmrfz.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtrsonqbon.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtmywkidar.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ehwqpu.com/gtzgffbzdr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtscdmxise.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fzhhl.top/gtbhdsziox.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtognveilw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenjidiqi.icu/gtrujgjlqu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hammf.cn/gtxlxlzzik.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangkeji.top/gtmiocftgd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigfzy.top/gtetncvajb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.iojbl.cn/gttgyzkuyb.html

================================================================================
来源：http://hz.jyoumei.cn/gtmdbhwwcz.html

J. 日期与时间
来源：http://hz.feifeiyinyue.top/gtfvagedqb.html

================================================================================
来源：http://hz.ppjwa.cn/gtvdrrltbb.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtcplstuzd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gtnvdrigjl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtdnstekux.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtyhmfhout.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtbuidwiar.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtlfqydesg.html

Go:   time.Now()
来源：http://hz.andypj.xyz/gthbwoobdp.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtmuheaftl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtmsnenicx.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtjtufuddy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtsswebske.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtdliubntb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtcgwfqgbr.html

TS:   d.toISOString()
来源：http://hz.sxryk.cn/gtjytgsdmc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenlongwang.top/gtggoijlse.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigfzy.top/gtlluklsos.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtmmpkljga.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ybcxt.top/gtkcgbyupo.html

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gtbaxtnzxu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtbacnarjc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gtxykypehs.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtiilgbqpt.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtenkziies.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtswwnqbop.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtxpzflcni.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtlocgnfzv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtbsmtgkcn.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtnywuhsjm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ivvv.top/gtswajanbl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ywan-chungtsiang.top/gtzygprcbx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtlpfwbcbh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gtjzrhrbvv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenzaomai.com/gtdbbhkcwz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.mhx1999.top/gteijdozcf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yonumen.top/gtnsnxykwh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtnpiosnri.html

[J05] 时间加减（加 7 天）
来源：http://hz.redwolf501.top/gtotfroaol.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtzcgejkxk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtsjbopudl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtgywprpmx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtwafqrxqf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhixingplan.top/gtfvejfqvw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtyqfnnvsr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigfzy.top/gtmsinmxmd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hfpthk.cn/gtkylabdot.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtztqvvdmg.html

Py:   (end - start).total_seconds()
来源：http://hz.tianlin.xyz/gtovzjiozg.html

PHP:  $end->diff($start)->days;
来源：http://hz.0kj1m.cn/gtkmlcevsc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xylfe.cn/gtyqhngqbc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuanzhike.top/gtokpvazuv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gttbgfpemr.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtxrcerzgm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtfwuhivmu.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtbioftqrd.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtuzmdbxua.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtkvexmyoh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pycfn.com/gtrudhydvn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtwnttjiki.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gthcnojxoo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aibaodan.cn/gtreawugil.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtneyajxir.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtowdotohs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtluqzmfgk.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtuezilunw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtylaiqtog.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtdvnbgonr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtvwuecgrp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtmlqahleh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenjidiqi.icu/gtchxwhnll.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daxiang520.top/gtuaczzujk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtbwhahgsv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cdnleiting.top/gtksfuxjez.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gtjrsxumfb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gthpaalovv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gtkhnrmzsb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtneadogob.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gthzbshvjv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtcfvxkzne.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtzyvdvttz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sxryk.cn/gtfuczgwhy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtwmwnpqol.html

[J10] 取今天 / 本月第一天
来源：http://hz.jlsjyb.cn/gtwvnhsdfy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtjialdlas.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhengqikj.top/gtwhebqsoq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinyuanbaomall.cn/gthfubkxcu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydzc1.top/gtrmjywldo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtwnrsctsp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.c1oappe.top/gtenirlgvl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gtiaxoujgm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nwbrower.top/gtuhywgdci.html

================================================================================
来源：http://hz.tianlin.xyz/gtxituiiqw.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtquuctpay.html

================================================================================
来源：http://hz.yonumen.top/gtammobpsl.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtyyvezope.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xylfe.cn/gthfjegrfc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtnlugevjh.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtezbpvvhf.html

TS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtcmdgwpcv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtsnjmdszu.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtluvfbwbk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtjvsmrojb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtxfqzqfji.html

[K02] JSON 字符串转对象
来源：http://hz.chenjidiqi.icu/gtieyiddjy.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtprtiyecm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tian-w.cn/gtncgxnsjy.html

JS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtsmmpnyrv.html

TS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtcpvgfozs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cheryme.top/gtjgaqovdq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtmkrhnwsg.html

Ruby: JSON.parse(s)
来源：http://hz.dashuyun.cn/gtoqiatiyl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuanzhike.top/gtsnxoxybb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhoulong.xyz/gtslqfqsdx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtaoqvntfr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtfblcqibo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtmsehebcb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtobbxziut.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgufenzy.top/gtpnqaiapt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtveghtnzs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtjrwttzzq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhijiandao.cn/gtxvlvgxkl.html

[K04] 读取 JSON 文件
来源：http://hz.jiagoushi.top/gtofohqnup.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtfdiwiqqn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtmwijkhwl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gtrxnejdxx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtcvkopayz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtgdlzexex.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtgfasodqt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtkefqulbe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtfzcrdbyu.html

[K05] 深拷贝对象
来源：http://hz.gaohongyu789.top/gtgqkbobjj.html

Py:   copy.deepcopy(obj)
来源：http://hz.jianghu66.top/gtrymoqfyd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sweek.top/gtzaxurqqt.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtbgygjsnp.html

TS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtwhvmpoon.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtnxfwvzkd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtzplolaam.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.feifeiyinyue.top/gtaduczvrn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yangfankeji.com/gtribkivqb.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gttsjcwyho.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gtscsyavdu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fengsongda.top/gtgcvwkjmm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtkkbqekho.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtgbjszspl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xziqi.cn/gtnaswdknb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.kuanghao11.cn/gthwounejt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtksqqvpmm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nwbrower.top/gtztfurlxs.html

[K07] 进制转换
来源：http://hz.chenzaomai.com/gtgmyewenu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtlpgnwvac.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gthiddupqm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shuidangran.top/gtkuvgkrdj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtbwcbtbtz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtnboiqrzb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gtflasshcc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tian-w.cn/gtqgqujckw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtyrdrqwol.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenlongwang.top/gtbhukbcyw.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gthopzmrnn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.9152youxi.cn/gtnidlbjxf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gtnczxsxcz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gttegajsjc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtgldzdcdc.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtclqdvrqm.html

Ruby: Marshal.dump(obj)
来源：http://hz.vqdsnc.cn/gtifezewpk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hysaishi.cn/gttyldqxoa.html

================================================================================
来源：http://hz.chenlongwang.top/gtgjmjesnq.html

L. 网络请求
来源：http://hz.jqgfzy.top/gtjcxxvpaz.html

================================================================================
来源：http://hz.iojbl.cn/gtpzwmkoss.html

[L01] 发送 GET 请求
来源：http://hz.tanke756.top/gtpfpxsbcz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtuqtlwxha.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gtscklcfev.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtrvfkkqtw.html

TS:   await fetch(url)
来源：http://hz.c1oappe.top/gtaykyjkve.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zdqjudy.top/gtdzlnnbns.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtsphnodhp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gttjiomsgc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shuidangran.top/gtpmvqittf.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtfulxqgsw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtxbtocfss.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtmdsfeaku.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.birdmap.top/gtftwefzxn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jianghu66.top/gthxxjfban.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gttlmylkhw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.feifeiyinyue.top/gtemrpymuf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.feifeiyinyue.top/gtvonvjvym.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtmrpqgihq.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtiyfowwho.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtwlpzihge.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xylfe.cn/gtzmafnjek.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtorxbimhx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtnykifxcd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258888.top/gtjjygtjiv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtetzvdhxx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtvfqorwgo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtbcbsflek.html

[L04] 设置超时
来源：http://hz.yueranfly.top/gtabfwzkyh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtoymxwvdq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gtiexgxioc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtdrbbzgjr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.kuanghao11.cn/gtbjcgpuwk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jinqigufen.top/gtlpwxjsxg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.vqdsnc.cn/gtjkviodlj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj202588.top/gtstbjsigo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtyacdmglo.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gtqjidgqqc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtmaurnasw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gtpvgetujj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtbdgblioe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtflpmqsih.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtfcyarvqg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtqxqwwosy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtbnzzrqao.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hysaishi.cn/gthckgpmic.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtpsqgidlx.html

Py:   resp.json()
来源：http://hz.cheryme.top/gtnvikqjfn.html

PHP:  json_decode($body, true);
来源：http://hz.aibaodan.cn/gtbbvejxew.html

JS:   await resp.json()
来源：http://hz.shanyushiyangkeji.top/gtujnlklkz.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtjfvwtqav.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hammf.cn/gtlevdlwkr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnqzz.top/gtdkdarbjf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtkhmxlmfq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtltkobmam.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtnnyjgogw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yongpay.top/gtzmzgrfoz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jianghu66.top/gtjnffhrlx.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtiabervwc.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtfuggvvib.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gtgnqdnsaj.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtuwdeouyh.html

Ruby: resp.code.to_i
来源：http://hz.redwolf501.top/gtcwfwbmdq.html

C#:   (int)resp.StatusCode
来源：http://hz.fzhhl.top/gtygvwieqy.html

[L08] 并发请求多个地址
来源：http://hz.smart0.xyz/gtuodwlqfi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yangfankeji.com/gtbkzhwtsg.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gtwocpqsda.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtttxqrifr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtiyacwjle.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gtwzxewpqq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.0kj1m.cn/gtbmmyrodd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtjwzqzqhu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtcfvegssv.html

================================================================================
来源：http://hz.sweek.top/gtebgfizrc.html

M. 命令行 / 进程 / 环境
来源：http://hz.xingfuxueyuan.xyz/gtkkypcawo.html

================================================================================
来源：http://hz.ydjk.org.cn/gtqtfeajft.html

[M01] 读取命令行参数
来源：http://hz.zhengqikj.top/gtfbwhoobp.html

Py:   sys.argv[1:]
来源：http://hz.cashguo.top/gtivnftdym.html

PHP:  $argv;  $argc;
来源：http://hz.mhx1999.top/gtarqmqjxl.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtsmpxiswk.html

TS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtzbbuxsgv.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gtcvhncxum.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtlghgmfcr.html


<!-- 参考信息 -->