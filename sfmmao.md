代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgfzy.top/gtzbbsibnb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtsimzbzck.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtxggfhzvd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gthuggkitg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gotoacloud.top/gtiovztyka.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.chenjidiqi.icu/gtkecgxiuv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtsmrmykts.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtodnvhrvm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sweek.top/gtgrxhdjvu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gthaobqxzy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtkgrnzytm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtkgcdpctn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gtsmpijhsn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtrrssnzka.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtwodxuujb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtvgrhdote.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtkhufizje.html

[I07] 忽略大小写与多行模式
来源：http://hz.xinyue.icu/gtoomkejla.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhixingplan.top/gtvmilohre.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtdnzjkzps.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daria6918.cn/gtjxbhiqlq.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtueivpcas.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cheryme.top/gtzzvebver.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cashguo.top/gtszhrhpua.html

Ruby: s.scan(/error/i)
来源：http://hz.zhijiandao.cn/gtkuymbvcd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gtfpblomzt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xinyue.icu/gtkstcqwjj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgufenzy.top/gtvxvvtaie.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtiezbjnjf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtcgsuzath.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtktlaofzs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sxryk.cn/gtllaflbbi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtrnwujcid.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gogol.net.cn/gtjfxfsllb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtgxbnjmgh.html

================================================================================
来源：http://hz.svipenyu.cn/gtmyorepou.html

J. 日期与时间
来源：http://hz.cheryme.top/gtuwowkgsi.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtdcaqokro.html

[J01] 获取当前时间
来源：http://hz.snrcjt.cn/gtceyukrim.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtlmpiikxp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtrdpxfwtw.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtfkttqmuh.html

TS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtqfbezohu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gtalcksrnm.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtxohcfybk.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtnhaaevpp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtfnzjpvpd.html

[J02] 格式化输出
来源：http://hz.redwolf501.top/gtmfbjmedq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gtvmsawpll.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtktwormkb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigufen.top/gtohvaicjw.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtwfqavdmu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gtwknycssl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fzhhl.top/gtbsassash.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtrngvvguf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gthxjaazns.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtequrztub.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtczeedceh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shuidangran.top/gtnwgjrcag.html

JS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtknbefwsn.html

TS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtvsfygsvy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtxlrdlyqr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtrwgdxvdk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cashguo.top/gtpojesmyy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtlpskxttn.html

[J04] 时间戳与日期互转
来源：http://hz.ydzc1.top/gtzvojvglr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtfzvbdvnp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtcsudecjd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtkuemfcfv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtcbjifekn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtxvonhcod.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guowangkeji.top/gtsqmlgebc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtgomdqhqe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sysykeji.top/gtdtioclrz.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gtlbxinpgv.html

Py:   now + timedelta(days=7)
来源：http://hz.nanxuanxn.top/gtkzjpiitb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtyecskjfk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtyyltrkko.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtiforrfbe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tian-w.cn/gtfymmdosx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ivvv.top/gtifhpqgoh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gtehaglwwv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtbysuzxvh.html

[J06] 计算两时间之差
来源：http://hz.gzhubu.top/gtmobecqhi.html

Py:   (end - start).total_seconds()
来源：http://hz.pengpengdd.cyou/gttfrpilmj.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtwprboncv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtjbxiutzu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtrhhldfht.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gtekukxpta.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtfciexeja.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtjpdplbbe.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangkeji.top/gtgrqrhtkx.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtvnilsehn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtcwjuwxsp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtazduzaau.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtnpmlkgpn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtndhfmgmt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtpppnxvgu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtilmiivtf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gthuqtbwfv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtyhctlymr.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtdpecwrwg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258888.top/gtghmqejzo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.iojbl.cn/gtnhwdvybd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cashguo.top/gtklwzrjbg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtpenhbmcy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhengqikj.top/gtkezmsyqd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.havefunace.top/gttwaeszck.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtsyqmrboi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtyzzysrqn.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtldmsbhwk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtjsunbpgq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuanzhike.top/gtjtrzycso.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtuwsoudql.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtrtgnycai.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pycfn.com/gtzxcgquxc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtlheficrh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gtkatfyzyh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.0kj1m.cn/gtrpyxbeqs.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtzydujxab.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gtgpeaoddh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gtijhbcvae.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtxmqnmyhr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtgxhkhyup.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jianghu66.top/gtbtllkfwu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtedxhnidj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinghuilouyu.cn/gtapxvshvb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtgwpwjxsr.html

================================================================================
来源：http://hz.bjfxy.top/gtwqshlrwb.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gtlkcrwshn.html

================================================================================
来源：http://hz.daxiang520.top/gtirntiyro.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtxzybmnxn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtcdpaqszr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtrcfnhbik.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtazaitnku.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtdnnmymwc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gtkgxoxqfl.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtwofoepoo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhijiandao.cn/gttujssujz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtuqqhwrdz.html

[K02] JSON 字符串转对象
来源：http://hz.wangdashe.top/gtcbbfuvwy.html

Py:   json.loads(s)
来源：http://hz.zdqjudy.top/gtiekeihos.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtfiwbfost.html

JS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtqsqixpik.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gttozrfzka.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnqzz.top/gtuvktfgga.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtsxxgxjmw.html

Ruby: JSON.parse(s)
来源：http://hz.nwbrower.top/gtindfnmly.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtwniomtsf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gtskrmlwie.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtogybsfqc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtmhkswwpr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtjdoaolbk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtxmljfefx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuxming.cn/gtatxtxupd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtmvpjdqoc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtziyhntnz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtozewroll.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtgepgpjhb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtitwusfni.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtgcumxehr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtlyfucjqu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtcacczzqk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtjkflhlvq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtzfvrpwzg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shangyingyoupin.top/gtcqfhfwls.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtimipqkfs.html

[K05] 深拷贝对象
来源：http://hz.hywenlv.cn/gthimcipnl.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtionjauah.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gtsgrcsabe.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtmislpsog.html

TS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtnwnqrink.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtzdpicwwa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gtltmxjgkd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sxryk.cn/gtooyqfnot.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.0kj1m.cn/gtvzilbjhx.html

[K06] 解析 URL 查询串
来源：http://hz.chenzaomai.com/gtrpjhsmpo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtivrkcdkv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gtzhmwyysc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtbbkdhfco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtwluuvfsk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtqqlcrpox.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtuwihpdyz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigufen.top/gtpwtytrdg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhixingplan.top/gtnysjhgrz.html

[K07] 进制转换
来源：http://hz.c1oappe.top/gtmpllftea.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.mhx1999.top/gtzgyzuetr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtxblpqvko.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtprdedwco.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gticnzwrxr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtdvvmwwbf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtfvppnbny.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigufen.top/gtvqipwthq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtpzcgrarm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.9152youxi.cn/gtdwvhzsgm.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtntgfolzq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtxuthgkwb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtkjugzuar.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtjbpdwgtv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtlbfwpavv.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gtwhugiohp.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gtwxjsnses.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gtyuxyewdk.html

================================================================================
来源：http://hz.nwbrower.top/gtjknjbooo.html

L. 网络请求
来源：http://hz.aibaodan.cn/gtxuwmwosm.html

================================================================================
来源：http://hz.xuanzx.com/gtrtlsvniu.html

[L01] 发送 GET 请求
来源：http://hz.yongpay.top/gtxpexqlnu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtyrnwzvys.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.birdmap.top/gtpewwnrel.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtbqnwrqow.html

TS:   await fetch(url)
来源：http://hz.jqgfzy.top/gtqeoduwad.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.iojbl.cn/gtcnfkyvgs.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtxknhdlif.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.birdmap.top/gtpwleqoiv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cdnleiting.top/gtwakpvbsk.html

[L02] 发送 POST JSON
来源：http://hz.hysaishi.cn/gtjhnmxwna.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtlhrdfagu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.birdmap.top/gtnemnfbbe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtcpvkaauv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtawllafaw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.smart0.xyz/gtbzelgczp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gtfwqrzlyc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hywenlv.cn/gtyrxbjndn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtmcpxxmfi.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtpezoxofj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtrshchoez.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tanke756.top/gtulxmswlm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtjoqjyrqi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gteykokagc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sufxvd.cn/gtbhfpeseo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtlubfcjhw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sxryk.cn/gtavmjhlfy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtoxaaxwph.html

[L04] 设置超时
来源：http://hz.daxiang520.top/gtjljaklhs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtynydqkeo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtjojbwtvs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtdfxwnkdc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtwzkoucsr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtspydowea.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtucqzfpgi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtinktlkiy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gtvewobicc.html

[L05] 上传文件（multipart）
来源：http://hz.sweek.top/gtrghrfssg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtpsdyhmkz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtanzxanfn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtcksjrlmz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtbalcpjcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xingfuxueyuan.xyz/gtqlwkmqkm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.52xcode.cn/gtrvmcexoj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtkzpckncz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnqzz.top/gtqaxlmbit.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gtjykqmpcf.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtyxyzkamh.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtbtappzjh.html

JS:   await resp.json()
来源：http://hz.daxiang520.top/gtibskhrgo.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtjflzzhpp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhoulong.xyz/gtdjjatsdy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.redwolf501.top/gtdyvcltxv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guannengcc.top/gtdqbwzcmc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gttbdekhnu.html

[L07] 处理 HTTP 状态码
来源：http://hz.jiagoushi.top/gthtisodpb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtjnhqbvqm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenjidiqi.icu/gtnrtnmknd.html

JS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtioryejek.html

TS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtclgwaokq.html

Java: resp.statusCode()
来源：http://hz.nanxinkj.top/gtjxpajgbm.html

Go:   resp.StatusCode
来源：http://hz.gzhubu.top/gtepfuhcjs.html

Ruby: resp.code.to_i
来源：http://hz.tian-w.cn/gtvvwfxkdr.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gthmsimexb.html

[L08] 并发请求多个地址
来源：http://hz.nanxinkj.top/gtyrbvnzeo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.kuanghao11.cn/gtczdxiqqo.html

PHP:  curl_multi_init() 系列
来源：http://hz.xinyue.icu/gteluhshxh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtqkhihgoz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gthixekeuu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtitnbtbdk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtmowxxsbf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gtlnptvwqz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sxryk.cn/gtqkpwlvxh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqykguopf.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinghuilouyu.cn/gtucjrtuck.html

================================================================================
来源：http://hz.daxiang520.top/gtzahdnwbt.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtfdkambgk.html

Py:   sys.argv[1:]
来源：http://hz.jiagoushi.top/gtacsfypuc.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtxxptxjxd.html

JS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtqadgvxqb.html

TS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtsvxsuhnf.html

Java: args 数组（main 方法参数）
来源：http://hz.yangfankeji.com/gtmpxsmldu.html

Go:   os.Args[1:]
来源：http://hz.yangfankeji.com/gtxiqrqcud.html

Ruby: ARGV
来源：http://hz.xuanzx.com/gtjhthhark.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dianchejie.cn/gtoggjlkcl.html

[M02] 读取环境变量
来源：http://hz.chenlongwang.top/gtdmimqubd.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gthgzpuidv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gttkktnyna.html

JS:   process.env.HOME
来源：http://hz.ywan-chungtsiang.top/gtabjlnhmk.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtnrkowthr.html

Java: System.getenv("HOME")
来源：http://hz.hnqzz.top/gtwcmxyrdu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtiugfikon.html

Ruby: ENV["HOME"]
来源：http://hz.nanxinkj.top/gtncguciwe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cdnleiting.top/gttiglpbjc.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gtnmqhzcbu.html


<!-- 参考信息 -->