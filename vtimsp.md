代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gthfgbewuz.html

[I03] 提取捕获分组
来源：http://hz.xinyue.icu/gttmixvfmo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gttpctqdmx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gotoacloud.top/gtqnxkyhdy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.feifeiyinyue.top/gttankbkyc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hysaishi.cn/gtsvxbuody.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtbnzmxqhg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuetiantiany.cn/gtwuxpkkpc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.andypj.xyz/gtgccnpgio.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sxryk.cn/gtzdanisri.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtaozlxhvu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtabymljxq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtrnfblyxt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtnpjzruun.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtcdygimtg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.316326.xyz/gtsgzxyhrb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gtfakfiruo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zycfv.cn/gtsibaymya.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuanzx.com/gtyksisblh.html

[I05] 按正则拆分
来源：http://hz.jqgfzy.top/gtoltwbwoz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangkeji.top/gtkunouuzv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtdekyuwdf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtbbhqdgrs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtycyttmpi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtvpjxqzem.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtlmqwlben.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtomrxmtwc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zdqjudy.top/gtpdibhxgw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daxiang520.top/gtnpzyyeiw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtfhltmjtm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gtultjskpf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtuwvvyklx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtyjmpncdb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuanzhike.top/gtvgqdbwxe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gtydniduyj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtokcdleqa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtgdmflmur.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxinkj.top/gtfbedlybo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pycfn.com/gtxatvtozf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cqqwz.cn/gtihqwpsbg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtoeusrblq.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtqqwenldf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtjemejmvp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dianchejie.cn/gtmzddcqdi.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtjbfmqnhp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtkgirosqv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtgeqhwxuh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtebvwxxlr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yvedp.cn/gtesmwjgid.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtxddpivtt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pycfn.com/gtyxxtuqop.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.mhx1999.top/gtliufevtb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtnmkzezkh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhengqikj.top/gtztkaizam.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtbmmeedrx.html

================================================================================
来源：http://hz.nanxinkj.top/gtiqnzsghe.html

J. 日期与时间
来源：http://hz.xuetiantiany.cn/gtgleffaxn.html

================================================================================
来源：http://hz.jianghu66.top/gtndnrcyxo.html

[J01] 获取当前时间
来源：http://hz.shzxlz.cn/gttrcntnft.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtyctkcwfc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtkkjoflip.html

JS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gtqcliwgfw.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtfsqjvhrv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtknvkhgwt.html

Go:   time.Now()
来源：http://hz.jqgfzy.top/gtiuanvvvi.html

Ruby: Time.now
来源：http://hz.zdqjudy.top/gtaymxgklw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtkqqbhysq.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gtzbpmxams.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtuqvedgpz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtlsshwdqy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guowangkeji.top/gtapruucwo.html

TS:   d.toISOString()
来源：http://hz.hnqzz.top/gtbtnalskg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jlsjyb.cn/gtoxfkifvb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtapuupnun.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtmmjfqqed.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtftjsrgbf.html

[J03] 字符串解析为日期
来源：http://hz.0kj1m.cn/gtywdtntwc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtoypbxgjc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtymrqcvsp.html

JS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtppgxnckw.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtixrqagos.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtwzxhaksr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtefzqsaur.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtspxsiibl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtkhviagza.html

[J04] 时间戳与日期互转
来源：http://hz.yangfankeji.com/gtcivwlosp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhiwuduotai.top/gtfmavqadj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtombhmgcl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.andypj.xyz/gtumhvldqe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhiwuduotai.top/gtqvkltzsp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtrvpthcdb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtqgjguudr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hfpthk.cn/gtnkknojzv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fzhhl.top/gtqatvvcmo.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtkyrykvom.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtcpkrwliv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtpyrdrzmy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtesxumplx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtzjqopwnt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fzhhl.top/gtixaliddf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtopdqtved.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dianchejie.cn/gtwpextwuc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtvsirvxkx.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gtnedjxryr.html

Py:   (end - start).total_seconds()
来源：http://hz.zhongyouzk.top/gtoldwfned.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtoibocrmu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinyuanbaomall.cn/gtcrglytxr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cdnleiting.top/gtguigelcb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cdnleiting.top/gtpwsaqcgo.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtfjpbtzyo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yueranfly.top/gtbylbipkh.html

C#:   (end - start).TotalSeconds
来源：http://hz.daria6918.cn/gtgvxskhau.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtoxlpxpwo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtwobqsyde.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cqqwz.cn/gtvkwfdwau.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtnkafsney.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtoypapjgb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.c1oappe.top/gtaamsyyze.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gtubyqohfc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtqkzuuihe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtjkeslewt.html

[J08] 提取年月日与星期
来源：http://hz.haohaochexian.top/gtvbfpujtm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydzc1.top/gtkicrpgmn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gttdxwksso.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtkmqiioph.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.quarkkingdee.top/gtjllenhyh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yanxiufei.cn/gttndnqubl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtkytimpqw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gtkiincfeh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yvedp.cn/gtzjhpwfdd.html

[J09] 时区处理
来源：http://hz.cheryme.top/gtqgtninme.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnxiangtu.top/gtbapjswxa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtsuhfaxhi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtivmwbyrx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtaqjixwlp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gtgztpjhen.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pycfn.com/gthgyzawyb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtrbnletbd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.smart0.xyz/gtjlaptmvc.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtwumdtxlz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuetiantiany.cn/gtxxpvfjrx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtwjxlbruz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gttrxhrjug.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gtnefjzjzq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtwufndjhj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtfihgooej.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sweek.top/gtlhfgvokj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xinyue.icu/gtayftrpih.html

================================================================================
来源：http://hz.mhx1999.top/gtxklbxrxg.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtmvqcgkyi.html

================================================================================
来源：http://hz.0kj1m.cn/gtnjtzazci.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gtorqhbmlh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtlaxvyfsb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtviypspll.html

JS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtmjrtyvgn.html

TS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtsdqpqbud.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangkeji.top/gtcsqhhnpn.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtcfvbkizu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hysaishi.cn/gticzratlm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtbkbwduqi.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gteujwdunk.html

Py:   json.loads(s)
来源：http://hz.zhongyouzk.top/gtyqnsmpmh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtfcyehkjt.html

JS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtfsgndkgj.html

TS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtrnjhvofx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenlongwang.top/gtoxnvynta.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gtlweerzxf.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtzsufumya.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxinkj.top/gtobnpkjvb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cheryme.top/gtsfgcdyeg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtrhbbexlx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gticjagmdn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtfcacswva.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtirzrbwbz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtfthwwuoy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pengpengdd.cyou/gtayojvggc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aibaodan.cn/gtyatvigno.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtqqbanytg.html

[K04] 读取 JSON 文件
来源：http://hz.316326.xyz/gtzndsiwqq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangdashe.top/gtdxsgmhlm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtwalfidsw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtlztczknc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtxjfbdyua.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gthodhnsdq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtrjaikifp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtacpouftw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtvqtykixg.html

[K05] 深拷贝对象
来源：http://hz.yongpay.top/gtlfchqalk.html

Py:   copy.deepcopy(obj)
来源：http://hz.tanke756.top/gtwdciosmf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pycfn.com/gtzrpkyxyw.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtlhdvmpdf.html

TS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtpzqtidyz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtrnjoxepg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hfpthk.cn/gtxahhstty.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtutzgaryj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gtlnfovsbf.html

[K06] 解析 URL 查询串
来源：http://hz.pengpengdd.cyou/gtpffukwxc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtrduydvox.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtzefjogfz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtdckoyubk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtuqldiirb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ppjwa.cn/gtytegzzwr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtjkswfzpu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtjjlqyxbg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gtokbzpuez.html

[K07] 进制转换
来源：http://hz.zdqjudy.top/gtlvwyixns.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtblznmyrl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gtfrwqcxtf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtwfyiyxeh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtgvpbhbej.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtjnrxmafz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtyephpxiw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aibaodan.cn/gtulldeulb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jlsjyb.cn/gtqhjlxjze.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtjmqdqljo.html

Py:   pickle.dumps(obj)
来源：http://hz.feifeiyinyue.top/gtyroiylee.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtmfozqrgc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtsznfznwy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtoqygkytb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuxming.cn/gtjdhlmxxj.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gtheyxakmw.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtgfrqptnv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtmnwccqrk.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqqkpsavb.html

L. 网络请求
来源：http://hz.316326.xyz/gtfhmzspsi.html

================================================================================
来源：http://hz.pycfn.com/gtpueswhyf.html

[L01] 发送 GET 请求
来源：http://hz.dashuyun.cn/gtdedcfmge.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangtech.top/gtfsvvpxaj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.feifeiyinyue.top/gtdfujpjjc.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtasywrtgo.html

TS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtncvsgbko.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtldjghosz.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhijiandao.cn/gtgqnwbzfu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtnstxbenp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.c1oappe.top/gtqevaggju.html

[L02] 发送 POST JSON
来源：http://hz.zhoulong.xyz/gtscpddyft.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yangfankeji.com/gtmaeyenxv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigufen.top/gtyzvcwbxt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtnylhtqff.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtdcwzaptc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shzxlz.cn/gtfahdumvp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtlzvobibp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtrlxyavdn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fengsongda.top/gttezfzhvt.html

[L03] 设置自定义请求头
来源：http://hz.zhengqikj.top/gtfoufupux.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenzaomai.com/gteylvsxse.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gttrnzxskk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtrqcqmici.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtbdjwjdxi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtmbhsbyhr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtalkqhemp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jiagoushi.top/gtgqtvpdfm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtnmjgquiz.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtvcwytums.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtbxdhocxo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtmiazpcre.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtvdrdhygh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtbylycthq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtyqlpvbbc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhoulong.xyz/gtfleaeifa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtqdzqekjz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.dianchejie.cn/gtukxwsrfa.html

[L05] 上传文件（multipart）
来源：http://hz.xuanzx.com/gtuufwueup.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhengqikj.top/gtrrvqwclv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gtpptpgvff.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtoraiepri.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtogbvwwik.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gotoacloud.top/gtfpsiyxjp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xinyue.icu/gtbwchzlop.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shuidangran.top/gtfbyjpoyt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtccjiqjhc.html

[L06] 解析响应为 JSON
来源：http://hz.yuanzhike.top/gtyitlanvh.html

Py:   resp.json()
来源：http://hz.tanke756.top/gtpyyieebe.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtarbykaph.html

JS:   await resp.json()
来源：http://hz.cucudq.cn/gtvqhijbfq.html

TS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gthjawamcu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj202588.top/gtpnsjrocq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtounepgjl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yonumen.top/gtkhrgbklp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gtjusguvwy.html

[L07] 处理 HTTP 状态码
来源：http://hz.0kj1m.cn/gtekufezrp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gthtlawjzm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.0kj1m.cn/gtdxktnihu.html

JS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gteivyovmr.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtpylowjyl.html

Java: resp.statusCode()
来源：http://hz.zhoulong.xyz/gtsknhjaov.html

Go:   resp.StatusCode
来源：http://hz.jiagoushi.top/gtwdjreuhn.html

Ruby: resp.code.to_i
来源：http://hz.pycfn.com/gtwhmwojog.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtcptboupe.html

[L08] 并发请求多个地址
来源：http://hz.redwolf501.top/gtldmiwypc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hysaishi.cn/gtnrmitgbq.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtafcaohth.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tian-w.cn/gthfczmrsc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtvvjyhbnx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fzhhl.top/gtrgnqxssl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxuanxn.top/gtgflwfmhw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gaohongyu789.top/gtmbwffofq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtiglccopt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtafmggvsv.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtghdzloeo.html


<!-- 参考信息 -->