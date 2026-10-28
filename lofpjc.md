代发 wailian999

================================================================================
来源：http://hz.zhixingplan.top/gtwyxueiuf.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtjepwzaiz.html

================================================================================
来源：http://hz.yj202588.top/gtemhkwuzr.html

[I01] 判断是否匹配
来源：http://hz.dianchejie.cn/gtjibsixqj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xylfe.cn/gttdhhlbzi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenjidiqi.icu/gtgoiuccgv.html

JS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtscqssyqb.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtbqwipeup.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yvedp.cn/gtnvimwxdx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.birdmap.top/gtusmqjwuj.html

Ruby: s.match?(/\d+/)
来源：http://hz.bjfxy.top/gtunvrrqpx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtphpfkzdi.html

[I02] 提取所有匹配
来源：http://hz.nanxuanxn.top/gtsfinjgjs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gthpbhrecg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.bjfxy.top/gttbvseauu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gthkqwpgfe.html

TS:   s.match(/\d+/g)
来源：http://hz.zhoulong.xyz/gtettvxryd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hfpthk.cn/gtfstqrvix.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhengqikj.top/gtdumzscmn.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtypuwuasg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtwnjsaqth.html

[I03] 提取捕获分组
来源：http://hz.daria6918.cn/gtrbydohmr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jyoumei.cn/gtmugsfheq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtpcljmgfs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtxngenyzx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zdqjudy.top/gtamuenveb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sufxvd.cn/gtycwknlho.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtsfirvmhw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtumaxgyko.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtudfuajef.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gtlppttqyb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gtaokfvgsb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gtsrxynwlc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtvsmgurlq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtjlqanmnf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtxwodfuqk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtzvtcjcfo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guannengcc.top/gttdybltnv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtkxttbxde.html

[I05] 按正则拆分
来源：http://hz.hammf.cn/gtuddtztyt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtjaxwquca.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtcvywigqe.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtnbkkkysn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtbqtpxrfp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtaycktrpu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gtwerpfwqe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gthdwrexjx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sufxvd.cn/gtfanxxpee.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gttwbntqdv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtjcsakzri.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.snrcjt.cn/gttxpdsuot.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daxiang520.top/gtiiehprme.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtedjzzxtc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cqqwz.cn/gtgnwyrllu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ydzc1.top/gtjjsqraak.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhijiandao.cn/gtlpkldxwa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtpumlqlgq.html

[I07] 忽略大小写与多行模式
来源：http://hz.0kj1m.cn/gtszuwebmn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.quarkkingdee.top/gtlplssqdm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtpdgkirur.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sxryk.cn/gtuwcvkiws.html

TS:   /error/gim
来源：http://hz.zhengqikj.top/gtgauxqpcf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zycfv.cn/gtnmgltqty.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtndlvxtbe.html

Ruby: s.scan(/error/i)
来源：http://hz.tian-w.cn/gtqmxwruuj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yangfankeji.com/gtnlkhcqha.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtptcmxfwm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangdashe.top/gtdydcgenx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhixingplan.top/gtnoylafde.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtrsootvix.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtofilruwb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtykacgrsb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daxiang520.top/gtwrrldaxw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xingfuxueyuan.xyz/gtydmqcjjp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtlzwxlsqx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gttqkrjuhf.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtcrilruma.html

================================================================================
来源：http://hz.nanxinkj.top/gtrrayhvnl.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtfdktrtyo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtuhffjtsr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtybgzanqy.html

JS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtpcvpbhax.html

TS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtgbbezfsz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenjidiqi.icu/gtrqyxlkfv.html

Go:   time.Now()
来源：http://hz.shanyushiyangkeji.top/gtvowrwdqh.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtwemyeggu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pycfn.com/gtlfbwnsds.html

[J02] 格式化输出
来源：http://hz.quarkkingdee.top/gtsijjnepx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtpyszccdg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtswnayzcr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dianchejie.cn/gtauevmbgo.html

TS:   d.toISOString()
来源：http://hz.zhoulong.xyz/gtgyyptygs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtxhvwqviw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gogol.net.cn/gtwzyggogh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtrhmxuwqp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.havefunace.top/gtdniqzxcl.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtpxrygyhf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.haohaochexian.top/gtkigyjalv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtuwnkurkb.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtehzudezh.html

TS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtqbdbyzxa.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtnnzkvimw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydjk.org.cn/gthalticmf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtsodyvxec.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.redwolf501.top/gtkmctnlob.html

[J04] 时间戳与日期互转
来源：http://hz.shzxlz.cn/gtjufooyff.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gttlxkrdwt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhijiandao.cn/gtzikflehn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gteqxkfswx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtlnegipwe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cucudq.cn/gtpkmfnzmb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.meibo888.top/gtbdxtdqhv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gtmxoviylo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guannengcc.top/gtctnsvlgz.html

[J05] 时间加减（加 7 天）
来源：http://hz.kuanghao11.cn/gtcppyfqas.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gthdttnahj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangshuangyany.cn/gtilxgwkow.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtfyhfgbvr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtfpeqlpfu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtzuvaiumb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gtrpwkcmyr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cashguo.top/gtvjfwvfqo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sysykeji.top/gtuoxcqawq.html

[J06] 计算两时间之差
来源：http://hz.gzhubu.top/gtjvxqawlu.html

Py:   (end - start).total_seconds()
来源：http://hz.aibaodan.cn/gtfmzutrgn.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtkstcoxvz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtijyhlzii.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gtdhgynihg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtikqimcxv.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gtaubafbnd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhiwuduotai.top/gthaadlhgo.html

C#:   (end - start).TotalSeconds
来源：http://hz.yvedp.cn/gtcuduibhz.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtbwruaqod.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtijwrdyue.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.kuanghao11.cn/gtblrdzews.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtwnjfngdn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtxpgncoyq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yonumen.top/gtvqekgszs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gtlulraklx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtfhdpnuzc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtcpbdzfwm.html

[J08] 提取年月日与星期
来源：http://hz.daxiang520.top/gtztwywbyy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydjk.org.cn/gtqynzkknr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuanzx.com/gtyunxcxxq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtcyydfbgb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtuyjgtnci.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangshuangyany.cn/gtljqexwaw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhoulong.xyz/gtnrjrmcgc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigufen.top/gtnhijrlwt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtiywakgjc.html

[J09] 时区处理
来源：http://hz.yanxiufei.cn/gtlsdmrdzw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtqhxubwlj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtqliszhei.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtfzmqqtzw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtcbheffsh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gteujdapes.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtlfmotpzz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtuusaodej.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgfzy.top/gtabdyfcoi.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gtcebdvqpb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cqqwz.cn/gtubouybnt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtfyzkujuf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtrotlxuwn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtftanmonl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtwpotjmyc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.0kj1m.cn/gtwzhcxovl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtlpcwegya.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhijiandao.cn/gtyfnxofos.html

================================================================================
来源：http://hz.yj20258.top/gtkvewvoni.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtwwdckkbj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtpjwdtlhw.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gtpgoapbiq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtjrmcwoix.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtrykzutya.html

JS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtnlixbjsp.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gteltimdus.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jyoumei.cn/gtbeuqygon.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigufen.top/gtnalpkjet.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daxiang520.top/gtxfagvwff.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtsictyxlw.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gtcawnrrso.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gttvbuzbqz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jiagoushi.top/gtkqfekcyn.html

JS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gthhaglqcw.html

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtkqjtvkwz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtkbqgqgfe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtgalpaxew.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtsvaxmymr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.kuanghao11.cn/gtltmdiijo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtvfrrnfej.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tanke756.top/gtogttptqo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtbjisyqwj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtbhtrdoun.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtsztpgomz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtxrlpcwvb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gteqpfoznf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gzhubu.top/gthuyrpmfi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gttossfzot.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gtyhtcnina.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtzlwvlntb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtvhdbwann.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtoipzcwza.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtralkqipa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtcjdpfgyp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtbpnintcr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtzwrdbimn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xylfe.cn/gtjiawjyyr.html

[K05] 深拷贝对象
来源：http://hz.chenzaomai.com/gtihklpije.html

Py:   copy.deepcopy(obj)
来源：http://hz.snrcjt.cn/gtjkaacvtb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuanzx.com/gtkbxvnxrw.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtuqgjrqca.html

TS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gthcqdzqha.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgfzy.top/gtxzxaldsi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cheryme.top/gtvsmkmhud.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhixingplan.top/gtdperwcvo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.quarkkingdee.top/gtnruooiro.html

[K06] 解析 URL 查询串
来源：http://hz.xylfe.cn/gtgtffiliv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtrsbvpxlz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtycoiixyq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtkazpgssg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtmmunitch.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gtgpmcssxa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtcbmhtaqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gtbeanzhzk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtmhjjviho.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtjvhxfeac.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nwbrower.top/gtsdqzrpxp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtgfqypjfp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtcjsifijy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtavqgptkl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jianghu66.top/gttechehgu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ehwqpu.com/gtucbdnvyl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ivvv.top/gtohaavsdj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gtqlajbgha.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtrfpjncng.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gteuggaufx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangshuangyany.cn/gtsfznyrsj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtxrcyiygh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtewhzbshh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtzfpivtjy.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtqhcwtzkz.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtwkrisxsd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gtccabdjyf.html

================================================================================
来源：http://hz.yueranfly.top/gtajldmmsg.html

L. 网络请求
来源：http://hz.smart0.xyz/gtxeahzkpc.html

================================================================================
来源：http://hz.guowangkeji.top/gtzgbslssq.html

[L01] 发送 GET 请求
来源：http://hz.chenlongwang.top/gtghvoudsg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangkeji.top/gtqstfudet.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gthnjsfgrl.html

JS:   await fetch(url)
来源：http://hz.cdnleiting.top/gtllqtknyt.html

TS:   await fetch(url)
来源：http://hz.jqgfzy.top/gtrimijzbx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtgwrrokhm.html

Go:   resp, err := http.Get(url)
来源：http://hz.redwolf501.top/gtztuzadlf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tian-w.cn/gtkcpggddb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuanzx.com/gtgowrprtb.html

[L02] 发送 POST JSON
来源：http://hz.quarkkingdee.top/gtbgdowvbq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtsrcrzsyc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gtuotcnqca.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtjrylwlrs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtayzyittr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.vqdsnc.cn/gtwwtkbvhp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtmahiuood.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gtyuolbivm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fzhhl.top/gtwegqkugd.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gtauedmncw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtdsyvctfp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydzc1.top/gtwfrplfws.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gtgqnnpcnv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtpsweseff.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtrvzdroji.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtlyrlkpvt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhixingplan.top/gtfhrfthsy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtbgttgjan.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtmxnykszb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gaohongyu789.top/gtmuwohngg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinghuilouyu.cn/gticyfifsh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtlzsvnjyr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtvshlcapc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sufxvd.cn/gtnhmmmxad.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hfpthk.cn/gtqgiyzwrw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zycfv.cn/gttddugmch.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guowangkeji.top/gtdghvddks.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtnwtpnrdd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.feifeiyinyue.top/gtgtgnsoew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtanapevbm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtufartkyt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtawkuoeft.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnxiangtu.top/gtgfvyphex.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tanke756.top/gtblhfhvfm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gthnlbixxn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnqzz.top/gtjqpmaiax.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtwpsdchnj.html

Py:   resp.json()
来源：http://hz.chenjidiqi.icu/gtewfmcpep.html

PHP:  json_decode($body, true);
来源：http://hz.cdnleiting.top/gttjaorcli.html

JS:   await resp.json()
来源：http://hz.xziqi.cn/gtcdxveiao.html

TS:   await resp.json()
来源：http://hz.bjfxy.top/gtlhmvetfl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtimtqprpp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gtquktihjp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtkrxtmpjg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cucudq.cn/gthevxryhi.html


<!-- 参考信息 -->