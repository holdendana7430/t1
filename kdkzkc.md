代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtyewvwxlx.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtswqzczsf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtoituifqb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shuidangran.top/gtdonalanz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gttafgqgzh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gogol.net.cn/gtiztfswwa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258.top/gtczuejfmt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yongpay.top/gtgsbtyild.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtkcennrqy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtziobgjcs.html

[I04] 正则替换
来源：http://hz.hnxiangtu.top/gtdjycmeje.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.vqdsnc.cn/gtreytqxhh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.andypj.xyz/gtvbikzepc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtpmoyhzon.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtqocpzhyx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydjk.org.cn/gtdsvajhhq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtvxjjjjnp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydzc1.top/gtwusrjehi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenzaomai.com/gtiuwpywvd.html

[I05] 按正则拆分
来源：http://hz.andypj.xyz/gtgrvtqrcd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gtvkjbbdnj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cdnleiting.top/gtpopqrtrb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtfkqdmkur.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gthkkulqmx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhongyouzk.top/gtmafnniqi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtalvobxpw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtooogqebs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.svipenyu.cn/gtjjedsiob.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtcohrgucq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtmfwgyahk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtenyxmfsk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtwesyhyap.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtxdgmqgvf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hfpthk.cn/gtjlndoruc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gogol.net.cn/gtpolcpjur.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xziqi.cn/gtyeygxvar.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtuepfoved.html

[I07] 忽略大小写与多行模式
来源：http://hz.ivvv.top/gtpopcwstu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtagcismje.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cheryme.top/gtfrpjgjky.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtdbbmkenz.html

TS:   /error/gim
来源：http://hz.dianchejie.cn/gtplzrlijo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fengsongda.top/gtmlpcqdxk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtdlfnzxod.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gteqoysjyo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cqqwz.cn/gtrksyhqev.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zycfv.cn/gtljvjzsjq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gtrwsmunhm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtjubosbav.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtbqbjgxmw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtkncwjxna.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtgvmsklec.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuanzhike.top/gtnhrmcjvo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgufenzy.top/gtzxzvtndf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtkvraogkm.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtwfuqouor.html

J. 日期与时间
来源：http://hz.sxryk.cn/gthdmjivcx.html

================================================================================
来源：http://hz.wangdashe.top/gtvfxsnufy.html

[J01] 获取当前时间
来源：http://hz.tian-w.cn/gthzwmltpf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtpfjkbmep.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.c1oappe.top/gtnvsddxvy.html

JS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gteivzbwfo.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtsikwzjfc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtdfanoqri.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gtvkmcsbts.html

Ruby: Time.now
来源：http://hz.xuetiantiany.cn/gtkaznzats.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtrheknprg.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gthijkeusb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtbnvkchnq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gttazellis.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.feifeiyinyue.top/gtlojugskz.html

TS:   d.toISOString()
来源：http://hz.tianlin.xyz/gtiptybvlu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtcigjpjam.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sysykeji.top/gtzbuijdza.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtrzwnqtwf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gtjecbzieq.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtjjvoffco.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gaohongyu789.top/gtsyfxdfal.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangtech.top/gtmmylkadf.html

JS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtubkpzgxm.html

TS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gteykkuqth.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtusgkcpyg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtbyyijwsn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtjtjbihcw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gotoacloud.top/gtwgjogrcv.html

[J04] 时间戳与日期互转
来源：http://hz.316326.xyz/gtasvvmxtl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yanxiufei.cn/gtpgaseokd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtnpeoahku.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhiwuduotai.top/gtjmwvpybr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gtmysmoyyf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtzdzypzwx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtrmtzftqn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtcsskdgiu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuanzx.com/gtxsonroat.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhixingplan.top/gtxzeasjtu.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtdgsudfjy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtnxikaypm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtnsqjxhzn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtueosuybz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtqadgtouz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtxlgwjhhe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtodsxgxwu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yueranfly.top/gtvnqokmab.html

[J06] 计算两时间之差
来源：http://hz.mhx1999.top/gtmxmkwjyo.html

Py:   (end - start).total_seconds()
来源：http://hz.fzhhl.top/gtwvvgrpjq.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtpqvxcrep.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gtwufaiqlu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtxysyphyu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtuglevymq.html

Go:   end.Sub(start).Hours()
来源：http://hz.iojbl.cn/gtxbnszuue.html

Ruby: end - start                 # 返回秒数
来源：http://hz.vqdsnc.cn/gtdoaqgwws.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtpsqjkwyx.html

[J07] 比较两个日期
来源：http://hz.chenzaomai.com/gtcfyivzea.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtfbdyqzcy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gttiqvtlwj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtdbmatcyg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtwxtheasq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtaoxxtcyv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258.top/gtzgedkkht.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtbrvrwlhc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtehwllucc.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtepkkjyfw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aibaodan.cn/gtiglthoxg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jyoumei.cn/gtbcdmduzi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cheryme.top/gtnxucxgpx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtsztpsfrv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtbkitdylk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtqmghxzts.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gteanahtsl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtacfzilyi.html

[J09] 时区处理
来源：http://hz.zhixingplan.top/gthmjpkjxt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtuejozwji.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtbumtxupl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.quarkkingdee.top/gtawpriibl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtiedfskox.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtfjvkllsa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtadkkrvgf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgufenzy.top/gtulvfmihh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtvynlbjvj.html

[J10] 取今天 / 本月第一天
来源：http://hz.andypj.xyz/gtpzcivkvq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gtfwpaxtih.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gteyckrbzz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sysykeji.top/gtmksxissj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtawyeaqit.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtoawgpdgo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangdashe.top/gtcttrmdjd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtpxhipshc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gtlxaorykl.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxykvjabp.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtzfitlwrj.html

================================================================================
来源：http://hz.tanke756.top/gtsmrxrfzc.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtbvcymysu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtotobbivt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtjzelgnix.html

JS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtpllwdssf.html

TS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtszahhtky.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtxkznjsez.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtyxzrbskq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtpwnaclrb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtcurgspbo.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtotryavgt.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtrdvtdxhl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhongyouzk.top/gtbquupafc.html

JS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtlrunnehy.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtmlmxzrzf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtfjvvbeab.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gttxfwqlvd.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gttoxakvrg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jianghu66.top/gttzzywbjl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtfjuozfet.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtoldcfmus.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cdnleiting.top/gtgxciedws.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtoyzuwqcb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gttexfszya.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhongyouzk.top/gtwvliilsl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hywenlv.cn/gturusjgaf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtjeukwpao.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtosaceoad.html

[K04] 读取 JSON 文件
来源：http://hz.andypj.xyz/gtltekcbpw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtoxattybh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtaavbnxji.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtbvozvsna.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gttflvntjh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtqimbygua.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtntjbhvmy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtvlxcnprt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinyuanbaomall.cn/gtrvnvvvoi.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtuvdydiok.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtercitpje.html

PHP:  unserialize(serialize($obj));
来源：http://hz.redwolf501.top/gtdolnoslw.html

JS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtmpcgsqqj.html

TS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtnemvjoxg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtifzsweix.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jqgfzy.top/gtreqcoczq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuanzx.com/gtyimzdznx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shzxlz.cn/gtljgmlvcz.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtktydrtgq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gticdfhlkd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gzhubu.top/gtnqjpgfgi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtoirbwubq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.316326.xyz/gtlihpgupc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gtyocugedj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.9152youxi.cn/gtsusopatx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtzmjpwqje.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gtbjfermxo.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gthfqmyybd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gotoacloud.top/gtvwauslzp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtuwzueqpg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtrnlpsxtr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtcicxwoiu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtdlhtfeke.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtldfkomzu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258888.top/gtvbhybttf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gzhubu.top/gtjznmettx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtmztzmcbh.html

Py:   pickle.dumps(obj)
来源：http://hz.0kj1m.cn/gtefsgqgha.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guowangkeji.top/gthulweaqn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtkpmcenzw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtndavrrbb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gttijzkyck.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtywkckbor.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxinkj.top/gtutisprnp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhixingplan.top/gtrxdxtbuv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcvnpcjyz.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtducgcsyk.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtcfdjahcp.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtnzbbhlqa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtuoedjwpi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shzxlz.cn/gtueczrtei.html

JS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtjkfvzyno.html

TS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtfbshgjbj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxuanxn.top/gtvpnwnidi.html

Go:   resp, err := http.Get(url)
来源：http://hz.pengpengdd.cyou/gtgkqatopc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuxming.cn/gtvfgoxtcn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.quarkkingdee.top/gtvsrnmhkf.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtcpqlxurk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtoqcoccoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj202588.top/gteoutxcgc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gttjzmtave.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtkcrtqbwm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ppjwa.cn/gtyxhdudia.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gttmxkkuqs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cdnleiting.top/gtqarukfbv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.bjfxy.top/gtdjqpopae.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gttjqgqipw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtaaipqtba.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnxiangtu.top/gtmaslsymc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtkhkskokt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtsmolkklk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258888.top/gtgzozknrv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daria6918.cn/gtzpzxnucq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jyoumei.cn/gtqaewkpbo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.birdmap.top/gtlocmjhts.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gttokgqqim.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yvedp.cn/gtvejgycsm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gthzvwgzsf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtqxyciqpv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtxsgasapu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtivuaznqp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtqacjzmkk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hammf.cn/gtoczgewrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj202588.top/gtojifhiee.html

[L05] 上传文件（multipart）
来源：http://hz.birdmap.top/gtjapaexcd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuetiantiany.cn/gtgcscspxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtsjaxucgp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtqzrbudfy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.iojbl.cn/gtvuczgxjt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pycfn.com/gthdkkbqqk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangkeji.top/gtbiwycdkf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtvuzyqiww.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tian-w.cn/gthshsnfxd.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtljdwemcn.html

Py:   resp.json()
来源：http://hz.jyoumei.cn/gtqhhfllxi.html

PHP:  json_decode($body, true);
来源：http://hz.fzhhl.top/gtahjbdktd.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gtmpocmomo.html

TS:   await resp.json()
来源：http://hz.ydzc1.top/gtwkhtpbye.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sweek.top/gtrkrwvorw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtzpbqyhkp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xziqi.cn/gtkrtmdnna.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtjwdeikzg.html

[L07] 处理 HTTP 状态码
来源：http://hz.xinyue.icu/gtlwlralxd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shuidangran.top/gtompdahfi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.52xcode.cn/gtlkgcniel.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtmgpunjhk.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtqtpjiuaa.html

Java: resp.statusCode()
来源：http://hz.ydzc1.top/gtraqhghuu.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtwhnrqkte.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtzsjemmfq.html

C#:   (int)resp.StatusCode
来源：http://hz.xziqi.cn/gtdzltxulk.html

[L08] 并发请求多个地址
来源：http://hz.xingfuxueyuan.xyz/gtablkjgjd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtuocaxknw.html

PHP:  curl_multi_init() 系列
来源：http://hz.kuanghao11.cn/gtmukxkwjm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtpyuegeot.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.redwolf501.top/gtneszhjxd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yongpay.top/gtmuuvyoru.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.andypj.xyz/gtiaiiquxh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtqbhalkos.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtowlphwki.html

================================================================================
来源：http://hz.sweek.top/gtkzfjmzfm.html

M. 命令行 / 进程 / 环境
来源：http://hz.ppjwa.cn/gtavyhgzlt.html


<!-- 参考信息 -->