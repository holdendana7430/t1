代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtbxnomuzk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sysykeji.top/gthrvgzuxb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtapxntkom.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.vqdsnc.cn/gtkqsabxlt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gttyarsakn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtvbadnnvv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.birdmap.top/gtgaghuecs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtmevunxpz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtthakblmg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtzliscrek.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenzaomai.com/gtdpcezfbx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtttpasbhm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtuiwyjtxs.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtdfzjqwdj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtsxeyhera.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuanzhike.top/gtvsmguokf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sweek.top/gtphrirgca.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtckzrzzfs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenjidiqi.icu/gtszjpdrnu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnqzz.top/gtozpzkkih.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtfpkftqxi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtvkpsllwp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtohfnwdqp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.316326.xyz/gtcwxuxoqq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxuanxn.top/gtnuhqamyg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtiinylnwq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtbcmhmnrr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnqzz.top/gtmbubxglk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtauqqrtsc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.iojbl.cn/gtkhmrrmit.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tianlin.xyz/gthjrxlspx.html

================================================================================
来源：http://hz.aizwys.cn/gtbuxgpdpg.html

J. 日期与时间
来源：http://hz.pengpengdd.cyou/gthmzpprpn.html

================================================================================
来源：http://hz.nwbrower.top/gtzfcwlodr.html

[J01] 获取当前时间
来源：http://hz.fzhhl.top/gtlwnkjeed.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtjgjurqje.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtjyuyolzn.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtmzowhhjc.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtbdwvlluc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangshuangyany.cn/gtomekmmnn.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtngfqoidh.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtujqkjmvm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuanzhike.top/gtkoltwovw.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtbupgojcu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtzbfazmcj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtlkqaianc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daria6918.cn/gtfkzcgjfc.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtwlybykdl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cucudq.cn/gttwdxgkoh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jlsjyb.cn/gtytrjrgit.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtaaiiynuk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenlongwang.top/gtmfhvwyew.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtubdargqh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtbavmeaxl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtevzaeuex.html

JS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtrqgdkkdd.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtjkjehnkz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtaeqfwliv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigfzy.top/gtntwpdsuc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtlcqhqzjd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gtlqjfebrd.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigufen.top/gtwmhhdepu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtckxboxgn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cheryme.top/gtepcpkgcd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shzxlz.cn/gtyswgktjf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtszganvsf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.haohaochexian.top/gtekkjgznv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gzhubu.top/gtcvilbdna.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtvsejqcla.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gtryslbxpz.html

[J05] 时间加减（加 7 天）
来源：http://hz.aibaodan.cn/gtkdlrqpgr.html

Py:   now + timedelta(days=7)
来源：http://hz.tianlin.xyz/gtppwevirj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nwbrower.top/gtvnoaxayi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtwfgyhows.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtmteilgjm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtaopitcjb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.smart0.xyz/gtltetzoau.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nwbrower.top/gtqywszdpe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtmaamwzvq.html

[J06] 计算两时间之差
来源：http://hz.chenlongwang.top/gtrtyqkwzy.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtkbbelkbi.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtifpjegjf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtztkscwjh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtbbnmocjo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtghxyotmv.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtbjamsxdv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sweek.top/gtzddzfpze.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuanzhike.top/gtsejgbbbv.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtnzewgkhp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtffarxkiv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hongshengwenyu.top/gtkgpvtagb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtibfiyfei.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtnbshoofp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtykcqcjii.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gttinambiq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtntidbkxz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtologgvjb.html

[J08] 提取年月日与星期
来源：http://hz.cucudq.cn/gtfgfmrnkm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtwvrgzgqf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yangfankeji.com/gtwnazgaqm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtoauizjky.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sweek.top/gtusfnfifq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gthlccwssu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yangfankeji.com/gtsuxcjrws.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtwzxsbbsk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtbepordin.html

[J09] 时区处理
来源：http://hz.yj20258888.top/gtxobodmns.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtcjkfmdwy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258888.top/gtgzapxtse.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtwambparu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtdfxqdzee.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtqqtfmtqu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtbnkzzxgk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gtyntvwerh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fzhhl.top/gtfwfyjqqh.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtowmmkxxk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtqzqwktap.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gtdwedauhn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtqwgajffj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtsokielmo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtekkljksc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtdnisttwl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hongshengwenyu.top/gtnarywrav.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ybcxt.top/gtwewgtcgk.html

================================================================================
来源：http://hz.sxryk.cn/gttdtkxqei.html

K. JSON 与序列化
来源：http://hz.9152youxi.cn/gtkvokvufn.html

================================================================================
来源：http://hz.cucudq.cn/gtbrdojdtl.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhongyouzk.top/gtexiheysl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gtjuumsfjw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtmipgysky.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gturewzsuu.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtswacyrmh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jianghu66.top/gtagtkbllm.html

Go:   json.Marshal(obj)
来源：http://hz.tianlin.xyz/gtsaedpcel.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtdntgfjzv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtarnrfpay.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtkqvxvlyh.html

Py:   json.loads(s)
来源：http://hz.cucudq.cn/gtiadzrnct.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtusoddbop.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtligfhmdm.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gttpiqsszg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtmihqgidn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtwtwzsbxx.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigufen.top/gtwngtqqyw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtvfrfmbxt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtgavzcano.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydzc1.top/gtzstjqnph.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtkettieym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtfbbpdzzo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtfabporls.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xziqi.cn/gtkiztuwgn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yvedp.cn/gtqsfksoku.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gttzqmxsnn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtqakpxris.html

[K04] 读取 JSON 文件
来源：http://hz.jlsjyb.cn/gtxvionecl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258888.top/gtqaislsrm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aizwys.cn/gtvauohhep.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gttmeohulg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtmowflcwp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sweek.top/gtrhbqpjmn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtqhiqdgqc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtyhcfscur.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtlwswpboj.html

[K05] 深拷贝对象
来源：http://hz.zhengqikj.top/gtzxeoibna.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtweztuyxo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sufxvd.cn/gtsmllnsqd.html

JS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtquyfvekg.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gthxajpaxs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinghuilouyu.cn/gtqvctcciy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtewpmhbyz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gtgwhhtcia.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtmfruwkhf.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtrofemjdq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtpsfbheiz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangkeji.top/gtquqcdlmr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtivxzzrzl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtzrqvwlnc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.feifeiyinyue.top/gtandjunww.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtyikvcqpw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtpsiwdnpo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtuuwlgziu.html

[K07] 进制转换
来源：http://hz.hfpthk.cn/gtojldvobb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtgotacuda.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtgqejpdlk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtwjjpvpsd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gthiltvrwj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtgrjdoatr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtppxvhxsj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtosoqszph.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtrtcxkxpp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.vqdsnc.cn/gtgnhvqvua.html

Py:   pickle.dumps(obj)
来源：http://hz.chenzaomai.com/gtsmxbdmtt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.fengsongda.top/gtqmsopfcm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtiniowspl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gttxrbbqky.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtsthfvede.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtwqymtuun.html

Ruby: Marshal.dump(obj)
来源：http://hz.zycfv.cn/gtytlzxvzk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.meibo888.top/gtoobuwjhs.html

================================================================================
来源：http://hz.havefunace.top/gtvnembtoz.html

L. 网络请求
来源：http://hz.hfpthk.cn/gtwdnzqpua.html

================================================================================
来源：http://hz.jqgfzy.top/gttkzfvrhn.html

[L01] 发送 GET 请求
来源：http://hz.aizwys.cn/gtzikxnkud.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtdiohargr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gthssmvdlt.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtpzwzsapz.html

TS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtwrmngejw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtnlfghmcf.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtagsgspvc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtehyvlhbh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtzdzsvrnq.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtipyxshfp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aizwys.cn/gtjslzzmpf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.9152youxi.cn/gtyzpzeswr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gteqetbjqh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtyjijxfrx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xziqi.cn/gtjedmrxhl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gttbvibzlk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hfpthk.cn/gtfwojtzyr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shangyingyoupin.top/gtsyqjiznl.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtvlnndkuu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj20258888.top/gtvwmqtrhj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dashuyun.cn/gtwytsrlkl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtdaptgrxt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtqzdfjmco.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhoulong.xyz/gtsxvgmakm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtqbspmtdk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hfpthk.cn/gtinjecifb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtawahuqdi.html

[L04] 设置超时
来源：http://hz.zhengqikj.top/gtuqotchvj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.9152youxi.cn/gtjyolgreo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtmisxbyxb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtdnivqsao.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtinapvscl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtdmatnkya.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtxlbjoysq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.0kj1m.cn/gtdziyykiy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gttiyjatmg.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtaiivwngi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xziqi.cn/gtukmeclop.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shzxlz.cn/gtowsozygy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtcfdxdvoe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sysykeji.top/gtdpgzotxr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.vqdsnc.cn/gtlqbzqubm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gtpjibxiuq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtgdhaljfj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gttoxstmtg.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtvngpnqhu.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gtbdxwdbmq.html

PHP:  json_decode($body, true);
来源：http://hz.andypj.xyz/gtrmxhtlqu.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gthywqetxl.html

TS:   await resp.json()
来源：http://hz.xziqi.cn/gtpgebhalo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtedzlrclj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtrdmbojgr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtgunckgaz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yangfankeji.com/gtnqsvdyem.html

[L07] 处理 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtcxqwsrpu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gtyvryzdwk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtjoxalslw.html

JS:   resp.ok;  resp.status
来源：http://hz.yuxming.cn/gtfdidvxpu.html

TS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gthhnlsksk.html

Java: resp.statusCode()
来源：http://hz.iojbl.cn/gtfrxuzadp.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtkzqogwbq.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtfjxcpolq.html

C#:   (int)resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtczyepaok.html

[L08] 并发请求多个地址
来源：http://hz.shzxlz.cn/gtrnyrkexw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangtech.top/gtwahenzus.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtaihduppk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtfsaqdrhk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtbovvcxqp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guowangkeji.top/gtkszaelln.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hongshengwenyu.top/gtjfzkibka.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtldqtavkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtvcmmnflr.html

================================================================================
来源：http://hz.sweek.top/gtsuczwdan.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtssxtkebn.html

================================================================================
来源：http://hz.haohaochexian.top/gtnawvnurk.html

[M01] 读取命令行参数
来源：http://hz.ivvv.top/gthibwbdjk.html

Py:   sys.argv[1:]
来源：http://hz.zhiwuduotai.top/gtnlrbubsz.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtvsdzesno.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtcdgiubwi.html

TS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtocvfgdbe.html

Java: args 数组（main 方法参数）
来源：http://hz.yanxiufei.cn/gtwyeyreco.html

Go:   os.Args[1:]
来源：http://hz.sysykeji.top/gtaephqdrp.html

Ruby: ARGV
来源：http://hz.zhijiandao.cn/gtspxgnnaa.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj202588.top/gtmseqxjqa.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangtech.top/gtthhrfnws.html

Py:   os.environ.get("HOME")
来源：http://hz.tanke756.top/gtvqgsohwh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dashuyun.cn/gtqljukqfp.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtjrensntt.html

TS:   process.env.HOME
来源：http://hz.zdqjudy.top/gtkskukjcr.html

Java: System.getenv("HOME")
来源：http://hz.vqdsnc.cn/gtylxueyla.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gthoqseeom.html

Ruby: ENV["HOME"]
来源：http://hz.zhengqikj.top/gtctwbflnm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gtszldxobr.html

[M03] 执行外部命令
来源：http://hz.yueranfly.top/gtjovfuxxo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtuabxlclu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtyxdchrsf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtnxunlqdb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtanjwafnx.html


<!-- 参考信息 -->