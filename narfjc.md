代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aibaodan.cn/gtpbxdidbe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtfzwlwgtt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtqcfugpxc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtycryryjy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtghrhhiiv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yanxiufei.cn/gtxuenldqe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtzoowtacp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yangfankeji.com/gtoocghhwm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sufxvd.cn/gthekjjgvm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtvsgoqtwp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxinkj.top/gtmogaexoh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtgoknitzx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xylfe.cn/gttqalfgux.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtswtwustd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.quarkkingdee.top/gtheklhfam.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtjesquvle.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtrhcafugv.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtdufokmsa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hywenlv.cn/gtjcppeuhz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtbqvtodou.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnxiangtu.top/gtgknbrtil.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gthchwxnjs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zycfv.cn/gtfegxczqq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.snrcjt.cn/gtnbxyjtwt.html

Ruby: s.scan(/error/i)
来源：http://hz.chenjidiqi.icu/gtkgpeafkk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtxvjmmpyq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhaomingkeji.xyz/gtsewoeeke.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gtgmgnlohj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gzhubu.top/gtjddveugm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtayiuhtaj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtswiijzfm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xinyue.icu/gtkbomfwmx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.9152youxi.cn/gtueabsvli.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhaomingkeji.xyz/gtmgkbfxhx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.redwolf501.top/gtfzqcrkte.html

================================================================================
来源：http://hz.hywenlv.cn/gtkbbfevow.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gteprdoien.html

================================================================================
来源：http://hz.gzhubu.top/gtfoeqwkzy.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtoanqbqky.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtouiciesz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtzszitfir.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtybppinfq.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtdpjshvza.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtmvuycvnb.html

Go:   time.Now()
来源：http://hz.ydjk.org.cn/gtdkdshbve.html

Ruby: Time.now
来源：http://hz.pengpengdd.cyou/gtnfbhuobo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cashguo.top/gtykwtkcyf.html

[J02] 格式化输出
来源：http://hz.jinqigfzy.top/gtikhtzfuf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gthmltlsxz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtgxeekkrg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yueranfly.top/gtzxlqobdl.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtikddmxlv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gtggjgiiuk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtevkicfsi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtxbelqdxh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtlgkrdqiz.html

[J03] 字符串解析为日期
来源：http://hz.shuidangran.top/gterzwddym.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.feifeiyinyue.top/gtnkhzumug.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.feifeiyinyue.top/gtlwokfhoq.html

JS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtakahglhm.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtdlfinchh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtnymtidkm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtzhhbzsrl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtzjddqncy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.redwolf501.top/gtlezwsrcv.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtuzrcomuk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtopnovzro.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtvosdxexs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cucudq.cn/gtfavqodtw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtsirldfob.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtelmqbbzt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gtddhxmaxy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gtjpjylxhk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gtkvmjqosz.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtpcdqxmmg.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtmiznqsid.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtfxmvfjjr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtrgduhcxr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtelgoclqa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuetiantiany.cn/gtceuphfvy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigfzy.top/gtynghhblh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hongshengwenyu.top/gtvkbsrxej.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gtefhcdyxz.html

[J06] 计算两时间之差
来源：http://hz.fzhhl.top/gtkvfsaton.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgufenzy.top/gtvxmbmjxi.html

PHP:  $end->diff($start)->days;
来源：http://hz.jyoumei.cn/gthxzopwcz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gthcpwekgh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gthmloykbh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtjjmajwng.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtxsghynsc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtlbhedzzi.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtlkvsaszy.html

[J07] 比较两个日期
来源：http://hz.jinghuilouyu.cn/gtnueazhnl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtkqubdbef.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nwbrower.top/gthdlrhqtl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtmazkqwzg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtzjptlxun.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinghuilouyu.cn/gtxuvdgaby.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtjmsamnqx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtdhhhyqir.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtcrkijhtp.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtjcoxwcrx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangshuangyany.cn/gtoafyfkvc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jyoumei.cn/gtfyxayaiy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258.top/gtpzgvjhqh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258.top/gtdbkqybiw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gtvdkfbnbu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhoulong.xyz/gtclxwterl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtolbzziai.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pycfn.com/gttrwndrxo.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtkgqyqxdc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtcxqbpgjw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigfzy.top/gtwotojvpl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtntvkvniu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtelmxuqna.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtzgaipyzw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gttpcpemmr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gtnvrddehn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtqdekxqum.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtcwryxpdl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnqzz.top/gtuiosaqks.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yueranfly.top/gtzlufbpda.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuxming.cn/gtogrgzqop.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtdlwzpeqm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.c1oappe.top/gtmvuibbfg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gtxprdpuim.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtyuljfvjz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtdrtxeomy.html

================================================================================
来源：http://hz.cashguo.top/gtbqgbplnm.html

K. JSON 与序列化
来源：http://hz.ybcxt.top/gthwtviuxm.html

================================================================================
来源：http://hz.jianghu66.top/gtccouysyz.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gtkxydbfuw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtkjptswig.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtjdwomfcn.html

JS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtgcoubafx.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gthfrzbcfc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtbnfexcqj.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gtcwhxaclc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtbobvmobq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.9152youxi.cn/gtfnuaifdv.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtzzzclzkk.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtkaqtnymx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zycfv.cn/gtukhqodcw.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gtavstaadq.html

TS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtzhptdirx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtnwpoljwr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtcfgxdcrv.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtxsaluejx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtrwgfycdw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aizwys.cn/gtvrbvadnl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtvdynatzm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtcndbljob.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtawvqloxs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtnyyacfkm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jlsjyb.cn/gtbajtjkiq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cdnleiting.top/gtdceqhttl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gtuykuekws.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtbucvmpup.html

[K04] 读取 JSON 文件
来源：http://hz.aizwys.cn/gtsznezwvz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangtech.top/gtgerajszz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aizwys.cn/gteksvjwkr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtvvesxxbg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtbcchmynr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtkewhlxno.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtjeignzmc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zycfv.cn/gtbwwswfil.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ppjwa.cn/gtmahplwrl.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtljwhbrho.html

Py:   copy.deepcopy(obj)
来源：http://hz.jiagoushi.top/gtalxpaepe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtasnkokdl.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtxcgfkghx.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtyzrcbpix.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtpgyyptua.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.birdmap.top/gtyrlhsmvk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtebjlkufy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenzaomai.com/gtzlxwdwki.html

[K06] 解析 URL 查询串
来源：http://hz.shangyingyoupin.top/gtqpkgzibt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtraztgcxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pycfn.com/gturyimznd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtdrxskaqy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtckxkgqrw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtuschuqbi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtvaopmufi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cdnleiting.top/gtaawseinp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.316326.xyz/gtkmngeuol.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtyuftvcbc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtqhgpnbto.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gtznzcskgb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gternaoofr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtxhhariav.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtimihrrhp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.tianlin.xyz/gtfbneaavz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gttrskaryx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gtvqkilcvs.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.iojbl.cn/gtdpujjtke.html

Py:   pickle.dumps(obj)
来源：http://hz.yongpay.top/gtokubmrmm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangshuangyany.cn/gtdqjvrhcy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gttetlsrem.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtslahzvcm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.andypj.xyz/gtnwchcuij.html

Go:   encoding/gob
来源：http://hz.snrcjt.cn/gtfzmflxgu.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtmeptybdq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtexaugqkj.html

================================================================================
来源：http://hz.yj202588.top/gtjnzfxawf.html

L. 网络请求
来源：http://hz.fengsongda.top/gttppbnuzp.html

================================================================================
来源：http://hz.aizwys.cn/gtuuilfvii.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtsaoqqhks.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gtfkeokqdk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhixingplan.top/gtxikxwhhi.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtxrvigtco.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtbeiqkjij.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangdashe.top/gtctnvjlnn.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtrutlmour.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtipawnthm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hongshengwenyu.top/gtahtwpvdn.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtxzijogtf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtdyjilchq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtejifqpcc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtlklvjjln.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtivlzlcrf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtfitmwbzx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtubvgczol.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gtyqiiewhp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258.top/gtjgywbhbc.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtwdliypci.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yueranfly.top/gtzfktaiyy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtfdlapigo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtnofsessg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtiimlufik.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtinlhavuu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtgthnsdlh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dashuyun.cn/gtydpwbzrh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtolxembcb.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gtxqdsjrrt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gtqlmldaos.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.mhx1999.top/gtjkhhfsbd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtavqpbipg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtujpotuja.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuanzx.com/gtwvsslvln.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtfyyfbujz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtvupeydoi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtvazcjlrd.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtvyvualzj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ivvv.top/gtbsrnjdan.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gtvgcttghv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtfkevciqp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtlklecdwl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhoulong.xyz/gtdguzofjk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhaomingkeji.xyz/gtqxfggoij.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnxiangtu.top/gthbqjsfis.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zycfv.cn/gtsuadtlyo.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtvmkmwmrv.html

Py:   resp.json()
来源：http://hz.wangdashe.top/gtiwqzgteo.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gtdzebprte.html

JS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtmgtdywlr.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtnxvprxjr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtaayxwvgl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gtxrwgyazr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shangyingyoupin.top/gtzezxpbir.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtsrtmkfqv.html

[L07] 处理 HTTP 状态码
来源：http://hz.0kj1m.cn/gtblmgnblh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.quarkkingdee.top/gtbwkofndp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtpjgdopzi.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtsxnwixzg.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gteywlkmue.html

Java: resp.statusCode()
来源：http://hz.smart0.xyz/gtfuuhsjxa.html

Go:   resp.StatusCode
来源：http://hz.sweek.top/gtucannzxk.html

Ruby: resp.code.to_i
来源：http://hz.meibo888.top/gtodtysofx.html

C#:   (int)resp.StatusCode
来源：http://hz.vqdsnc.cn/gtqknldaub.html

[L08] 并发请求多个地址
来源：http://hz.kuanghao11.cn/gtbevrbzpt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtygodmiji.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtqrmxyieu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtzsjtfrlv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtbtmegozn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgfzy.top/gtjpbzirfd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtywipputc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtjwdlixrl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yongpay.top/gtlizwqjer.html

================================================================================
来源：http://hz.yangfankeji.com/gtrxyqblkd.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gtedvilwro.html

================================================================================
来源：http://hz.cqqwz.cn/gtvcmztcsu.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtcztlgrra.html

Py:   sys.argv[1:]
来源：http://hz.chenzaomai.com/gtczmqfyhm.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtigbvgjzv.html

JS:   process.argv.slice(2)
来源：http://hz.zdqjudy.top/gttdoxoddi.html

TS:   process.argv.slice(2)
来源：http://hz.hfpthk.cn/gtztkovrjd.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtpeidtmbw.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtxlyiohvr.html

Ruby: ARGV
来源：http://hz.jianghu66.top/gtelmwzele.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtpcidstci.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtvcxjoxsh.html

Py:   os.environ.get("HOME")
来源：http://hz.cdnleiting.top/gtbvnngmqf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hywenlv.cn/gtgaonsajx.html

JS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gthfkuwiug.html

TS:   process.env.HOME
来源：http://hz.ydzc1.top/gtcputybhd.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtfxryhxye.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenzaomai.com/gtnvnvnaqo.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gteypsxadu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gthvyhmkjb.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtxwuerhej.html


<!-- 参考信息 -->