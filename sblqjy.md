代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.svipenyu.cn/gtlkcnkrfn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gtogqxbtxk.html

[I04] 正则替换
来源：http://hz.yangfankeji.com/gtakcazeat.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hysaishi.cn/gtsvdtkrhi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtopxsltkf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtyqgbiibz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtpaiessja.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tian-w.cn/gtolfpekpl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtzftkknee.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gtrfkbtnnw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhongyouzk.top/gtixjflcmc.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gtjilqecft.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtlqgnztzq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtpkdjthvr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtwjsfsusk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtuywuddwe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aibaodan.cn/gtsoxmcqdh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yanxiufei.cn/gtpmoinaqz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtbazioptk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sufxvd.cn/gtfmsdsvlw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shzxlz.cn/gtydzumcde.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtnnkzumtt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gteeftxxbj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtmophnizh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtbmpqeyck.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gttqgtxroc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnqzz.top/gtlnumkllb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tanke756.top/gttrljhwvc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtisgebdrb.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtuwyvsald.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258.top/gtxzbvxdwz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xziqi.cn/gtdfohdgpd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hfpthk.cn/gtjunujglx.html

TS:   /error/gim
来源：http://hz.xziqi.cn/gtkqcpauei.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtncqrwhvp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtapaibgjw.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtqnsflnbq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gtnacqebvi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gthgshipbc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnxiangtu.top/gtdbpqmzjp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtwlbreepi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtmpvnpswx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gthyerbeak.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtyrwygpgv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hongshengwenyu.top/gtzjpruioa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtwfaysoey.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnqzz.top/gtktxnxmay.html

================================================================================
来源：http://hz.zdqjudy.top/gtdowlvkej.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtukutfzrn.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnljfsajz.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtzjehgzyt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtqeuwpkad.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtzohjiydg.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangkeji.top/gtdzqmymad.html

TS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtqbdtbljj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gtkpkhuwpu.html

Go:   time.Now()
来源：http://hz.yj20258.top/gtxwrgudmx.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtvrapsodw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtocvuxfhj.html

[J02] 格式化输出
来源：http://hz.dashuyun.cn/gtxkdefdhn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gttjfayowe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtfejglcnk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtjmxnvpdx.html

TS:   d.toISOString()
来源：http://hz.iojbl.cn/gtmultxqjc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.meibo888.top/gtcncbjfao.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gtachustob.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtcjcobcxl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtayoklwtu.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtrizrdixg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtusdjugho.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgfzy.top/gtkciiiosa.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtdrodmpjy.html

TS:   new Date("2024-01-02")
来源：http://hz.cashguo.top/gtkaqchvsv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtciaoiyro.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtpnbsppaz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gtfusiilxx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtpseesgrn.html

[J04] 时间戳与日期互转
来源：http://hz.hammf.cn/gtkajzbiny.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtqfqrfopi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.kuanghao11.cn/gthwonycya.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtnbkijxrv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtbbfiwepx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtcohtaibo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtcczbgfhe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuxming.cn/gtwgzwvier.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gtwcbudnxg.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtpeefudlr.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtmzcrkejr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinyuanbaomall.cn/gtmdxityow.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtrsleilsz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtbkexygdp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtmdkvecme.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtphiwzlrg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.havefunace.top/gtzfuyozlg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtkgtuwxhf.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtaevjblsh.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgfzy.top/gtpsxysttt.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258888.top/gteapjgjig.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtaocvqshf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtlhhcamhq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.52xcode.cn/gtjjuakril.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gtzpgglyaz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gtixddrliw.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtrochfdkc.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtxnhiyypl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtrvmjiaxk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtjefsjsuh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtcremvqbe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtffcmhnva.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtiqemviut.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtnrifzrhm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtgpoxikun.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtikgujxtm.html

[J08] 提取年月日与星期
来源：http://hz.cqqwz.cn/gtmjaxeodv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gteamilmhk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtkqvpuymu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xingfuxueyuan.xyz/gtsiiwynwb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtqfdslqea.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.kuanghao11.cn/gtaivjcffe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangshuangyany.cn/gtpnfihkzf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.snrcjt.cn/gtnnfzmbnh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnqzz.top/gtqyiswesa.html

[J09] 时区处理
来源：http://hz.shuidangran.top/gtvcugrpgf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daxiang520.top/gtdxcbweqa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtiyuwlofj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtcatibaej.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtftpessyt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shanyushiyangkeji.top/gtthqhnflb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.smart0.xyz/gtrulolmgd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuetiantiany.cn/gtccowgktm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gtrctlyhdd.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtfhkjdnbr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtebzotbhx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gtvygibwjn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtooxbhvqb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tian-w.cn/gtpiadwbwd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtroiwodtu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenlongwang.top/gtgtvfbgji.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtsqwvxyeg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ppjwa.cn/gtywcibjli.html

================================================================================
来源：http://hz.yj202588.top/gtntzagnjz.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gthazychqz.html

================================================================================
来源：http://hz.iojbl.cn/gtxeigddev.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gtfxmqbejv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtotkbvazv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtucftsfqb.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtztgquvhh.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtpzqwelwv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtdzfbczyd.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtlvxsumci.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtwjylausa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ppjwa.cn/gtekirynlo.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtolhljuxk.html

Py:   json.loads(s)
来源：http://hz.daria6918.cn/gtlubzbxuc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenjidiqi.icu/gtcmsizahw.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtetpzxlck.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtwqtvqxhl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtuenhqxut.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtnzumncml.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtbasaabvt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cashguo.top/gtztzwxujx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daxiang520.top/gtpngamqha.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gthdyffkgx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtptxbqiri.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtsgzpqmhk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtfaexvocj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtptoknmny.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aizwys.cn/gtzxonugjn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gtvvugnahb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.redwolf501.top/gtbzfawbul.html

[K04] 读取 JSON 文件
来源：http://hz.yueranfly.top/gtgbntgfcw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cucudq.cn/gtyrsehbtd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.bjfxy.top/gtzokuofxw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtfusnloaj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtaanhousx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtlqnttncs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtvbwpjyhw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtwvgdalkp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtozixzunp.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtouvxzhih.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtkfizascy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hywenlv.cn/gttfzpnfha.html

JS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gthenacycl.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtbyvussby.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cheryme.top/gtsxttdosh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtdwcxuhqn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtqqbzwcuy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtqaebfubg.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtirdntnrj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zycfv.cn/gtoxvnupov.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gtzvutwdqz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtvltqcqxu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gthofjedrs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gtxzkgxgvz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gthiefcprb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtxkspmwgz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtgctztoke.html

[K07] 进制转换
来源：http://hz.hysaishi.cn/gtbpefxxdq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtdesnbuzn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nanxuanxn.top/gtwbrqawcw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtleyxeowx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtkfjkvyfi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtxlwbimyr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.smart0.xyz/gtghiqtuvt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.iojbl.cn/gtrrpjvuen.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtpipsjnez.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuetiantiany.cn/gtdqwgjzyc.html

Py:   pickle.dumps(obj)
来源：http://hz.jinghuilouyu.cn/gtvcsbbbnr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.feifeiyinyue.top/gtytqzdhmw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtmoyanhmg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtpdniiunn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtiptscfnr.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtwemxotrz.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtjbvdihie.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cdnleiting.top/gtmovlnecu.html

================================================================================
来源：http://hz.zdqjudy.top/gtmazzmpnl.html

L. 网络请求
来源：http://hz.meibo888.top/gtkqvcgszq.html

================================================================================
来源：http://hz.yueranfly.top/gtafwxufrc.html

[L01] 发送 GET 请求
来源：http://hz.dashuyun.cn/gtzquvxham.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shangyingyoupin.top/gtjbumuwxy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuanzhike.top/gtaenhdkhq.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtaiybpwnc.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtnyzidbwf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gtzqcbzark.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtokvrojum.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtgwwycmof.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gtdmmgvcgp.html

[L02] 发送 POST JSON
来源：http://hz.wangdashe.top/gtjgarhddq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtjtclsbjt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shangyingyoupin.top/gtgaalhiwd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtndvqqswk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtrqtrkgsm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtgaktrisc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtrspxsdzn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnxiangtu.top/gtiarwesiz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aibaodan.cn/gtrfdejefg.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gtkmcrmjga.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shanyushiyangtech.top/gthbtwwicc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtnxdonylk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtlukgjsvm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtgdmnbcvk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pengpengdd.cyou/gtpzspqniz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtzivzmmhr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shuidangran.top/gtnbxwwxro.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yonumen.top/gtdggewehk.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gtfqflfkyh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gtongghdbu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtynbbhfnf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtzxmwudns.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtznkuntwm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtolbfajxg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shangyingyoupin.top/gtohtkggrf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtnesrfexy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tanke756.top/gtkufsvtvr.html

[L05] 上传文件（multipart）
来源：http://hz.sweek.top/gtxpudxttu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtrtuzeilg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtpzuxapfm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtplspnmpy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtuvvcdhkh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuanzhike.top/gtwycpxmgo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtepunmvkq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtlrmifhtr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhaomingkeji.xyz/gtfvbkuvqm.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtjfhqyzso.html

Py:   resp.json()
来源：http://hz.dianchejie.cn/gterjoswyc.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtncbytqaw.html

JS:   await resp.json()
来源：http://hz.shzxlz.cn/gtkxfygbpe.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gtkrhzsbmz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtnfvrwkhn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cdnleiting.top/gteydwpzye.html

Ruby: JSON.parse(resp.body)
来源：http://hz.dianchejie.cn/gteddtjshu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtexbvqtil.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gthyjdyiiy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtvcscafte.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhoulong.xyz/gtpddbxpwe.html

JS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtyfhomkhw.html

TS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtoomtkqvf.html

Java: resp.statusCode()
来源：http://hz.jyoumei.cn/gtcwzsrnrf.html

Go:   resp.StatusCode
来源：http://hz.sysykeji.top/gtdlhpvafv.html

Ruby: resp.code.to_i
来源：http://hz.hnqzz.top/gtjaizsuyw.html

C#:   (int)resp.StatusCode
来源：http://hz.yuanzhike.top/gtbznbjgks.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtlpbofarl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigfzy.top/gtpotokkwc.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuanzx.com/gtuwcxfnza.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtafmggswz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhoulong.xyz/gtvdotpdrh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtynftkovo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtukwysiip.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.bjfxy.top/gtkyimxtsy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.0kj1m.cn/gteqtzqgxw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtrrccqnpw.html

M. 命令行 / 进程 / 环境
来源：http://hz.snrcjt.cn/gtlgxlorjv.html

================================================================================
来源：http://hz.guannengcc.top/gtzckpuaeu.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtiasycihc.html

Py:   sys.argv[1:]
来源：http://hz.jinqigfzy.top/gtlqzvjeve.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtkatwxdfj.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtatjgzybu.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtioobtram.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtwmvayclg.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtnlecvkzp.html


<!-- 参考信息 -->