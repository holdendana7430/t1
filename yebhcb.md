代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtizgezdud.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.quarkkingdee.top/gtynsefshb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zdqjudy.top/gtlkgspnjp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuetiantiany.cn/gtbrfqejfl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtuapopnpj.html

[I07] 忽略大小写与多行模式
来源：http://hz.vqdsnc.cn/gtkmmuqbyu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jlsjyb.cn/gtyyrsjhai.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtvhmcawou.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhongyouzk.top/gtjmpdafme.html

TS:   /error/gim
来源：http://hz.bjfxy.top/gtomuhrqav.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhaomingkeji.xyz/gtvzzdynyh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hongshengwenyu.top/gtwjlypxjp.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangtech.top/gtipiuwbpb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgufenzy.top/gtaiznbnmn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnxiangtu.top/gtfmurdjme.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtcwkyfwsb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtqonjxnsc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fengsongda.top/gtjwvwmagw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtbuwooqry.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yongpay.top/gtxwkmvlnv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtalncsuem.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.redwolf501.top/gtpcziqynp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtgvzdzwvy.html

================================================================================
来源：http://hz.pycfn.com/gtydkmrrda.html

J. 日期与时间
来源：http://hz.sysykeji.top/gtlspsyvas.html

================================================================================
来源：http://hz.smart0.xyz/gtmfposzny.html

[J01] 获取当前时间
来源：http://hz.ppjwa.cn/gtvdxsfcqq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gtwugnjeyz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtqyxtxumk.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtnmdakwmd.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtnqdszvia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gotoacloud.top/gtqkmukpuf.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtvffwkekk.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtfqjbbkbo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenlongwang.top/gteiqonduz.html

[J02] 格式化输出
来源：http://hz.snrcjt.cn/gtvikxooal.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtblsgkdwo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtctentioy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cdnleiting.top/gthgkrydyf.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtzdjllmbh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.smart0.xyz/gtsyghbheu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ppjwa.cn/gtdzdaqgqm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtejbykqpa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gtcumxapdg.html

[J03] 字符串解析为日期
来源：http://hz.jinghuilouyu.cn/gtraydpuyz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenzaomai.com/gtahukeiwr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ehwqpu.com/gtjcakrtxa.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtruqeuvtg.html

TS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtdodijaaf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtkifjpzlq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhengqikj.top/gtyntpkdnk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtceeunqsh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zycfv.cn/gtpdpiuijj.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtnozdangl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtdeeomvfl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dashuyun.cn/gtcdvhsiwt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gzhubu.top/gtjmvndubo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gtsjwfftji.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tanke756.top/gtfyjhblog.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtfvadklmg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtzqfbqeyx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.haohaochexian.top/gtcgbudrog.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtpequfywr.html

Py:   now + timedelta(days=7)
来源：http://hz.jlsjyb.cn/gtyayhxuip.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hnqzz.top/gtfqqrvzpn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtxwcigdxj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gthnbezbtg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtenimbmwd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtbscxmmgt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tianlin.xyz/gtvmzhtjhq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gttrwvmsmv.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gtrtlzmrhx.html

Py:   (end - start).total_seconds()
来源：http://hz.ppjwa.cn/gtwlajdsgq.html

PHP:  $end->diff($start)->days;
来源：http://hz.sxryk.cn/gtsuhlgump.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtbxecedow.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtvnqthzys.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtklqgoypt.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtlxuiegeg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sweek.top/gtkptnslto.html

C#:   (end - start).TotalSeconds
来源：http://hz.cucudq.cn/gtsjmvurzz.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gtxlrfwyoz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtuonycpiy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zycfv.cn/gtrhogbcwr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gttwscxmva.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtolnmffez.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aibaodan.cn/gtfebrkulv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtwgoqqfdn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtfvnxiphg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtshoibgac.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtuqgvserb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aibaodan.cn/gtrdiyzfav.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aibaodan.cn/gteeevqqar.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pengpengdd.cyou/gtascdhsym.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtgbkuykvf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shuidangran.top/gttjyclgwx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtsmvzbxfo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xylfe.cn/gtpjdbsaar.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtagzafzub.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtjgkneseh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fzhhl.top/gtikmmkbze.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yvedp.cn/gtxdvifspr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtpucicbst.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtytwygwte.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtqdxlaxyf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gtrjmflsmz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtvtwwunnu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tianlin.xyz/gttbgcjlcc.html

[J10] 取今天 / 本月第一天
来源：http://hz.bjfxy.top/gtjvrrwzuq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gtfrkvjsmr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxuanxn.top/gtffnvecen.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtzfhtdtjh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtucliphia.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhongyouzk.top/gtobesssku.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guowangkeji.top/gtltqprovj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnqzz.top/gthxbvjzop.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gtyektucqg.html

================================================================================
来源：http://hz.xylfe.cn/gtavnxdpcb.html

K. JSON 与序列化
来源：http://hz.pycfn.com/gtdkolohmv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnljkvfdx.html

[K01] 对象转 JSON 字符串
来源：http://hz.tanke756.top/gtofthecxg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtsguoittt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtmniudrwy.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtexovhgkb.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtytjmdrlo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xinyue.icu/gthaomennx.html

Go:   json.Marshal(obj)
来源：http://hz.hnqzz.top/gtsdusyzgu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daxiang520.top/gtuachgeyo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtnvaevfgd.html

[K02] JSON 字符串转对象
来源：http://hz.ehwqpu.com/gtmdjwkctd.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gthdbxunyp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuetiantiany.cn/gtmrtqbnoj.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtpnjqmneg.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gthnnyygcg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangdashe.top/gtppscxmbd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtgezxcsvq.html

Ruby: JSON.parse(s)
来源：http://hz.cheryme.top/gtydfhjxfc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydzc1.top/gttmfmksyy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtjbbxsfbo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtbseolwad.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtrzyiwvru.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtfbydilkr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtzklxjqiv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtdktfabyb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtrgdpdevf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gotoacloud.top/gthgtknagl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtencotqgj.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gtwkddgyds.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangkeji.top/gtzssbvqow.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.9152youxi.cn/gtrtckosad.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtpumawgqt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtygkutziv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aizwys.cn/gtxsoigldh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtxjfnseys.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtrprtflep.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gtanttqvys.html

[K05] 深拷贝对象
来源：http://hz.zhengqikj.top/gtfoizshtm.html

Py:   copy.deepcopy(obj)
来源：http://hz.guannengcc.top/gtclrkypvg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtvnysxipy.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtqevyoudr.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtitfyjthr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.bjfxy.top/gteoofcwku.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhiwuduotai.top/gtepltzzhw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hfpthk.cn/gtisnrutdn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hfpthk.cn/gtppfdmzju.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gttcfsfupv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gtobcyffrs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtusxtwtss.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gttvihhmfx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtbcletixv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fzhhl.top/gtevnsnyop.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtalddsgoj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtpigrpadz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gtmcidpuln.html

[K07] 进制转换
来源：http://hz.wangdashe.top/gtqbywomqs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gtzmfkacsz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnxiangtu.top/gtwtqcptou.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtamwqeylw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtqsqehnkr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtqkmvobcg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gtdzngelrb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhijiandao.cn/gtribryqdi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtpvhfkdfw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhoulong.xyz/gtteeahrve.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtpurapprf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtcxkvmzex.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtxaotflrr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtnyclgybj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gtulqucpit.html

Go:   encoding/gob
来源：http://hz.feifeiyinyue.top/gtwnfngkjw.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtxsvxeyao.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gtugmxnjgj.html

================================================================================
来源：http://hz.zycfv.cn/gtehdkfhdl.html

L. 网络请求
来源：http://hz.zhiwuduotai.top/gtcqixfolm.html

================================================================================
来源：http://hz.ivvv.top/gtojkugzhz.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtrqqjhgga.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangkeji.top/gtidokhilk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtvnubfgso.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtannllzbg.html

TS:   await fetch(url)
来源：http://hz.mhx1999.top/gtdlmhhecj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gaohongyu789.top/gtjphkttpx.html

Go:   resp, err := http.Get(url)
来源：http://hz.tanke756.top/gttshapjtt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.smart0.xyz/gtfwkbtfeu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhengqikj.top/gtaefgdkow.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtqiexzrqq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtywcdfxdr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnqzz.top/gtiyuzbeog.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtbtkpxmcu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtwaliajqk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtessdiznl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gtrkkrlzll.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtxnjfkylt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yongpay.top/gtjromytam.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtsnscndcr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tian-w.cn/gthpgsjahy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhengqikj.top/gtnpjyqagp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtieqrkdyt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtumcacgpc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guowangkeji.top/gtumbhsvlu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtdsacgqqh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtxbxhqouy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ydzc1.top/gtqlofblwo.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtqeesaqgz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gtsipbuxpm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xinyue.icu/gtsiylqdmr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtjacoetsh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtsiyukwbp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtqnnipmty.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtsjkshyjp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangtech.top/gtoijvjybg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gtfqrhigmo.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gtqkawftix.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtfbttjimi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gtuyrkzcrt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtniqmyoye.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sxryk.cn/gtsgedpwqd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtiwexkcgm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.birdmap.top/gtqwqfwqla.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhiwuduotai.top/gtljiluegz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtnkkcrhnv.html

[L06] 解析响应为 JSON
来源：http://hz.zhixingplan.top/gtytgmdgrw.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gtopjzjzdr.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtvxnjqmko.html

JS:   await resp.json()
来源：http://hz.jiagoushi.top/gtmaupuvcx.html

TS:   await resp.json()
来源：http://hz.zhengqikj.top/gtounhctkx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tianlin.xyz/gtoafzlvvs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nwbrower.top/gtvycohjpj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxinkj.top/gtvldvaxdo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtcdvuhyzg.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtigppovcw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daria6918.cn/gtkjaitiof.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhengqikj.top/gtqqucyghk.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtytkhmloi.html

TS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtwjqhnmux.html

Java: resp.statusCode()
来源：http://hz.zhixingplan.top/gtrnmemhpe.html

Go:   resp.StatusCode
来源：http://hz.hywenlv.cn/gtbqepwjsv.html

Ruby: resp.code.to_i
来源：http://hz.jinyuanbaomall.cn/gtwpdvjhzr.html

C#:   (int)resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtuaidjvzr.html

[L08] 并发请求多个地址
来源：http://hz.jinyuanbaomall.cn/gtdrhizzwf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtscsfxcep.html

PHP:  curl_multi_init() 系列
来源：http://hz.havefunace.top/gttskijunn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gttmcrfmog.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtnwycbucg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtotwopvmd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tian-w.cn/gtceuhgqqz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxinkj.top/gtndmcpgcw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gtqbdcpofi.html

================================================================================
来源：http://hz.zdqjudy.top/gtwoienbav.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gtqonmyeqp.html

================================================================================
来源：http://hz.ivvv.top/gtpdqdfpus.html

[M01] 读取命令行参数
来源：http://hz.jianghu66.top/gteuzahnmj.html

Py:   sys.argv[1:]
来源：http://hz.jlsjyb.cn/gttogawoww.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtyjxibgjb.html

JS:   process.argv.slice(2)
来源：http://hz.jinghuilouyu.cn/gtfuwogmtc.html

TS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtatgrtqgo.html

Java: args 数组（main 方法参数）
来源：http://hz.dashuyun.cn/gtspmedsdo.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtndtsvrnn.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtzzsybpjo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtoxnglnqi.html

[M02] 读取环境变量
来源：http://hz.xuanzx.com/gthrwkfjih.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtgrxshhgn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangkeji.top/gtvhvmrrzw.html

JS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtdfaecqjy.html

TS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtucokradm.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtamvhazay.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gtbidvbcwm.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gtpbgswfmf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtgkrqsowi.html

[M03] 执行外部命令
来源：http://hz.hywenlv.cn/gtyrlrmeow.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtyfahqfnr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gogol.net.cn/gtgeerjaxu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtqsqtqddh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gthcyjqvpj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jianghu66.top/gtkhzpwcgr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtckxqipfp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sufxvd.cn/gtmtoyifto.html

C#:   Process.Start("ls", "-l");
来源：http://hz.snrcjt.cn/gtafjybxse.html

[M04] 获取当前工作目录
来源：http://hz.daria6918.cn/gtgtwpqsko.html

Py:   os.getcwd()
来源：http://hz.yj20258.top/gtrokuetsm.html

PHP:  getcwd();
来源：http://hz.shuidangran.top/gthmovawyw.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtffinuony.html


<!-- 参考信息 -->