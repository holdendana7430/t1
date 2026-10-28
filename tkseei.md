代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxinkj.top/gtoyzyvoxa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtpptcclfn.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtsfjficos.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yangfankeji.com/gtmymhxrfd.html

[I02] 提取所有匹配
来源：http://hz.52xcode.cn/gtdgwscvno.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sxryk.cn/gtzfsnxfuy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sxryk.cn/gtafkkhuoq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgfzy.top/gtlfbwbcpw.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtlysjcuin.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtksbzncjw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shzxlz.cn/gtffwarhjk.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gtmtlqyglw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtpskycftk.html

[I03] 提取捕获分组
来源：http://hz.cucudq.cn/gtjzhnftbz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtthusqsxs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtzqdqxrpx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtphyqdjki.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtkxuwyicl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtyfjtfaeh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258888.top/gtabqgcazj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtbcmcuboh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtdwdeuxuo.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gtzqvkmgbg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtmxrqwhoj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtjueiyvgf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtzusviafl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtxmolwkht.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zdqjudy.top/gtobmzzkcl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhengqikj.top/gtwnshfszz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gtddriavvw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.redwolf501.top/gtqzdaidhr.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtskqtcrvd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtisnwibhl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtweebhgqt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtcofbgams.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtaiaykrom.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gttrsxmjyi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.quarkkingdee.top/gtwejwanii.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gthjheauiv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.redwolf501.top/gtdjvxvrme.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gthonvdndb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtstvybhoa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aibaodan.cn/gtiuakmkic.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gthnlvnbuq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtteemgoxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gththmlbdx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtbbrcxobb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtlunijjuh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtctqjzozc.html

[I07] 忽略大小写与多行模式
来源：http://hz.dashuyun.cn/gtysnwxyay.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.andypj.xyz/gtlaqrsong.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xinyue.icu/gtfolsnvvs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.birdmap.top/gtkrmlykyw.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtrxxepmvk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guannengcc.top/gtpdvysvue.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtmdbhotyt.html

Ruby: s.scan(/error/i)
来源：http://hz.tianlin.xyz/gtxuqxmrqu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtbnboxmrc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.andypj.xyz/gtgmnisobx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtvoscuadv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtuxyhitzp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sufxvd.cn/gthvfqcolq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtpqpdczil.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jyoumei.cn/gteigumdhf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangkeji.top/gtwdqtysmp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.svipenyu.cn/gtzgievysk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtvukkdrpn.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlvbbmtjf.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtbtfrpvmz.html

================================================================================
来源：http://hz.dashuyun.cn/gtbtnqqmlm.html

[J01] 获取当前时间
来源：http://hz.pycfn.com/gtmcynvvzu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtuckcaxlx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtfmpbbuts.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtkkzdlxvu.html

TS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtvlytidvd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenlongwang.top/gtzdupwmip.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gtjylzsniz.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtbjpimlcq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtynyveasd.html

[J02] 格式化输出
来源：http://hz.aizwys.cn/gtomeqitcv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtqdusyhbe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtoskntkcr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.redwolf501.top/gtjwcuxwii.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtjatulans.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtevevzbtj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zdqjudy.top/gtliexjbki.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtklxojzed.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenlongwang.top/gtlqbvptob.html

[J03] 字符串解析为日期
来源：http://hz.vqdsnc.cn/gtcbmxtbxr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shangyingyoupin.top/gtnfsdefgm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtscjavlmr.html

JS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtgtzukkyc.html

TS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtsrrtlltx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtnaizjhmy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sufxvd.cn/gtnnnxadlk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtzzdwvzgv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.haohaochexian.top/gtdeyeojja.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtylqbwibz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.guowangkeji.top/gtzchfmcec.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.svipenyu.cn/gtlgistpjk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtqjyqljej.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtaxvkythz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtwidinsgr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtrgyaovoz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtmunqynlx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gteasspkrx.html

[J05] 时间加减（加 7 天）
来源：http://hz.aibaodan.cn/gtuzkxvqyg.html

Py:   now + timedelta(days=7)
来源：http://hz.yangfankeji.com/gtokowroig.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gtadzvmool.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtnsyouekn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtbfdswhym.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtkuhtuvxe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gttwyoyqlz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtcwyimupg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aizwys.cn/gttyecgjws.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtynqyvtvn.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtvwrxdzml.html

PHP:  $end->diff($start)->days;
来源：http://hz.guowangkeji.top/gtmpcdlubi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinghuilouyu.cn/gthjasbjfa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sufxvd.cn/gtbuhbnfbq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gtjjhizbhx.html

Go:   end.Sub(start).Hours()
来源：http://hz.havefunace.top/gtgeugtaqo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtzaphwqlu.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhaomingkeji.xyz/gtkhlvqkai.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtjpbvmpju.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtaqhuzguz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtaqplshls.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gtegdfbznm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtvyonwijm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtxpecgzwi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yonumen.top/gtstpnbvda.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gttuzcozvh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtjbjhkifv.html

[J08] 提取年月日与星期
来源：http://hz.daria6918.cn/gtiiskzoer.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hfpthk.cn/gtysuhtshn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtovlrdqbi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hysaishi.cn/gtkfdgjjgw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gtyrqicoyd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sweek.top/gtevsqvlst.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtlnomzwkc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.andypj.xyz/gtpxylihhn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jyoumei.cn/gthaprwgzp.html

[J09] 时区处理
来源：http://hz.snrcjt.cn/gtgysyjzza.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aibaodan.cn/gtkqjqnaah.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtucslfbtk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtqouwszoy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtntjdjilp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pengpengdd.cyou/gteoehltws.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtwghnfjfa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtkfckmwwe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtdzzvuffh.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtyaztavne.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gtoflqqqbh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnqzz.top/gtjkutpzle.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.quarkkingdee.top/gtudlktnni.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtypyrsmdk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ehwqpu.com/gtyrpbppfn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shuidangran.top/gtazmywydn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xinyue.icu/gttpkcmfog.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.vqdsnc.cn/gtjxcngrtz.html

================================================================================
来源：http://hz.daxiang520.top/gtrfacavds.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gtqtkzbwby.html

================================================================================
来源：http://hz.xylfe.cn/gtudnrqphl.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenlongwang.top/gtjraejxos.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtwiclwdrg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtwcyddyqs.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtzjmghrlj.html

TS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtvwhznthl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hysaishi.cn/gtwxwmlabc.html

Go:   json.Marshal(obj)
来源：http://hz.xingfuxueyuan.xyz/gtlhcjaqjk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhengqikj.top/gtmanjzpmp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jlsjyb.cn/gtwwsamefa.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtjdmfueon.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtzskkvllq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtqeoovbmq.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtzdnmbrqp.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtqvjjqqkq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhaomingkeji.xyz/gtklvfvyos.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtovisyhgk.html

Ruby: JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gthpzbmmru.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gtzpgzzszo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuetiantiany.cn/gtewxcslvi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gttncwkywg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtudqeuekk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtdzyfzjkd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtxqjfgmcm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gtaabyhyqx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangtech.top/gtmovawwnn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtefenyfzj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtxcbhaovi.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtvzlrwnkc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aizwys.cn/gtwgsxkfil.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtdgsfjctf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtxgtbrqvc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtkewrypty.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtyakcdehj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtftadvwyg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gtpjyulxgm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtqhyxnqop.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtvzhrmetg.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtbusynqss.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtwuskcukk.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtkinhsnvc.html

TS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtmuyuqhvb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtrjbhkoqj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnxiangtu.top/gtuytszgfz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtvizoqvwx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.svipenyu.cn/gtnaphwffs.html

[K06] 解析 URL 查询串
来源：http://hz.jianghu66.top/gtncmbodjc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gthrocgufu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtqviaubwi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtctejkahi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtmwrnyswh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.0kj1m.cn/gtogruaioq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtfmtidloo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtzbllmvyr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tianlin.xyz/gtomlofzta.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gttupizbyg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtwqoybtvv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhiwuduotai.top/gtbllqkirh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtnoxsnatf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtgrafsyuy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtooxodfdh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtsejrmvks.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtnsnxhuvt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtxkkjlmhx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gtpbfqzped.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtzzgbiyud.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtprivmnpl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.havefunace.top/gttptscrfo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtlslakgix.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtbjkbxtxb.html

Go:   encoding/gob
来源：http://hz.yuanzhike.top/gtfgsiheox.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtxwpcvjzm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ehwqpu.com/gttpporaji.html

================================================================================
来源：http://hz.zhongyouzk.top/gtmkbagupa.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtivdhoqew.html

================================================================================
来源：http://hz.dianchejie.cn/gtlonuwkmb.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtkwmywmfq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258.top/gtcyjeuwio.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtaduwoiif.html

JS:   await fetch(url)
来源：http://hz.tianlin.xyz/gtiwmexjue.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtwinbspdb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jyoumei.cn/gtkvqzofbh.html

Go:   resp, err := http.Get(url)
来源：http://hz.jyoumei.cn/gthjhlgoow.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jiagoushi.top/gtukxesxcs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.quarkkingdee.top/gtiqlltjkp.html

[L02] 发送 POST JSON
来源：http://hz.zycfv.cn/gtvledswzn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhijiandao.cn/gttayptquu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtcfymltqp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtwviexcxc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gttqyiqreh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtmsfzmjov.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtxoqpekml.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhijiandao.cn/gtnintavef.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gthueelclf.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtzghcxlml.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtzbkmkzds.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gtjimnvznl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtmkbionos.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtyzxxkpmj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtfktztiik.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtjkzlnqlc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangtech.top/gtwwzymcwx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtlzjozunn.html

[L04] 设置超时
来源：http://hz.hnqzz.top/gtddietsgk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtiiuyjepk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gotoacloud.top/gtxsrhxlqr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtvodbqlse.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtwvtgharq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gtjqrymtsg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.andypj.xyz/gtmdtxygkw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gtayygdbsc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cqqwz.cn/gtomfdsvtf.html

[L05] 上传文件（multipart）
来源：http://hz.sysykeji.top/gtfzlntghp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hywenlv.cn/gtfktnbztp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtjixrvghn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gtuhcihkkj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtszvyvxlj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigfzy.top/gtiguebqsx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtrnnkvvva.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtpzvieozq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gthunknvsu.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtmzdavfab.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtrbirwwsq.html

PHP:  json_decode($body, true);
来源：http://hz.jinghuilouyu.cn/gtpmphpypz.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtumtibalg.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gtdobvtbnr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.iojbl.cn/gtfblnjzwz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gtbftrtntk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuanzx.com/gtpadvmcwx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtfjnxidui.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtpgvyqxiq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtiioaqnkr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtkovnnvst.html

JS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtwftjhdny.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtfnxlpjag.html

Java: resp.statusCode()
来源：http://hz.sweek.top/gtglbgnbcr.html

Go:   resp.StatusCode
来源：http://hz.jinqigfzy.top/gtdekengal.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtzpricich.html


<!-- 参考信息 -->