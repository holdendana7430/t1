代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gzhubu.top/gtkylswiwc.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtaaxlvfth.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtkjwnqanu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gturmgxyva.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtamsvecuk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cheryme.top/gtwrjuudav.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gteowryrum.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigufen.top/gtbowtjxjy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtuuconvrc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gtaxpgganw.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtwtufmmkv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gtvbemgcpy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daria6918.cn/gtcecnnzmc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtlfudsccd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gttgiwgoye.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ybcxt.top/gtbbfcwdpo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tanke756.top/gtzzavevtn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhixingplan.top/gtjmlabksy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtdocfsbpi.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtewujhpbl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtxjtzotwh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.feifeiyinyue.top/gtytlphbnw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtsigqjtgh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtpizwawmg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tianlin.xyz/gtuooecflw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtprzzyppw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtadztscjv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.haohaochexian.top/gtrhqfmvzk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtpahdfcor.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtjmpvqpph.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtrmzznymo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtarcimwvr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtsygogqpc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gotoacloud.top/gtsnhayrbi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtymarnnti.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtsgttkqvm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yanxiufei.cn/gtrmvuubzf.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuxming.cn/gtcfooxouy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zdqjudy.top/gtwxsulnfe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yueranfly.top/gtunsywqwn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.vqdsnc.cn/gtdfibmole.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtxzeqbfcv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cheryme.top/gthenxhqjy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangkeji.top/gtcpysclae.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gttympodnm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.52xcode.cn/gtnmootqaq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daria6918.cn/gtwhhufhva.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtxjhkjqxf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtoylfcckz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtxtncopoc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gthxvfwdvj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gttsfvwuct.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtwfhlmybw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yangfankeji.com/gtlvtvggzk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtzoqzdzwq.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtyubpxzlk.html

J. 日期与时间
来源：http://hz.0kj1m.cn/gtcacadmxd.html

================================================================================
来源：http://hz.zhijiandao.cn/gtaooxttye.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtsrxpvpwj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gthpawpbxo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtblgtmwga.html

JS:   new Date();  Date.now()
来源：http://hz.316326.xyz/gtcqcceumi.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtgsxyqwzw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jianghu66.top/gtiawoxrnl.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtzhutvalr.html

Ruby: Time.now
来源：http://hz.daxiang520.top/gtrgzcjqkg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gtewcogkfm.html

[J02] 格式化输出
来源：http://hz.gzhubu.top/gtdjubhdle.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtovchsedh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtdyjahxyq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuetiantiany.cn/gtixhnriuu.html

TS:   d.toISOString()
来源：http://hz.xziqi.cn/gtpxfvupjq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gtioxhyftt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhoulong.xyz/gtwvpzjjgj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtivevutsm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jlsjyb.cn/gtgdpzshmg.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gthcssqaoj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuetiantiany.cn/gtjbsrnowj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.mhx1999.top/gtbiblobif.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtmlnxtarl.html

TS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtojmcgxhj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtpctawohj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gtxqxzijrd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtspgzmyzu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtltppnadd.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtsvrxadas.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yangfankeji.com/gtnqmsdouh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sweek.top/gtuzzrdqqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tian-w.cn/gtclgaalnu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtnxkefojq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtvooljvel.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gtfhdypgcr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yanxiufei.cn/gtzisozgsi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yvedp.cn/gtvdflzeks.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtbzrfyzcm.html

Py:   now + timedelta(days=7)
来源：http://hz.jlsjyb.cn/gtykqrlpvb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gotoacloud.top/gtlyiynzbi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtbafvcncj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtpukeihzd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtvudakbxm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gtxjhtimyq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hfpthk.cn/gtrfylplfw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hywenlv.cn/gtuyacokof.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtwyupzykq.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gtmcztmsfs.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangtech.top/gtdzckvzig.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtcsefhnoq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangkeji.top/gtpmomrnbj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtqtbtipqj.html

Go:   end.Sub(start).Hours()
来源：http://hz.52xcode.cn/gtqisgrdtr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtnnirsgij.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gtipgedsjm.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtjoxjpnwp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtqnvqjfae.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtbfjcxsvx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gttciylwzj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtkxcilcoc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aizwys.cn/gtsloztfta.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tanke756.top/gtrscebfvs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtguvpympk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gthttlrtey.html

[J08] 提取年月日与星期
来源：http://hz.xziqi.cn/gtfesmqyki.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gtivdrbzcm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigfzy.top/gtvimlzaej.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtzvbqsjas.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenjidiqi.icu/gtnlmfarzh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtudbujbvw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jianghu66.top/gtiyumgtsf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtbeixmttu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtoyaihber.html

[J09] 时区处理
来源：http://hz.andypj.xyz/gttpegqnwe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtrvpkadvs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yvedp.cn/gtllokfzjb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtunzdjzdd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtuvpqsjhy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cashguo.top/gtttrvrnpx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fzhhl.top/gtczrkzcyc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ppjwa.cn/gttpomolfm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yangfankeji.com/gtycxjqfue.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtzujwvpqc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gthtwtmduz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxuanxn.top/gtgdcrfxiw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gtdthbydxa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtrvfkayul.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtvxlehpqn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtjlqfgozk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gtayislnle.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shanyushiyangkeji.top/gtwlcjkudp.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtsafpppuf.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtyyxufxyo.html

================================================================================
来源：http://hz.guannengcc.top/gtgwgcwmzx.html

[K01] 对象转 JSON 字符串
来源：http://hz.feifeiyinyue.top/gtthperelg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yonumen.top/gtgpnujuzw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtloszzpsm.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtweiebzxk.html

TS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtsvcfgnet.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.svipenyu.cn/gtjdplqodm.html

Go:   json.Marshal(obj)
来源：http://hz.smart0.xyz/gtluluxzsq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.iojbl.cn/gtltmjxdbp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtamgbqcpo.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtaqugnwdg.html

Py:   json.loads(s)
来源：http://hz.snrcjt.cn/gtvvluxbky.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gtpyzislzb.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtyirgvphf.html

TS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtrivbzkkc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gtvoztubvi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtcdxbqfiw.html

Ruby: JSON.parse(s)
来源：http://hz.yangfankeji.com/gtwhsenyqc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yangfankeji.com/gtfstmhltp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtbyibudgf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtqqdyofjc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gttneejqxl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtubrczixv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtuoqhxchi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jianghu66.top/gthjsiqkie.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtucjrcbcu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gtljxlhrts.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gthomudqtp.html

[K04] 读取 JSON 文件
来源：http://hz.xylfe.cn/gtipuunfjm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gthrobemjp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tianlin.xyz/gtsgekzsah.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtdlveqxmf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtaxwvuqko.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtlzfkyjyq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtncqbbads.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gtxxzufsmr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuanzhike.top/gtkmbhczry.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtfrpsyaaf.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhixingplan.top/gtjoxmkths.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sxryk.cn/gtmvtzzcrm.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtfblhxfdh.html

TS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtwjivadop.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtbfxmcbed.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yangfankeji.com/gtogulyyxj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydzc1.top/gtamilgkld.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtznbryaxn.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtqaxavqlf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xylfe.cn/gtyfihhvuh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daria6918.cn/gtfwtzqxah.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtpjfajmep.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtnbxgxwao.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.svipenyu.cn/gtxwpcpakr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daxiang520.top/gtumivzeor.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtzyuezebf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtdpliogmv.html

[K07] 进制转换
来源：http://hz.yuanzhike.top/gtzmqjgktg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtuubkhouu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.kuanghao11.cn/gtpibesgqm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtnkhuqgqs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtykwuxmfw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ybcxt.top/gthjhvzvmz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.quarkkingdee.top/gtokvqrcdr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.iojbl.cn/gtimavrmks.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxinkj.top/gtlyjugdzn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gtmrugejwd.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtboybenlx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gtdehmiqjl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gteawmfxsr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtssjgbsid.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sweek.top/gtcorhrwtq.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gthrgydsiw.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtpwtbtvhz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtpbfgvqkk.html

================================================================================
来源：http://hz.ppjwa.cn/gtlhzkcqjo.html

L. 网络请求
来源：http://hz.dashuyun.cn/gtpthpccba.html

================================================================================
来源：http://hz.redwolf501.top/gthfqvvahb.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtqiicfznx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gtsavcoqof.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tanke756.top/gtkvsejqfr.html

JS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtxwptmqft.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gtvjpdmyck.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhengqikj.top/gtfjkgxixa.html

Go:   resp, err := http.Get(url)
来源：http://hz.dashuyun.cn/gtgrkvpruw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtiofpwbcy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xylfe.cn/gtklrqmbmc.html

[L02] 发送 POST JSON
来源：http://hz.ybcxt.top/gttqmwxnis.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtltyeebzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtycniiwjq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtaqfbcakg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtmozvhrnq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dianchejie.cn/gtdxgpaqlh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtinuhsvfv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtfapfubdw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtaiznnogy.html

[L03] 设置自定义请求头
来源：http://hz.yongpay.top/gtlkoshjme.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtwnqxsdmx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gtcakvaele.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtklxmlpwe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gttqqhilhi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgfzy.top/gtxswakvfa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtncqrdjrj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gtynafrtai.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtqlqrqgam.html

[L04] 设置超时
来源：http://hz.mhx1999.top/gtbyivfrkh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigufen.top/gtlyzshecm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtwzgzybsi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtpgskjyzr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtgiudtcrf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtrtgzumbc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gaohongyu789.top/gtcpoaonsn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtkocksypk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenjidiqi.icu/gtmuxtiqrj.html

[L05] 上传文件（multipart）
来源：http://hz.zhoulong.xyz/gtddhigvhs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jianghu66.top/gtyohcrhfs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenzaomai.com/gtrrgogkpf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtucusaujv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtnfamnpam.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gaohongyu789.top/gtsptatmge.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gteluxrmdz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhiwuduotai.top/gtdfuqshnw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtdigoyzxi.html

[L06] 解析响应为 JSON
来源：http://hz.yuxming.cn/gtazyrunxj.html

Py:   resp.json()
来源：http://hz.guannengcc.top/gtmdjbaaal.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtpufosjfn.html

JS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtvrmjtmmz.html

TS:   await resp.json()
来源：http://hz.sufxvd.cn/gtcraplhkv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gtvirgrxzn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.52xcode.cn/gtivcsnecq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tian-w.cn/gtxyowfqra.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ywan-chungtsiang.top/gtoatcxqto.html

[L07] 处理 HTTP 状态码
来源：http://hz.birdmap.top/gtewierjce.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zycfv.cn/gthizwfxco.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtvzopaots.html

JS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtbozsggqj.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtylfgxxdf.html

Java: resp.statusCode()
来源：http://hz.wangdashe.top/gtdzjjgqlr.html

Go:   resp.StatusCode
来源：http://hz.jiagoushi.top/gtypwfiakq.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtxuufgyao.html

C#:   (int)resp.StatusCode
来源：http://hz.daria6918.cn/gtqldlrwaj.html

[L08] 并发请求多个地址
来源：http://hz.cdnleiting.top/gtdgmbefqe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtcgzimgww.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtdjurqdhv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtnmtjxyuu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtluxogzxi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtzqxlkkmt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.0kj1m.cn/gtcvrbclvy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gtluwgnbjb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gtdbgxwlxj.html

================================================================================
来源：http://hz.aibaodan.cn/gtvvxatkec.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtkduvasmm.html


<!-- 参考信息 -->