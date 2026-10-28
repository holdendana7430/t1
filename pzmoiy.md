代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtevccslbe.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtqifjkvax.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtkatyuumr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtygcsvuvn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.snrcjt.cn/gtazzuequo.html

TS:   /error/gim
来源：http://hz.zhengqikj.top/gtyyhayrlg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtkdrouhbj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gtocpouxhk.html

Ruby: s.scan(/error/i)
来源：http://hz.kuanghao11.cn/gtxsauamec.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.svipenyu.cn/gtqosnuqup.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gthgxpxvby.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gtczhmngvv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.dianchejie.cn/gtnoesbtvf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gterjohwkh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtpfzthjtd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtxognzymr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtmaubqbdb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daria6918.cn/gtxzowgnwx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtdylmwwwx.html

================================================================================
来源：http://hz.dashuyun.cn/gtfescobzm.html

J. 日期与时间
来源：http://hz.zdqjudy.top/gtnkpriweo.html

================================================================================
来源：http://hz.jyoumei.cn/gtemxakkye.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtvwebkvcl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ehwqpu.com/gtrvbavpdw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtarhiseol.html

JS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtzdqjmcku.html

TS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtskgwvyzv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sweek.top/gtvdkgdsos.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gtdxeuftph.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtoniqdowh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtbtiznvfi.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtqaigaiug.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtmxhzyeix.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtsqqjxkff.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.redwolf501.top/gtubmmjsqp.html

TS:   d.toISOString()
来源：http://hz.yanxiufei.cn/gtbvxztrgm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gttlusnrnp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtsfsypygw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenlongwang.top/gtsxhlrabp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtxgbbcjmp.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtuitspcuq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtkschapjs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtwxqsbyms.html

JS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtixbgicei.html

TS:   new Date("2024-01-02")
来源：http://hz.snrcjt.cn/gtpenkpbwk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtvnuyydxb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtxhrvexil.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj202588.top/gtdywaakwb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zycfv.cn/gtxfdnolgf.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtvjxtymmu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtwceftwsi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuanzhike.top/gtaomjhjre.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtzzjaopqm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gtjfeewqkb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gtxhsfdfqn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hfpthk.cn/gtawdckhkh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.bjfxy.top/gtbgysaxje.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.vqdsnc.cn/gtxwdqxkbr.html

[J05] 时间加减（加 7 天）
来源：http://hz.snrcjt.cn/gtdnprpgzz.html

Py:   now + timedelta(days=7)
来源：http://hz.hammf.cn/gtsbdyvrbg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuxming.cn/gtgwaopsxf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtpfowfaze.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtjrygwrrb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shuidangran.top/gtidesoviy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hammf.cn/gtqywsmdyj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xziqi.cn/gtnkxomity.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gtrlenosah.html

[J06] 计算两时间之差
来源：http://hz.ivvv.top/gtlcrxwdag.html

Py:   (end - start).total_seconds()
来源：http://hz.yongpay.top/gtfbgtfqht.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtiemfzkqq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gaohongyu789.top/gttqvdzbns.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shzxlz.cn/gtvclycmnz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hongshengwenyu.top/gtvmgbmpdh.html

Go:   end.Sub(start).Hours()
来源：http://hz.yonumen.top/gtuykymqxv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zycfv.cn/gtzfmycklu.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhongyouzk.top/gtbctfswck.html

[J07] 比较两个日期
来源：http://hz.yuanzhike.top/gtihbjkvhn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtvwnncvbx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtpsybpdzs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtmuqmslkn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtuawalopd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fzhhl.top/gtjyziselb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.quarkkingdee.top/gtndlfswti.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gteewqkdld.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtmpexmnne.html

[J08] 提取年月日与星期
来源：http://hz.quarkkingdee.top/gtzvttrcxh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sysykeji.top/gtudnfkplv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtzjcopotu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtdfzwvjyn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtxyqgmiiw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtorhlzadb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhongyouzk.top/gtnbbgkgmb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtepptushe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gteoaefeut.html

[J09] 时区处理
来源：http://hz.jiagoushi.top/gthnwdistr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhoulong.xyz/gtdkndmbgu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenjidiqi.icu/gtkkyiordq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtplhyiskd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtjkogapkq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tianlin.xyz/gtpynzyqdj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtrrzdvixb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gtslperkxd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zdqjudy.top/gtxanjjfoi.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtzcmsljjr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtnnktwlxx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhongyouzk.top/gtwyeoodnz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtxaxxsarf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtzpvcidda.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuanzhike.top/gtkltntlua.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gtuweduyqy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gtdfyxzcun.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnxiangtu.top/gtjnpmxijq.html

================================================================================
来源：http://hz.yueranfly.top/gtyvjttejd.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtufxzurqx.html

================================================================================
来源：http://hz.cucudq.cn/gtxcaympng.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtwfhbfolh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtzsulotyc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtxrynwhoh.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtplfyeefu.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtdcktqxnr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guowangkeji.top/gtkifhiicp.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigufen.top/gtrjpfwejs.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtlrvvrzri.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.pengpengdd.cyou/gtgmunnnvd.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gthhtrcfkg.html

Py:   json.loads(s)
来源：http://hz.gotoacloud.top/gtvfmrlrfr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtqrmfposk.html

JS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtcxpumisu.html

TS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtizsifkha.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gtavofkosb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtdipcwesc.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gtnllurrmc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtsgydnfpp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hammf.cn/gtrwqsxthl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtacimoydu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtujgscgnx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtjtjyjcws.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtdqvuuxvq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangshuangyany.cn/gttxxgiztl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yueranfly.top/gtvnorreux.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gtuyzcpdfc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gttqalotqi.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtfhexnlsf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aibaodan.cn/gtsvloftds.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dianchejie.cn/gtlagtnqgi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtxmehattw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtodyxaboz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtzsujznzg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtnhaeftfj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.316326.xyz/gtgaitzzvl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gtqguepwcl.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gttbwzauoh.html

Py:   copy.deepcopy(obj)
来源：http://hz.meibo888.top/gthrlerbob.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gtobinkifo.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtbcofzhzs.html

TS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtcscvfabh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtamofboeg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dashuyun.cn/gtaeissyhy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhiwuduotai.top/gtinrmevbd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.svipenyu.cn/gtsdqvaxbo.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtsouoxvbj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gtbxshczrv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gtacbucjgm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtqoenapsd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtspqsqjvl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxuanxn.top/gtcjedukfe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtekgjzedl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtkthkcnbn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tian-w.cn/gtgdndmzuf.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtkpwmqdws.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtnhgxvrky.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shangyingyoupin.top/gtlbmiykty.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gteoxwfttm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtlytbugwu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtrjmhabsl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhixingplan.top/gtfgvcysii.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhengqikj.top/gtdqloiwua.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gtidditfei.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenjidiqi.icu/gtpsmfqgac.html

Py:   pickle.dumps(obj)
来源：http://hz.cashguo.top/gtdnebrmvd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtnrrcltuf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtrormmfip.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gttxjasqfb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.svipenyu.cn/gtmecwwcop.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtapdgjmto.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gtoxrqgatw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gthxbjtrzl.html

================================================================================
来源：http://hz.dashuyun.cn/gtemuguxzs.html

L. 网络请求
来源：http://hz.yj20258.top/gtmgivhkxn.html

================================================================================
来源：http://hz.ivvv.top/gtnvtaomsn.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtacowrbsz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guowangkeji.top/gtvkmxiqex.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zdqjudy.top/gtjkrgiesa.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtmwdupeos.html

TS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtgyukrrkl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tanke756.top/gttnazbeht.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtqbirfveq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtmzvfmgwg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtjzyxvccm.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtsfryhfpl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtdmoyvqlo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yvedp.cn/gtnnclaiol.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtrahmbvev.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtevidvbmr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtcmcrsvgv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtkmiyxirq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtcllcxxsr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinyuanbaomall.cn/gtbloukezv.html

[L03] 设置自定义请求头
来源：http://hz.yj20258.top/gtzemdzpro.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtujlwizbh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sufxvd.cn/gtixwpdqyb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtfhcxaszi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtikclzxye.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258888.top/gtofrxtfbp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtqdnuvgtc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.svipenyu.cn/gtgliysrcy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.meibo888.top/gttunqwbqs.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtnuzbiuum.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gtyporuvmc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hfpthk.cn/gtruyfntyt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtqadctlqe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtygztgmia.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtfdkoyxud.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fengsongda.top/gtzlbtlvlr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtvaigftjp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhiwuduotai.top/gtiutbwaat.html

[L05] 上传文件（multipart）
来源：http://hz.hywenlv.cn/gtqfwqiuyj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtankiuifp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtqzjwgmcs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtwmnacoqx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtqajlnyrj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtjidfdbao.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xziqi.cn/gtlhowggty.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtpuvcmwxi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shuidangran.top/gtknxsnfbc.html

[L06] 解析响应为 JSON
来源：http://hz.52xcode.cn/gtguhaeeqo.html

Py:   resp.json()
来源：http://hz.yvedp.cn/gtvxelvukh.html

PHP:  json_decode($body, true);
来源：http://hz.ydjk.org.cn/gttqgkahwl.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtbwrzrcob.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtinbspzrr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.vqdsnc.cn/gtcgugtkjn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtqrtfdfdt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cheryme.top/gtdeyvotpm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtcgqliggy.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtusnwkrjp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtniasvwoq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258.top/gtzbaloxkz.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258.top/gttypsldns.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gttvrxkfhf.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gtwtpmbrwu.html

Go:   resp.StatusCode
来源：http://hz.cashguo.top/gtapmfnwjc.html

Ruby: resp.code.to_i
来源：http://hz.shangyingyoupin.top/gtjnstjism.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gthxnwdugz.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtdahebnhu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pycfn.com/gtsmakrvry.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhiwuduotai.top/gtnefajwnn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxuanxn.top/gtbeihnjet.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtzqxnwelm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jianghu66.top/gtocvamgct.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.feifeiyinyue.top/gtdtnnuurx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtxqkobvaw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtldiqflcg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsnlxtcxj.html

M. 命令行 / 进程 / 环境
来源：http://hz.yanxiufei.cn/gtniapobsd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtloigteei.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtwixyfdvj.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gtaqxrrnuk.html

PHP:  $argv;  $argc;
来源：http://hz.cdnleiting.top/gtmoggrjwc.html

JS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtmgtrgmth.html

TS:   process.argv.slice(2)
来源：http://hz.feifeiyinyue.top/gtokwpbkqd.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigufen.top/gtdxywcsdi.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtuqbuvklx.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtnyvdxels.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtcxeudjky.html

[M02] 读取环境变量
来源：http://hz.yvedp.cn/gtqjchetwp.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtdcjjecba.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtibpffevu.html

JS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtjrgwaxgr.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtjiwaccog.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtnymwmcbk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cqqwz.cn/gtzkbspxsy.html

Ruby: ENV["HOME"]
来源：http://hz.aizwys.cn/gtzcvcqzhi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtvfaizvmw.html

[M03] 执行外部命令
来源：http://hz.jinqigufen.top/gtghazpqvx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtgdvfrydt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jianghu66.top/gtuiztvsya.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtqthtnvnv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtvyxkgqdv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtsdewdwdc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sufxvd.cn/gtduwakqcy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sufxvd.cn/gtwugccmxv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hysaishi.cn/gtpplgwvwt.html

[M04] 获取当前工作目录
来源：http://hz.guannengcc.top/gtvpvumdso.html

Py:   os.getcwd()
来源：http://hz.yj20258.top/gttvvwkcgs.html

PHP:  getcwd();
来源：http://hz.52xcode.cn/gtiswrmrpf.html

JS:   process.cwd()
来源：http://hz.zhengqikj.top/gtgxbuwexc.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtfqbcrvui.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuxming.cn/gtrmtzghmr.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtplbitnif.html

Ruby: Dir.pwd
来源：http://hz.jqgufenzy.top/gtaoyfueis.html


<!-- 参考信息 -->