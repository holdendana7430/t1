代发 wailian999

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtpdfgjnhd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gthnvzrhrf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zdqjudy.top/gtdraijjyo.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangtech.top/gtaotseuom.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gtsfzorxca.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtvngaegll.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gturpaaxef.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtetwmltsx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtahcoxdpo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtrhpfuerp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtezhsmyfk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtyqukymeq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daxiang520.top/gtemckxzat.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtlujphhkm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cucudq.cn/gtbemjqclx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtylfbnoea.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtjfgeqvzk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxuanxn.top/gtrlrggroj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pycfn.com/gtbxqcupdw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtukheqbgj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtrtbemuen.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gtjixlrzcc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenlongwang.top/gtigeipfti.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtchvflnvd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jlsjyb.cn/gtrmaeueer.html

TS:   /error/gim
来源：http://hz.sweek.top/gtvicxqbxi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtagtarbfb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtuxcfqpgq.html

Ruby: s.scan(/error/i)
来源：http://hz.smart0.xyz/gtyoxwlmhx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gtnqnjfzzk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigufen.top/gtbdkyutfo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hywenlv.cn/gtzvptmszs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangtech.top/gtgedldlfl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtjacxzpri.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtykzlkxsk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtbkcyuwlv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.iojbl.cn/gtwmruxajj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.feifeiyinyue.top/gtvdclqyvo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtsmcfclvx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqomjdiqt.html

J. 日期与时间
来源：http://hz.daria6918.cn/gtyhpwipns.html

================================================================================
来源：http://hz.svipenyu.cn/gtbwfnguzl.html

[J01] 获取当前时间
来源：http://hz.hywenlv.cn/gtaxivbyox.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtuzsoaknp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtsymeesnk.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtvkvsyjrr.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtjfvvjzqf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zdqjudy.top/gtohzojilq.html

Go:   time.Now()
来源：http://hz.hysaishi.cn/gtwbnvcsra.html

Ruby: Time.now
来源：http://hz.chenzaomai.com/gtmrpjvcwu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtwqxtcgwq.html

[J02] 格式化输出
来源：http://hz.xziqi.cn/gtqtjyklgp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtyxerrxhk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gthuvqvgft.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtfxwjlhmw.html

TS:   d.toISOString()
来源：http://hz.guannengcc.top/gtpznaphpo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gtojzltphj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangshuangyany.cn/gtukchhcuv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtsvywtepq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ppjwa.cn/gtczhbfgya.html

[J03] 字符串解析为日期
来源：http://hz.ydjk.org.cn/gtzvicfadh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hfpthk.cn/gtltcntohb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtcdcgkvwc.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtrcdgnyri.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtrzbfjiar.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gttjlwivsf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.316326.xyz/gtmceaymkj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtoderndxo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtwzltqhkl.html

[J04] 时间戳与日期互转
来源：http://hz.ywan-chungtsiang.top/gtpwrorclt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtktbinkxl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtihdfurcf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.snrcjt.cn/gtxsmqulth.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gtmrwyisei.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtjguegwep.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gtexibvjdg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtrvvxillg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtpgfgqbit.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtgtiqypgh.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gtgjfrpkvu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gtjfkffpxw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtyxnwvfuy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.bjfxy.top/gtkoepghdw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtaeroaosw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtakzcomnw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sxryk.cn/gtpeantkhf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gtondkdzxe.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtrebqfwcq.html

Py:   (end - start).total_seconds()
来源：http://hz.hnxiangtu.top/gtszjfxgky.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtuuagoziw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtqjtscoxa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtcxfmfvgz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtrbkqkgjp.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gthrkrmcxb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtvkpkhkab.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtugbqtivu.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtcdaftrxa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtzulzeqhu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xingfuxueyuan.xyz/gtosyunxrj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtngbecdhh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtjzeldjzs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gteldchxio.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.andypj.xyz/gtqayccuhs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtlvgzbyny.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtquikkasp.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gteyhtcmsr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtgavofbxq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sysykeji.top/gtrqujivxt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.0kj1m.cn/gtngzfydcb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtozqvmtem.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtrlcdzzra.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.svipenyu.cn/gtnenlnvyp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gtsqjrrsiv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jiagoushi.top/gtloizxvzf.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtqfivsozr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtzmjwrgvn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gtqzqhftfa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtpkvbawze.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtsujksnim.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtgfptuool.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.haohaochexian.top/gtkhnjyrfa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtjlsszugq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtawsqcqti.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtkrffqmew.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtjarmdrzr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtackqcebf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jlsjyb.cn/gtpebfqjbc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gotoacloud.top/gtnyjiiyvd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtnbkzernf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhixingplan.top/gtmcfqowut.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgufenzy.top/gthqwzdash.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtwsobhfhx.html

================================================================================
来源：http://hz.chenzaomai.com/gtlrebmpae.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gthkadwkgb.html

================================================================================
来源：http://hz.cucudq.cn/gtmogeuhtd.html

[K01] 对象转 JSON 字符串
来源：http://hz.yangfankeji.com/gtynlajkkl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtkaopxygq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtofvtmmkf.html

JS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtgjhhplct.html

TS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtsnkzmcfy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ehwqpu.com/gtejnwnkwj.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtxydpnxzg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtjopqxvai.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtjnsbfhrq.html

[K02] JSON 字符串转对象
来源：http://hz.mhx1999.top/gtrkxabgjh.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtywjkpwqb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtrwquylgp.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtfnhriflr.html

TS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtimnbquuh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhoulong.xyz/gtunibjzsa.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtkqeswhpw.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtmnggdhhu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj202588.top/gterbgxqfs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hysaishi.cn/gtcnglqnlv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtznnevatv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtotiqyyec.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtctrmjpct.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtcrpihumy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtqrvkigxk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtlgumfhmb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cdnleiting.top/gtporghocc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtrkupahbz.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtxanjrqbq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtqvutieks.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuanzhike.top/gtyowedogp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtrwgxpzmu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtpvkzgehn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gtfmxhpyey.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtklnwgysx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gotoacloud.top/gtulvvlstf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtvalgdxhp.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtrqmscdta.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtsuvevepr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtszautylm.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gteyxhnvno.html

TS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtsjdfnmlw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gtqduqaseb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guannengcc.top/gtlojzymzr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yonumen.top/gtcsozjkqj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ppjwa.cn/gtckiejcgs.html

[K06] 解析 URL 查询串
来源：http://hz.chenzaomai.com/gtiuvtdwot.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.svipenyu.cn/gtkmwmcxbu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shangyingyoupin.top/gtbunfxvjx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtieoacaja.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtunwgnkzd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtajdqohnq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtxkconatw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fzhhl.top/gtbbbusrwq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhengqikj.top/gtsmaiwxkj.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtlhlfzefm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhiwuduotai.top/gtktgucjzq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtvfzyhfcc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtznlwgrhh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtgclscdnu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtyrholhta.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zycfv.cn/gtxpzfgisi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtgcjlclvj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gtvuyfyqoo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtqqfdgqnc.html

Py:   pickle.dumps(obj)
来源：http://hz.jianghu66.top/gtqxcvnlvd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtafjhdmlk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtumntavhy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtmzvejlgs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtophntuuo.html

Go:   encoding/gob
来源：http://hz.jqgufenzy.top/gtdystrimf.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtwdpadtln.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daxiang520.top/gtbdeghsfg.html

================================================================================
来源：http://hz.dashuyun.cn/gtpymmuupy.html

L. 网络请求
来源：http://hz.pycfn.com/gtedxtkpfj.html

================================================================================
来源：http://hz.hfpthk.cn/gtgxzscbze.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtdvzcjhej.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangtech.top/gtmxjnewor.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtngiixymc.html

JS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtlzhdgtjm.html

TS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtpeuekkib.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj202588.top/gtkugnfgra.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gtnadhsdzz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ybcxt.top/gtvcmqjpba.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gtxapasfdl.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtehpkufzr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sufxvd.cn/gtejvwudip.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jiagoushi.top/gteovbwhat.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtolzqizan.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtyvhabsry.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtdtsdwras.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hongshengwenyu.top/gtlgwkxorb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pengpengdd.cyou/gtrcuhzhcz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtsixafezu.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtafcxdrxi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangshuangyany.cn/gtcceuvelu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gtamhjmpnp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gthvwqctfa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtemsjkhfh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtwqdwcahe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gthdymrmbu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhixingplan.top/gtayrvzjms.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtqbslezta.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtteiowhlb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yvedp.cn/gtohndngsz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtykorlhtj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtegedcnhi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtjanwmdez.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daxiang520.top/gtkusbolka.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtfpyvtkaz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.vqdsnc.cn/gtikxzdqtw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtpnevnpbv.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gtpbmsjkec.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guowangkeji.top/gtleeukfia.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gtptskqysn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtcbicsdzt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtwdixqgge.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.bjfxy.top/gtjckcryma.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtpjdoiebo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hywenlv.cn/gtigzexmgf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtgkwfisxm.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gtkdmklcjr.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gteowfxnpc.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtldavgrrk.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtqbpykcto.html

TS:   await resp.json()
来源：http://hz.jyoumei.cn/gthuzzpqwr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sufxvd.cn/gtudxpjkep.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigufen.top/gtucupsyen.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yongpay.top/gtcncghbbl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtewustrhf.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtijbefhhh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gteidvqrdn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.52xcode.cn/gtcumtzbhl.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtjfxajmjz.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gtgaedbuwi.html

Java: resp.statusCode()
来源：http://hz.snrcjt.cn/gtzddgfawo.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtacmcgtap.html

Ruby: resp.code.to_i
来源：http://hz.jinyuanbaomall.cn/gtzmzwmysi.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtylepylpg.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtvaipahhz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtegelivsa.html

PHP:  curl_multi_init() 系列
来源：http://hz.sweek.top/gtmuxnwite.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtkvfkuoyb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtasiflrbf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gtdmigxdgn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gzhubu.top/gtcpcqbgzp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtoehszale.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gtzmqgdips.html

================================================================================
来源：http://hz.zhongyouzk.top/gtingppstc.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtogrfswwp.html

================================================================================
来源：http://hz.sufxvd.cn/gtfrcbfrxo.html

[M01] 读取命令行参数
来源：http://hz.daria6918.cn/gtolzwtzmy.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gterdscevx.html

PHP:  $argv;  $argc;
来源：http://hz.ivvv.top/gtfdcywdqp.html

JS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtzrhupoml.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtbndbeeur.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtsnfqloot.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtioaihlvm.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gttuhhwjgo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtguaxxhhg.html

[M02] 读取环境变量
来源：http://hz.redwolf501.top/gtlnwnjptk.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtdgmmdgly.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gthqnqcsli.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtxqkoyvhv.html

TS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtaxssvdbw.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtuotpuurf.html


<!-- 参考信息 -->