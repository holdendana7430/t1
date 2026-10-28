代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gtwdjxrpuq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtickavkgo.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gtvbbbxysy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yueranfly.top/gtmrjifqpf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtfenudloh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gtkzuwxsdi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gteimqreep.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhixingplan.top/gtspezuqvk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinyuanbaomall.cn/gtbkcaigll.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.0kj1m.cn/gtcxvoaviq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnqzz.top/gtzheuipat.html

[I05] 按正则拆分
来源：http://hz.xuanzx.com/gtnwzkavud.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtpupjsceh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhixingplan.top/gtmflyihhq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtxdzxvkjn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtmuirwbza.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhijiandao.cn/gtyovjlmqw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cqqwz.cn/gtvxpjdymm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gthrjagqzh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhixingplan.top/gtnxnzubep.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gtvexlrnxs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtbtvoiger.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtwnjodczv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtvhhyijej.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtqzahauor.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtgpnqrlbp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgufenzy.top/gtupstyelf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.andypj.xyz/gtdqisngxr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtpwqimfaz.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtjukjnfva.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtkmyxzkhm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtthrevcfs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.iojbl.cn/gtgrkzsplr.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtcsomlegv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.bjfxy.top/gtheluulqn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ybcxt.top/gtisjlcoco.html

Ruby: s.scan(/error/i)
来源：http://hz.haohaochexian.top/gtydsizlml.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hammf.cn/gtkpysoeiq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tianlin.xyz/gttlqzbkho.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhijiandao.cn/gtezhtueed.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtifdnbgoi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtbchumonr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtrwbkvmlv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hongshengwenyu.top/gtxrdmykdm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shzxlz.cn/gtspyqxoop.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gthlpqmoor.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gthywhiknm.html

================================================================================
来源：http://hz.cashguo.top/gtmikonxcx.html

J. 日期与时间
来源：http://hz.xuanzx.com/gthjswlfrl.html

================================================================================
来源：http://hz.jinqigufen.top/gtlwjgzere.html

[J01] 获取当前时间
来源：http://hz.tian-w.cn/gtebbhvcbj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aizwys.cn/gtwommuntk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtyncnkcby.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtjvokwpbt.html

TS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtecwpunxp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yanxiufei.cn/gtqogtovnk.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gthehsewll.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtudwkxvjj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guannengcc.top/gtugtlmiun.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtxkkafdhx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtaldwyjge.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtjbayjytr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cashguo.top/gttkwmnalj.html

TS:   d.toISOString()
来源：http://hz.cheryme.top/gtcmjwxxtp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtqepmqtoc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtkijrntfh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtkhjlnfzi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtdaxsfxmu.html

[J03] 字符串解析为日期
来源：http://hz.hammf.cn/gtzdrkrhzk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtvbqfcsni.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtjlsgelrv.html

JS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gttwzcmhhc.html

TS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtimwtacva.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtjnqagenh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenzaomai.com/gtsrvkjdqx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtkqosobgf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtszvgysfj.html

[J04] 时间戳与日期互转
来源：http://hz.birdmap.top/gtoapdlhjk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtsiaiytkw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daria6918.cn/gtvtynbpmp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtgdlamajw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gttfvrrpqr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuanzhike.top/gtbbpvlpfq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtpiqufbkl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtzshfeoqn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yongpay.top/gtxufylbjg.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtvwmirrtt.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtupunbvyt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gteexolzro.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gttqqlnxjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtxxtdphvk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtzochrnay.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxuanxn.top/gtmjejiepr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtcyzwuccw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtlansjttn.html

[J06] 计算两时间之差
来源：http://hz.sysykeji.top/gtxwsecvxk.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtxltpjxge.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtkhzwmnjg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cashguo.top/gtqreeegyh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gtwikcujua.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigufen.top/gtjxyntpfq.html

Go:   end.Sub(start).Hours()
来源：http://hz.aizwys.cn/gtvojcprsg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sweek.top/gtaiuqhtpd.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuanzhike.top/gthbgebzef.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtwidyaqbq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gteithcmwv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtsxnxogqd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yangfankeji.com/gttnzehycy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtxyryrjse.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gthnzwuctx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtbtgbfvfy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtjqutupyp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtgyzdniap.html

[J08] 提取年月日与星期
来源：http://hz.zhoulong.xyz/gtamoeawbz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gturmrtyja.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gtouaylzzf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtilrycvzw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xinyue.icu/gtbyvtgyjp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gtwaoryinv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhixingplan.top/gtqveyvsnd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuxming.cn/gtxvlxwfwv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nwbrower.top/gtvwesszic.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtabeivawp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgfzy.top/gtzeubzmfo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtcmvsqzjk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gthijylpuf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gttfuocjad.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtkavyxqro.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtgyajvtza.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gtvchbvufu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yangfankeji.com/gtozimcdbe.html

[J10] 取今天 / 本月第一天
来源：http://hz.dianchejie.cn/gtcuaiazwx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yueranfly.top/gtfetcsvmn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtqjxesdcl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtymxpscke.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigfzy.top/gtcovfyczp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gthhpeunln.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guowangkeji.top/gtoschlrig.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgfzy.top/gtnbonlyar.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.c1oappe.top/gtijmwtduj.html

================================================================================
来源：http://hz.tian-w.cn/gtperqynif.html

K. JSON 与序列化
来源：http://hz.zhijiandao.cn/gtaugkvobk.html

================================================================================
来源：http://hz.bjfxy.top/gtelmugfis.html

[K01] 对象转 JSON 字符串
来源：http://hz.yangfankeji.com/gtzfcmxfky.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtzykqpsix.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtibdpylmz.html

JS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtdiruetct.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtmcfntktq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtqoxvagtd.html

Go:   json.Marshal(obj)
来源：http://hz.chenlongwang.top/gtkcjwcmpl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gtnhqqvqjp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtazjwwjba.html

[K02] JSON 字符串转对象
来源：http://hz.yueranfly.top/gtmybvgmej.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtzllmwlaz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ehwqpu.com/gtionpuxip.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gthrytkfag.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtagrbvlgv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtdxhabfgs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtamektlhb.html

Ruby: JSON.parse(s)
来源：http://hz.ivvv.top/gtafohmwqa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtagjrecuu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtfyeqcrde.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtmehmadlk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtvexsprse.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtjnkqdxyy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtdfoatgkm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yangfankeji.com/gtwwnprgmg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gtszebpcew.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gteohekdet.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtnxttefqs.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gtqnjvykpr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtczjlwvna.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtqexjvhud.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtdttkbdxm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtravfbngw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtnnuqkkkg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtzirvhgom.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtoxlkaovz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtxvqlapte.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtdhvhcpmz.html

Py:   copy.deepcopy(obj)
来源：http://hz.daria6918.cn/gtlgrcesxc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtgsrfmxpu.html

JS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtoejjyamp.html

TS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtqzodjoyq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydzc1.top/gtjdcowgko.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtcyqteire.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtvfuwvwrl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gttfiakbox.html

[K06] 解析 URL 查询串
来源：http://hz.cheryme.top/gtfczlffng.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtshrghzpj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.svipenyu.cn/gtepvpywtb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtwmxanfmi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtbqtmazzn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtfnppkjcc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtocnbryye.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtcdjapyrm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gtzdeergdc.html

[K07] 进制转换
来源：http://hz.svipenyu.cn/gtshfwvnir.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shzxlz.cn/gtktogyzkc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gogol.net.cn/gtrvedeogp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtnoknrzon.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtjpkchbze.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtvukheweg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gtsgjrqjzh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtvnohxpgy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtoldthvcz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtdsspwkoj.html

Py:   pickle.dumps(obj)
来源：http://hz.daxiang520.top/gtczdzeiri.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yvedp.cn/gtommdluys.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtfqnhdqpe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtiqeaomah.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangtech.top/gtucmtctgh.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtmlpsqeka.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtojofylxf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aizwys.cn/gtxdkbxifp.html

================================================================================
来源：http://hz.nwbrower.top/gtyorkihvx.html

L. 网络请求
来源：http://hz.yj20258.top/gtszopfjur.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtxzrkfnwx.html

[L01] 发送 GET 请求
来源：http://hz.meibo888.top/gtrfpmldvc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.iojbl.cn/gtcznicbue.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guannengcc.top/gtlqdwrazj.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtyahzupem.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtssgijkuq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cdnleiting.top/gtfmhtwfie.html

Go:   resp, err := http.Get(url)
来源：http://hz.yanxiufei.cn/gtbnfltjqc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtvsjurkej.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtguplaeci.html

[L02] 发送 POST JSON
来源：http://hz.jqgfzy.top/gtjluluykd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gtxcyclban.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cucudq.cn/gtuqqezcpw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtctjrzyuc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtcjimzscr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtxghzeopw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xziqi.cn/gtvwxghruz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sysykeji.top/gtevaeyqyz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtsudodklg.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtlucnbyjj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shuidangran.top/gthnyvpyft.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydzc1.top/gtyvkswwnn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtsjyetmoe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtbqxvebsg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtoobwcyvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aizwys.cn/gtfslojdfo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtwqrhkejb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.316326.xyz/gtbziuyvku.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gtyhhilttb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtnkvfvzle.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.52xcode.cn/gtvacoipnw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtdmvtbpoj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtfbrtfgsr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtznjknwsp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhixingplan.top/gtuqhamhry.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhixingplan.top/gtlltespxl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtlcbitnvs.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtewqmfglt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtksqhgosl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daria6918.cn/gtypsidcpy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtyvrxsrcy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtbozxztfz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtylvukwwe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtbdknjjbs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jyoumei.cn/gtvmrodrix.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuanzhike.top/gtkxdktoth.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtmmllfrvj.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtdmtabfum.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtdkhkeozw.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtqhbrmcpr.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gttwkotiag.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtpqzztjdj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangtech.top/gtkgwliamt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtfenqkyyq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtsigrqzkf.html

[L07] 处理 HTTP 状态码
来源：http://hz.daria6918.cn/gtrhtaokda.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtkyytmaqk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gtgstuxgxx.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtfavadjuh.html

TS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtdqtkkdng.html

Java: resp.statusCode()
来源：http://hz.yuanzhike.top/gtqujmfeqt.html

Go:   resp.StatusCode
来源：http://hz.birdmap.top/gtdxzjdjbp.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtmuixhbyi.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gttepuanlw.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtmwrotigc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtduyanwzq.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258.top/gtvkfbhuqt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtvkgztesn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtsevzxjxg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuxming.cn/gtbkeqczqw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cashguo.top/gtwiheicwe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.quarkkingdee.top/gtcmlwqwto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.redwolf501.top/gtjydhpcdm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkloblyev.html

M. 命令行 / 进程 / 环境
来源：http://hz.xylfe.cn/gtcwhtwkoz.html

================================================================================
来源：http://hz.ehwqpu.com/gttpdrvadb.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtkzihyeeh.html

Py:   sys.argv[1:]
来源：http://hz.jinqigfzy.top/gtglsxawsu.html

PHP:  $argv;  $argc;
来源：http://hz.kuanghao11.cn/gtydjljztv.html

JS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gttrydgdtg.html

TS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtidckmpwu.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gtawsljwkg.html

Go:   os.Args[1:]
来源：http://hz.shzxlz.cn/gtgkozwugq.html


<!-- 参考信息 -->