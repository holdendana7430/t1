代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yueranfly.top/gtvnvswony.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtxgnopixa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtccjalbdc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guannengcc.top/gtsvjbemnb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gtczghgoon.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigfzy.top/gthqwgjtxy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gtbauizmiv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gttagwnmjd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhaomingkeji.xyz/gteigladps.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hysaishi.cn/gtntrbiosz.html

[I04] 正则替换
来源：http://hz.ehwqpu.com/gthptjtlni.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gtgjshglge.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtawgpyptw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtzltavgpg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtewucmjxo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gtreouebbj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gttbezeizd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtobvhaxzv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yanxiufei.cn/gtgpgqyrnn.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtmrojukzl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtroooogbe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgfzy.top/gtwaayvfft.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtkezvludo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtjvrpykpp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jyoumei.cn/gtaawhqqdn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj202588.top/gtojeqwrcj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtoajklzsk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gttxtxfplf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtzvwyewpk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtvxjybyae.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gogol.net.cn/gthkdvvdwj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtbkfyuxlg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtavwcbyhm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.redwolf501.top/gtdnstdcvp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtyszehbvc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.c1oappe.top/gtcnivljki.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtwbgxcrfi.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtlqipeywm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigufen.top/gtdzaasxdg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtjfvtebhl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.52xcode.cn/gtvndrmblw.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtbdsexefn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtuesftfab.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tianlin.xyz/gtgccrsowg.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtzqskrxxs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shangyingyoupin.top/gtbvakweth.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhoulong.xyz/gtenjjieuk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xinyue.icu/gtbafteuaw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtpefnmdmw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtvpxyqzjt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtsvktpvhn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtfzjjmhso.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtcsukwxbo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangshuangyany.cn/gtrllsneiz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtmzwdmlky.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtzognqgga.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtljhltmkv.html

================================================================================
来源：http://hz.ivvv.top/gtnesnivhq.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtrglhbipz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtmpxvcepm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtiiacerql.html

JS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtwnoqvttm.html

TS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtpohmvofy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gtwyfltujc.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtthaaaoot.html

Ruby: Time.now
来源：http://hz.zdqjudy.top/gtbhhtfcnu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shangyingyoupin.top/gtkifttxre.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gthjsrgmte.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtvuzopopn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtsfulyxom.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.quarkkingdee.top/gtazfleihp.html

TS:   d.toISOString()
来源：http://hz.birdmap.top/gtzhpjvpum.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.havefunace.top/gtvdurgnmd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtwsqugnxn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtokhoewei.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangshuangyany.cn/gtvgkoipnv.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtfseqaedz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jianghu66.top/gtqbcvscvr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtbfprkgnn.html

JS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtkofewrcj.html

TS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtuwkoaypi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtnjhpkgba.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtcluhbkis.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtbchkzrkb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258.top/gtfloktcnx.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtittvubwd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.iojbl.cn/gtwxgfhrqr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtejpoozuq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cashguo.top/gtwfslpygj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtqaruditr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtexlllfbz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtsapeipta.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gtoqyjpqwv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtunnfshap.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtylgzttvr.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtbewmkfwy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtyneqjokm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtbjpimlho.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtjvlwdcis.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.iojbl.cn/gtqouytyxx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gtzgizidrp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xylfe.cn/gtuojorekx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fengsongda.top/gtofalzjry.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtjzlbdqjn.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtyhbfoklv.html

PHP:  $end->diff($start)->days;
来源：http://hz.yueranfly.top/gtnofjrtdz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gtlvfzylyx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.9152youxi.cn/gtufvxqofl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtafjaphnz.html

Go:   end.Sub(start).Hours()
来源：http://hz.52xcode.cn/gtpcbiaezj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtlgquopnm.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtxlxhfcdh.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtrbagtlmu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtohtfnwcc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtmnoafeqe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gtvuzyicta.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtvffajhgr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xingfuxueyuan.xyz/gtxhdwvaej.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ivvv.top/gtsalpiffp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gthvlwnwba.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtjzvhchan.html

[J08] 提取年月日与星期
来源：http://hz.ivvv.top/gtvrcklgqo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtpfxibrcv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cashguo.top/gttnbjaqwx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuanzhike.top/gtvedqzfdz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gtznxjbowc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtkiajjnmt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nwbrower.top/gtryygfrkj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxuanxn.top/gtejicdbtw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhengqikj.top/gtgrteymyx.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtwbajhiuj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangshuangyany.cn/gturxauvtz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtbghtyznf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtcrgwvtuj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtonwfeprw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtuzjdojqf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dianchejie.cn/gtcfoixwkg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydjk.org.cn/gtfltsehte.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtovxqxkbr.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtnffmzjnl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigufen.top/gtlryzzmmk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.kuanghao11.cn/gtcvjsfujt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sxryk.cn/gtvcbgudam.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtzdiyjkke.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtrwtrpemc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtmkhmvtba.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gttkwmavbu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtgrooaxnf.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtppxzokji.html

K. JSON 与序列化
来源：http://hz.tianlin.xyz/gtmqchhsjz.html

================================================================================
来源：http://hz.shuidangran.top/gtlnfhyzmq.html

[K01] 对象转 JSON 字符串
来源：http://hz.xylfe.cn/gthrtvpfmv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtfpexyykr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtgdjzxkof.html

JS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtldztakeo.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtvmxxjchh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yongpay.top/gtubxrwqad.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gtaxorhfpn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.fengsongda.top/gtuwnugixr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sufxvd.cn/gtrgctsdxz.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258888.top/gtdpauzxlf.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gtigliuciz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtuojkywbf.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtzcjjhsnf.html

TS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtrjtbvvev.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gttzomvitq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtktreeqax.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtxwuhjlgy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtfmixrgtu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtwjdlorxc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtchhlwexl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtyyidwcdm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtpbvjwygz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtyeotqlvq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gtsezcnycj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.iojbl.cn/gthzieebts.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gtooicpihh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gthdxcpond.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtgnpqitmz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tian-w.cn/gtapmrgxwd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtsyqvqibl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtzwocgzqq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtdplgbxjz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.meibo888.top/gtdtfvbfty.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtnqvwuvkc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.svipenyu.cn/gtawxwlvum.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gtssntilrn.html

[K05] 深拷贝对象
来源：http://hz.feifeiyinyue.top/gtqocukjsf.html

Py:   copy.deepcopy(obj)
来源：http://hz.zdqjudy.top/gthyrxezyg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtoarixzil.html

JS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtmbmyxkgi.html

TS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtwampufrh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nwbrower.top/gtovxvwnrf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhiwuduotai.top/gtteflvpiz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtzaiyjhvj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.c1oappe.top/gtkjsdjxsv.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtfctousqb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtwtmerrqu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtexounfpp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtjvaeygrn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtywqzvjcq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtptaprjee.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gttyiovpep.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtwhngzcok.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yvedp.cn/gtizswsxvz.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtrlxyiogw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtvlvekpkn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtgiwibfac.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtpdpufywb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtontnwcdr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtngcdvikz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yanxiufei.cn/gtxoehzcqy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258.top/gtkphvitbh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtlqgpbdqy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtfqnfqlpf.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtquvbrtes.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.bjfxy.top/gtbjxzzhot.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dashuyun.cn/gtudwfaqkr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtfljyiauy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtljwahbky.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gtvqqcgytt.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtquhujzlx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.dashuyun.cn/gtpfxmdobi.html

================================================================================
来源：http://hz.dianchejie.cn/gtgtvgsimr.html

L. 网络请求
来源：http://hz.birdmap.top/gtpckvdyrw.html

================================================================================
来源：http://hz.sweek.top/gtrkftmyrk.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtcfmwhexc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtzhymsndt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtlcxdnjgu.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtnfwcixdv.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtjadtpoib.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuetiantiany.cn/gtujgrqglo.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gttoorhdxj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtbxlkpwls.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtwylaylma.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtibiytmvu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gtufjrhvke.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gthuqdhwqh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtqrtxtjkg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtobzxmjdz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zdqjudy.top/gtvzptreue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangtech.top/gtfjgmjpoj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhoulong.xyz/gtcugqvdhp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fzhhl.top/gtwbvnevmm.html

[L03] 设置自定义请求头
来源：http://hz.bjfxy.top/gtntpiyral.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhoulong.xyz/gttubulmhj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gtreybewvv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtzoycbygn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtqwyirhqm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jyoumei.cn/gthzbvjpwn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtlcpnspwv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.c1oappe.top/gtrgyrtwcv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtxqmqmcrt.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gtynlrqjhx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtrjsllfzd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydzc1.top/gtfjznlybb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtzyobunzh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.bjfxy.top/gtohtbogby.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtsokzybao.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinyuanbaomall.cn/gthigowuyu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtobdjmftj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gtvtvyarjm.html

[L05] 上传文件（multipart）
来源：http://hz.xuetiantiany.cn/gtpefmtjey.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuetiantiany.cn/gtjtlwfksr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ivvv.top/gtrxmmlimt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtpmkrufvh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtxkvnubfp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxuanxn.top/gtdkmwzslo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daria6918.cn/gtnharojxz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gttnoutuvb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gtlruyzcem.html

[L06] 解析响应为 JSON
来源：http://hz.feifeiyinyue.top/gtbtxnurdq.html

Py:   resp.json()
来源：http://hz.sufxvd.cn/gtzxhjbjaz.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gtjlzaicct.html

JS:   await resp.json()
来源：http://hz.xinyue.icu/gtcymxpbyd.html

TS:   await resp.json()
来源：http://hz.meibo888.top/gtbmrdftbr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtuucvlpkk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aibaodan.cn/gtvwlyczmd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guowangkeji.top/gtdexaugja.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sysykeji.top/gtenuainum.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtvkdhimfj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shzxlz.cn/gtvufsxavh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cheryme.top/gtjvhsgldu.html

JS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtsfvcnnoi.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gttiynnnal.html

Java: resp.statusCode()
来源：http://hz.snrcjt.cn/gtimebytoz.html

Go:   resp.StatusCode
来源：http://hz.ehwqpu.com/gtjteooqaa.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtoawpftya.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtwoayuhyt.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gtvggzjqrc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtqhxwksij.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtrkcnimmo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtimksdpnp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtmwiauftm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangkeji.top/gtbbfxsrot.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtigpxfskn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gteiehnfkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gtevhxjxwi.html

================================================================================
来源：http://hz.pycfn.com/gtjfmitben.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gthgxfuizh.html


<!-- 参考信息 -->