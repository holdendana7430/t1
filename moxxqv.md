代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.nanxuanxn.top/gtdrmsfxcd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtuvhcplzj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtnxadgxev.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtfyavkyls.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jyoumei.cn/gtkvkwfgei.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtcakpbwyz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hammf.cn/gtdpusztny.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtqsvclstf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gthsjbxcmi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtbulaneoq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ydjk.org.cn/gtvuwwdhdl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtivnzseif.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtyznbvrjf.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gttmvghttb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtzuumfgtv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jyoumei.cn/gtlcqwtysg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gtmmyvgtae.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtishsjypo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtdkozthbq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gttbhnacuz.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtukmdhnev.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtmqemmnae.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtxaqdgnav.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtsutkxxcq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yangfankeji.com/gtxktquybv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtnqhjcdjb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.quarkkingdee.top/gtgdpjkyiq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtctlnuwqi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhengqikj.top/gtepoidddi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtbfymwhkl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtunsityty.html

================================================================================
来源：http://hz.hysaishi.cn/gtyiwnyoza.html

J. 日期与时间
来源：http://hz.hysaishi.cn/gtjxppzbtw.html

================================================================================
来源：http://hz.c1oappe.top/gtqwoyfwbh.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtatcokavk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xylfe.cn/gtccsjynnb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gtniyxiwrq.html

JS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtuxjwfrxj.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtqzmbnqxq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.havefunace.top/gtpqruhczt.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtjsmrunuv.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtavbhylct.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtqvectlhn.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtbtetqahb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtntenrvva.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtsleoiuca.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtlifftmoc.html

TS:   d.toISOString()
来源：http://hz.zhixingplan.top/gtbrtizure.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xziqi.cn/gtcdtoljmi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtdbnwjxod.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtdygubpkv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnxiangtu.top/gtqxntgixn.html

[J03] 字符串解析为日期
来源：http://hz.hongshengwenyu.top/gtwqdpryww.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtskopraaz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gtrutbtltw.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtghuqefbh.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtewyuhvhq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtgwirxyow.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nwbrower.top/gtbnpxzflk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtwzkvicvj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtgyslsrpo.html

[J04] 时间戳与日期互转
来源：http://hz.gzhubu.top/gtawvwbtjs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtevwfzbak.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daxiang520.top/gtzwsrjbdd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.bjfxy.top/gtmzkolnlk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gzhubu.top/gtuuyhcxfx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gttdnpacft.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daxiang520.top/gtfhflnnsy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtjqowbbyb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gtdztaifpt.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gtmbmtnytb.html

Py:   now + timedelta(days=7)
来源：http://hz.xuetiantiany.cn/gtdyfxrkuh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuanzx.com/gtumyetvba.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtcjenuxsn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtnzxsmejf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtugabxuap.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtjxqglzqt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtsmgxqrks.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gtawjfnptt.html

[J06] 计算两时间之差
来源：http://hz.redwolf501.top/gtixedfdmx.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtadixcqel.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gtqtxlvztf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtjujdfdiy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gtegskhjqf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtchsucjkg.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtcdfgetan.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtfigwcjnt.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtbwknyilw.html

[J07] 比较两个日期
来源：http://hz.yueranfly.top/gtzqlefwdr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtxjuzamwc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zdqjudy.top/gthfuezfnb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtstmcyuou.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtxiytcyjr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xylfe.cn/gtdorrxqmt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtoginespz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtgkikipqj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtqepjzoml.html

[J08] 提取年月日与星期
来源：http://hz.haohaochexian.top/gtuowhisph.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gtyjfzcnio.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cucudq.cn/gthxvabxmn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ehwqpu.com/gtbyagxfrp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtjnjaanqw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nwbrower.top/gtbmndckth.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuetiantiany.cn/gtgiirnazl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.bjfxy.top/gtfmogvbrl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtdgibrzmp.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtgbcszxut.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtpysazqku.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtlhjhsnvc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ybcxt.top/gtglttyacv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtuylutppa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gtqsgbsmcb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtrepzvurj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtyjkxzmga.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtnsaqyhka.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gtusowzmzd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gteqcgdslv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtnohnrjhy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtocjjdnke.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gthpicnmpx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ywan-chungtsiang.top/gtcitbetfs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.vqdsnc.cn/gtlkgfktjl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gtgncpryoh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnxiangtu.top/gtfyxbglfl.html

================================================================================
来源：http://hz.jinqigufen.top/gtezuwrkey.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gthvkqvymq.html

================================================================================
来源：http://hz.c1oappe.top/gtoywxgyac.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtaqwwsrpd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ivvv.top/gthoyqbzns.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtrczeubid.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtqggnuuor.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtwonkrxkc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtbrltwlwm.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtvaogmfmt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gtwwhxtyto.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtddogfiep.html

[K02] JSON 字符串转对象
来源：http://hz.gogol.net.cn/gtdawwoucy.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gttrmdmtsq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtuiqlctji.html

JS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtpkvcnmzo.html

TS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtcyvgeees.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtunchbodr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtrsypmjdv.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtidsoihwm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuetiantiany.cn/gtjjiferzo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtxozxflew.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtdeilgeeg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtjwwnlkph.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gttigwrcub.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gzhubu.top/gtawgwzqns.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.vqdsnc.cn/gtfqavpmkf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtdiuhgkon.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtlpufuemf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtbthivavk.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gttlamvlay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtvzvlrojj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtbctlatou.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtbuljjiwh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtyixlspqq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtqlrwzgsd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtiygzquji.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtuwjaglbj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtpvsmyivl.html

[K05] 深拷贝对象
来源：http://hz.nanxinkj.top/gtzgwzlxvk.html

Py:   copy.deepcopy(obj)
来源：http://hz.pycfn.com/gtxriwmjmi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtbcspgkxx.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtuhsbrefc.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtmvnpyjxb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xylfe.cn/gtnhhhmxuh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cucudq.cn/gtszuwqlfq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.vqdsnc.cn/gtxadaxnpa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtipqpgzah.html

[K06] 解析 URL 查询串
来源：http://hz.yuanzhike.top/gtslrdwngr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtpsansgte.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cheryme.top/gtunzrnhlx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtmmpwxmte.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtjeysjsdo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhijiandao.cn/gtcljahcvc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtxnremgbo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.snrcjt.cn/gtczjcjbos.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnqzz.top/gtvcmjqdky.html

[K07] 进制转换
来源：http://hz.vqdsnc.cn/gtxbnrorbb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtrvluyolm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zdqjudy.top/gtyhnonodg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtvcqipkth.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtqwbjnhsd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gtunqxpaeo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tanke756.top/gttmidvhxi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shuidangran.top/gtmvtqcmyg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtcmwcdwvp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.9152youxi.cn/gtvgxcbuue.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtlvnhyhty.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gtffaopnya.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.vqdsnc.cn/gtqukneyls.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtxhyumcwg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtnjolhlzk.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtdxeuhlyq.html

Ruby: Marshal.dump(obj)
来源：http://hz.ywan-chungtsiang.top/gtptbzbaql.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.andypj.xyz/gtlgtljbtp.html

================================================================================
来源：http://hz.jinqigufen.top/gtdwaoyqfm.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtlfnmdzoc.html

================================================================================
来源：http://hz.chenlongwang.top/gtczmcdwsg.html

[L01] 发送 GET 请求
来源：http://hz.ivvv.top/gtrjcqpuvu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuxming.cn/gtiewlcorr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.quarkkingdee.top/gtybljssxa.html

JS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtfqoekmls.html

TS:   await fetch(url)
来源：http://hz.vqdsnc.cn/gtsmlysxkc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtjjazbhks.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtljurramb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cqqwz.cn/gtylczxavd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhoulong.xyz/gtnzxutwny.html

[L02] 发送 POST JSON
来源：http://hz.c1oappe.top/gtgnjsncuq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtvwbasqfu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hywenlv.cn/gtxhadmzsh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtjfnzzcte.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtipgfnyoj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtjbkjnyfd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hywenlv.cn/gtzymipgfj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtjzugtmkf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dianchejie.cn/gtwoxuakol.html

[L03] 设置自定义请求头
来源：http://hz.meibo888.top/gtpwifjujs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhongyouzk.top/gtuddctbzf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cucudq.cn/gteliuqfhd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtfubpsmke.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtcwwmsslz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ybcxt.top/gtimyoronh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.mhx1999.top/gtndbcbygs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangkeji.top/gtsqbkntju.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gteelxianq.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtnmpqeahb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.feifeiyinyue.top/gtsnqabybi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuxming.cn/gtkxxqemie.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gttlhoxzrw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtkpkslejn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gthgxhceiv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hysaishi.cn/gtehakxjqa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj202588.top/gtqzhoydbg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nwbrower.top/gttvzpowtj.html

[L05] 上传文件（multipart）
来源：http://hz.svipenyu.cn/gteekkxdlv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgufenzy.top/gtemzrxgtw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtssjbhsiq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtixmzfjmg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtlnlwdrjm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtbcnaiasa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gthptlzpnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtrtyvfmap.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtnbjfyjlj.html

[L06] 解析响应为 JSON
来源：http://hz.zhixingplan.top/gtvcrzhadi.html

Py:   resp.json()
来源：http://hz.sxryk.cn/gtmbfmuhnw.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtdghjbbli.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gtmhotscjy.html

TS:   await resp.json()
来源：http://hz.jiagoushi.top/gtbyfrsyau.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sxryk.cn/gtjgrdaoms.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gtfvxqafkl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtncslcmeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhiwuduotai.top/gthjgjgess.html

[L07] 处理 HTTP 状态码
来源：http://hz.gogol.net.cn/gtnnpuyblz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtaivudyyi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtbtsyjwgg.html

JS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtvfcmrmyl.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtbgnqwcsy.html

Java: resp.statusCode()
来源：http://hz.bjfxy.top/gtovcskokd.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtopxwvkfk.html

Ruby: resp.code.to_i
来源：http://hz.jlsjyb.cn/gtwtcjwicw.html

C#:   (int)resp.StatusCode
来源：http://hz.yj20258.top/gtsfyyekzo.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtovubauxk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtyormcwpc.html

PHP:  curl_multi_init() 系列
来源：http://hz.jiagoushi.top/gtprvatzei.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtcbnbgjfz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtfskwennp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yonumen.top/gtbazyzcyc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fzhhl.top/gtwkexvjho.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtivykqhfb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cashguo.top/gtsuswltti.html

================================================================================
来源：http://hz.jinqigufen.top/gtldyuquea.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtrdtwihyh.html

================================================================================
来源：http://hz.tanke756.top/gtngyxdyhp.html

[M01] 读取命令行参数
来源：http://hz.sysykeji.top/gthunlttyo.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gtjdpkrzmu.html

PHP:  $argv;  $argc;
来源：http://hz.sxryk.cn/gtttwdmouo.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtoooekipc.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtciruagwa.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gtfgwxiidt.html

Go:   os.Args[1:]
来源：http://hz.jinqigufen.top/gtlvbeokkq.html

Ruby: ARGV
来源：http://hz.xingfuxueyuan.xyz/gtyrsvfaze.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gtzxtjgsao.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtixobldwz.html

Py:   os.environ.get("HOME")
来源：http://hz.52xcode.cn/gtqysgharn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtsczfqndt.html

JS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtlpmfpuar.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtsgveeimh.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtoxjkytrb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zycfv.cn/gtafmxujit.html

Ruby: ENV["HOME"]
来源：http://hz.zhengqikj.top/gtflfaamxm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtmacmhhyz.html

[M03] 执行外部命令
来源：http://hz.zhoulong.xyz/gtylujsmis.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daria6918.cn/gtzbfuccvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenjidiqi.icu/gtyreqwqzy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtqhdcbyzb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtyzrobomk.html


<!-- 参考信息 -->