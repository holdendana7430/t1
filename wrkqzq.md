代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtpcgnejdh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtycbcjbfz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.vqdsnc.cn/gtvbgfbphs.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydjk.org.cn/gtnyxxjniu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daxiang520.top/gthazfsczi.html

[I03] 提取捕获分组
来源：http://hz.yanxiufei.cn/gtmenuacku.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtowjaskvt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangtech.top/gtkohzkvqs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.birdmap.top/gtzcbqhqed.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtsorjqnqi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhijiandao.cn/gtqnozzcvd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtwahojwip.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zycfv.cn/gtypohzpii.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dianchejie.cn/gtvmmnevdu.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gthanixgtg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhixingplan.top/gtohtzjtiy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtphbetlpm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtqeslinwh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gthrfczdfe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtwzinmozo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydjk.org.cn/gtzuozdvge.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtazvkurjc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtwafzpeea.html

[I05] 按正则拆分
来源：http://hz.9152youxi.cn/gtsflberfd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtcabwrnfi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gtbxsfumue.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtlkqiedir.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtpejtueao.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtmciabcsc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xylfe.cn/gtzmztfuuc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtqrvwrbky.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtcjvcdtqt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gzhubu.top/gtgyikjero.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtirnptydb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtdfuablvv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtwrwyeefk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daxiang520.top/gthikqiypx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenjidiqi.icu/gtfrltyhkf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtcglnyrjh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aizwys.cn/gtjeaywkhe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtlzavjxzu.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtuuaplwat.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtddjvsxzk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tian-w.cn/gtpvuewztx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gthhnuvfaz.html

TS:   /error/gim
来源：http://hz.hongshengwenyu.top/gtssbypmvf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtegzxlnjq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gtutziqkbw.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtaogastir.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ywan-chungtsiang.top/gtufygvbha.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtixpjnpef.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.9152youxi.cn/gtcosgukia.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gthuihsojb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtebuvgxqc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtcmbmjscx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtiquprhqt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhongyouzk.top/gtgagdmixu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jianghu66.top/gteoxacvxg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.316326.xyz/gtgzdgfrtf.html

================================================================================
来源：http://hz.mhx1999.top/gtzehwnrli.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gthpiofwlp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gteubmvulh.html

[J01] 获取当前时间
来源：http://hz.jyoumei.cn/gtlsmlxstw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydzc1.top/gtdlydhryz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtaycodgrz.html

JS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtnbmbqgqm.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtaykowiyp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yanxiufei.cn/gtrtvlraie.html

Go:   time.Now()
来源：http://hz.gaohongyu789.top/gteyhmgmgg.html

Ruby: Time.now
来源：http://hz.c1oappe.top/gtbpxzwkcn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtxwzpdbod.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtpdtclucb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtjxodtpuh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtzxyxbjoo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtywivxaoi.html

TS:   d.toISOString()
来源：http://hz.fengsongda.top/gtaggcsqqq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtljbcfdjd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gtqoxszhnx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtngfpmqwk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gtpcvtswgo.html

[J03] 字符串解析为日期
来源：http://hz.hywenlv.cn/gtmapvjhmk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgufenzy.top/gtzycrisqe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gaohongyu789.top/gtkjhtltuv.html

JS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gthjlfxqzq.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtusynwquz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtjdujsbln.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtemkgixck.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtfxvdmqez.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtahvekirb.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtiwsdbxxj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.0kj1m.cn/gtrnkewvmg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtlxxpjbei.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtntdfgbaz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtzcsfrytv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ppjwa.cn/gtgzpkhgwk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tanke756.top/gtmwyqlthg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtjoegokmf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jyoumei.cn/gtgkdybqvv.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtbqrcxfuq.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigufen.top/gtpgptkbdf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtdoenvnbp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtiwsbnmwq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtcvlrqatn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtggjkweiw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.9152youxi.cn/gtjfdrklwn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtjmoscngl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnqzz.top/gtrhhxhmna.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtvmzqfyjh.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtnjbtjhph.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtimqcrlee.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhaomingkeji.xyz/gtilifutsv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gthnlleifb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangtech.top/gtpxqfdxnt.html

Go:   end.Sub(start).Hours()
来源：http://hz.ppjwa.cn/gtoiyfdmsq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnxiangtu.top/gttllfjepa.html

C#:   (end - start).TotalSeconds
来源：http://hz.shuidangran.top/gthuyolqnx.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtppibmojt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtdrmyfmkn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtncoytziu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtqillbvxq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtwhlovzrm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtsekufshj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtfgggomcu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtzqtidwev.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtuxwkgozx.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtleyskdbw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtoclseukp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtvamfdflu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhijiandao.cn/gtrydbevhf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangshuangyany.cn/gtxnjebatl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtaylxbvly.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtgseqzrzz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtoqomrmqz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guannengcc.top/gtgexqjijk.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtqugsbvmt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangshuangyany.cn/gthlumkyvz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtwpsbkczk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtghoasrjp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gthdllvrcd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtqgplaybw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtvwxupqig.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cqqwz.cn/gtmwvelhvm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtfeubmxuo.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gtgrhffxcy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.316326.xyz/gtzqofjgqo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sweek.top/gtgpnztrck.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yanxiufei.cn/gtzisrzoki.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhaomingkeji.xyz/gtrzpnhbln.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtnlgvpxnb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xziqi.cn/gtzxolcjnq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gthdazbhug.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnqzz.top/gtrmqfuouy.html

================================================================================
来源：http://hz.yj202588.top/gtqenvaqme.html

K. JSON 与序列化
来源：http://hz.tian-w.cn/gtivghrmvf.html

================================================================================
来源：http://hz.yueranfly.top/gtljjdpcca.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gtkyllnxcr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtlstaeekk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtdhiprnkn.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtleagqubp.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gteevlzuxx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtnrhcqxhj.html

Go:   json.Marshal(obj)
来源：http://hz.chenzaomai.com/gtjykymflp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj202588.top/gtutwcdvzi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.quarkkingdee.top/gtkbenecgx.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangkeji.top/gtrficuiao.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtxwunlbeo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhengqikj.top/gtqjzqsdvi.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtrmyjoaux.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtfrclhfkw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cheryme.top/gtqyarildo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtfakybnms.html

Ruby: JSON.parse(s)
来源：http://hz.havefunace.top/gtdyxdtdnw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuanzhike.top/gtwoxmjfat.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gthjcqsedv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtjvykorns.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtnmrlkowc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtlscpyyus.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtmnjonlfc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sxryk.cn/gtzmemikqr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gtbhpgmcpd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.iojbl.cn/gtqmnacpoi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fzhhl.top/gtlmjeyuvn.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gtodsnzkuo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtsbafdmuu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtkehjcptr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtyobyufzj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtbtisltwq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtopnnpatg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtdoygwmyv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.svipenyu.cn/gtvnsqqcxo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gthnyxayuc.html

[K05] 深拷贝对象
来源：http://hz.nanxinkj.top/gtkcvgdnwo.html

Py:   copy.deepcopy(obj)
来源：http://hz.ivvv.top/gthpkoeyux.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtgzpnufmo.html

JS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gttcmjixjv.html

TS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtdzmnwajc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinyuanbaomall.cn/gthfoymmvi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtaateomer.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtkhhxxjtr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtsfinlgxz.html

[K06] 解析 URL 查询串
来源：http://hz.haohaochexian.top/gtcizqgkci.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtuyztwynz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shangyingyoupin.top/gtouomiawl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtkdaotpzk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtdilqopgo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtzoidwora.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guowangkeji.top/gtssypmuzi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtxrzejozn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zdqjudy.top/gtvepfylgl.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtiwbompse.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guowangkeji.top/gtxgdblnyv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtetgouhcn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtaiupynds.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtbiblqzdw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtwnwgfkgc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ywan-chungtsiang.top/gtcxnnpbwy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cdnleiting.top/gtgcmugqdm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.c1oappe.top/gtavebasai.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtgpqbmpgb.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtcnylctvg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtotxgsbgs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtbhesprpn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtwuhesxjt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gotoacloud.top/gtigsufmdd.html

Go:   encoding/gob
来源：http://hz.shanyushiyangkeji.top/gtmkjdyhhe.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtbcwtjdit.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gtmtuanann.html

================================================================================
来源：http://hz.yvedp.cn/gtpmqzptiy.html

L. 网络请求
来源：http://hz.yanxiufei.cn/gtzepobpdq.html

================================================================================
来源：http://hz.zdqjudy.top/gtpoaajohj.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangtech.top/gtgbwxhytn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtthqkrvqx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtqffqfdqx.html

JS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtjfdlsjrv.html

TS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtgcreyvlr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtybxqszsv.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gtjzdnpcol.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtyyivfrui.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gttxfvssmr.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtivskkdbg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtpbiomzwc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtlddqsnvo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtyhxxmswk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gthixibedk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtuarplplr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhixingplan.top/gtmqyddqcx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gtlfgxtyhv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtoonchuan.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtfbqlcgzc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gteyljubre.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tanke756.top/gtpaarlguj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtnvmqcmvo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtlkagffho.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gtraysdhji.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtbmhftxvs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtsfjkdxef.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cheryme.top/gtmbvokezk.html

[L04] 设置超时
来源：http://hz.gogol.net.cn/gtfhhasete.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gtnbqhembw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cashguo.top/gtsjdqausw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtiapizrzo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtkzffrych.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtawvjtgik.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhiwuduotai.top/gtxdmvccle.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtwakagmos.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhoulong.xyz/gtzlkmvioi.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gthrqxvfgd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hysaishi.cn/gtuecnnjzk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gtszfrtffu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtspnugobm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gteaeurwcs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhongyouzk.top/gtoqyipqbd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtepmksbam.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gttgowratl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtegoiecgu.html

[L06] 解析响应为 JSON
来源：http://hz.zhixingplan.top/gtjstarmiy.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtccigdvgt.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gteyslhbkq.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtqowspkjr.html

TS:   await resp.json()
来源：http://hz.yongpay.top/gtnmxoqjfv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tian-w.cn/gtutbdjkwy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtcqlffkgn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydjk.org.cn/gtokrniayj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtuvinxwvl.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gttftskzat.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gtrqupyknw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xylfe.cn/gtxykxbqhm.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtysvjzsiu.html

TS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtebrdmnps.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtgoajcwiz.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtydhdniad.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtlfonqjnc.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtszhogkpj.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtjezkzadi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtmcpykaqd.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtawioqeda.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtimlrsvpu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtmhvjzdjr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtiyvfnpms.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtrzkdyhyn.html


<!-- 参考信息 -->