代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtmvhsxgsl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yangfankeji.com/gtbeciikcn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.kuanghao11.cn/gtnnkugcno.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.quarkkingdee.top/gttovnrcxm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtnclrkkmk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydzc1.top/gtnummykbd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtgsrczjsa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnqzz.top/gtbhsafkcl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.redwolf501.top/gtgmzaggai.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xziqi.cn/gtsjdpwyfu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtsacbhagc.html

================================================================================
来源：http://hz.xuanzx.com/gthqwrnulv.html

J. 日期与时间
来源：http://hz.tianlin.xyz/gtwkmvuhsm.html

================================================================================
来源：http://hz.cashguo.top/gtjlzpwxkj.html

[J01] 获取当前时间
来源：http://hz.yonumen.top/gtylirsmzz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gtzijyydev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtlwuqdjgu.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gttykvanzr.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtstyyhhgi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sxryk.cn/gtrrkbrszv.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gtmtposenz.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtyjdrcgea.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtsxxfvkkw.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtvmrrgxkm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtvpfbgkud.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtvtqqlovq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenlongwang.top/gtfdohxboy.html

TS:   d.toISOString()
来源：http://hz.0kj1m.cn/gtxobfltpy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtrbhkgpsy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtzhfnisrp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtqzdkkqar.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangshuangyany.cn/gtklrlolyw.html

[J03] 字符串解析为日期
来源：http://hz.zdqjudy.top/gtebtmiepu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gtbdmadean.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtquenhdza.html

JS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtcfnsizxz.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtqidnifrb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtqbvafeuo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.redwolf501.top/gtnwxgmxik.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtlqmerzgh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtpqhsuerr.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtoeaukxhe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sxryk.cn/gtqwmnbhcd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtmmjpcrsa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtoancdejt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenzaomai.com/gtkgyopohf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtwkpwmbkp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gtxfmbcdhm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gotoacloud.top/gtxsshqwxh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sufxvd.cn/gtecoleeya.html

[J05] 时间加减（加 7 天）
来源：http://hz.guannengcc.top/gtwnxbydyf.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtrqsmhjmm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.snrcjt.cn/gtqqaqsdoe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtlmmelbuj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtosobesnz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dianchejie.cn/gtaqiicaob.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuanzhike.top/gtigktuzeo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jianghu66.top/gtbuyxvqfm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtfskqpywy.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gthiqntqxp.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtqifdsphi.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhiwuduotai.top/gthipqcqqm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hysaishi.cn/gtaqoxvuhq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtaplgkywr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtunkvwido.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gtrgwgswji.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuanzhike.top/gthfpkavgy.html

C#:   (end - start).TotalSeconds
来源：http://hz.smart0.xyz/gtmhawienb.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gthebuijcy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtereprfcn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangkeji.top/gtlujacrmj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtxbpdikra.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtjzlegmpn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.vqdsnc.cn/gtdffzsedo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtxkntgymm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtqlcyrszj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtxxhrxmvt.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtxnweiuhw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dianchejie.cn/gtggwtjlex.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gttithysln.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtnhyzkvli.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daria6918.cn/gtzyffxeoi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtwlgxxtqq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtgxjqfxpw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtguwxspec.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtafubbrzt.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtnchbbebs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuanzhike.top/gtmttpjpqy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gtsvsadggu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtkafldcnq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtprplzmsy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtzypnawoj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtoejrhrum.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zycfv.cn/gtzknybkmh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtcabbcxiu.html

[J10] 取今天 / 本月第一天
来源：http://hz.shangyingyoupin.top/gtxdmzenzt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhengqikj.top/gtmyecxrvt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.vqdsnc.cn/gtdfqwfnel.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtffjsgbnx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydzc1.top/gtefbnmzay.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtotjwoigf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtrbrpgouy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtstcxcbul.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guowangkeji.top/gtiiediijp.html

================================================================================
来源：http://hz.yvedp.cn/gtqtfmumek.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtbatstbwx.html

================================================================================
来源：http://hz.yuxming.cn/gtdbywazus.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinghuilouyu.cn/gtdromqavr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gthyzawzjb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtbgxcmjuj.html

JS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtufqogmmg.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtlylxvqyj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gtrqhqzjcs.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gthesfoajr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hysaishi.cn/gtuegbijuo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gtpzeucful.html

[K02] JSON 字符串转对象
来源：http://hz.chenjidiqi.icu/gttsnyjydz.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtwvgcuahw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gttaikmshp.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtxvwtnfcs.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtkqmepekm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gtvxqzyvfk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtwirbkrrl.html

Ruby: JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtwqfezbvz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guowangkeji.top/gtxxdskwgv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtmyqvazef.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtjimvenlh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtithjujlw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtglnrhhof.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtjpuornca.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gtvosqwdpu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtdytitnvq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtombpwxgl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gttgjfuesv.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtthcckaad.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.9152youxi.cn/gtbdtfnazr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sweek.top/gtvorrcpnc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtcwapzqei.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtfmaxkkxe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtqxbzmqev.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtklkpeyjg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtntxjxxck.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtojshiifj.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtoaafxbgw.html

Py:   copy.deepcopy(obj)
来源：http://hz.dianchejie.cn/gtrfuyudkk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.redwolf501.top/gtmnzlyytj.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtztjocqej.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtxdjuxnxj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shuidangran.top/gtlyyqtufn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daria6918.cn/gtxbfyvvqt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtlxcpecgn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhaomingkeji.xyz/gtxvwjaymn.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gtpdxhbvek.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhongyouzk.top/gthbghnwvl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangkeji.top/gtcounrggz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtaepstqhe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtszhazmsq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.andypj.xyz/gtailratga.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.havefunace.top/gtaagsfhlz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gthfdpwwdm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgfzy.top/gtsooeezyv.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtvvvcksuu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtidihaeoq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gtmiehbuce.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtjbeehxfa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtvurjvexq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtfnrrosiw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.quarkkingdee.top/gtbjkeacub.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gtrghrnmxy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gtnidarksx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gaohongyu789.top/gtbpsvoard.html

Py:   pickle.dumps(obj)
来源：http://hz.52xcode.cn/gtdhfruamf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtbwfneyqu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtlzapphhn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gttcuplfjb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gttweutzty.html

Go:   encoding/gob
来源：http://hz.zhongyouzk.top/gtwkfrbxdd.html

Ruby: Marshal.dump(obj)
来源：http://hz.hammf.cn/gthigcqthn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigufen.top/gtihcbumrb.html

================================================================================
来源：http://hz.jinqigufen.top/gtuqznmqpp.html

L. 网络请求
来源：http://hz.yonumen.top/gtquahxeug.html

================================================================================
来源：http://hz.0kj1m.cn/gtqayqidhb.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtsdtkfulu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ehwqpu.com/gtuoptnufz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtnmywoest.html

JS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtawyduyyy.html

TS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtbfdjzbys.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinyuanbaomall.cn/gtltflqatl.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtktuuurqe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenzaomai.com/gtnbuubiik.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shanyushiyangtech.top/gtiibkwnes.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtgflyhzzq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gtlmaargkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dashuyun.cn/gttwjmqfsh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtxlapasmc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtuxengwvo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtmxbrfznk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtfuntmixe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtakcfwiaq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtrsubycea.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtmiqwphyy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtzmlyvjgs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258888.top/gtkkwlvytl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtvnbziibe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtmzesvxid.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.9152youxi.cn/gtusnblyvx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtmyjgblzh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cucudq.cn/gtaftpkpmy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtvzeimaug.html

[L04] 设置超时
来源：http://hz.zhaomingkeji.xyz/gtvrgebgjf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtudhdvqwr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.c1oappe.top/gtiukgydao.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtpuqnmqzx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtzlowjttz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtuvduxwhg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shangyingyoupin.top/gtffjfqvoz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnqzz.top/gteikjrzaa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtipsahsld.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gtbdnvlhxg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtozjrpktc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.smart0.xyz/gtivnhmdqh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtvkgysnvh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtdmvtztml.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtniaewniz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtnxnibrsw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gticueizvw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtvtaytavf.html

[L06] 解析响应为 JSON
来源：http://hz.svipenyu.cn/gtqlcdkiij.html

Py:   resp.json()
来源：http://hz.cqqwz.cn/gtewalesow.html

PHP:  json_decode($body, true);
来源：http://hz.cqqwz.cn/gtotqhmgnt.html

JS:   await resp.json()
来源：http://hz.jqgufenzy.top/gtpifnfzhq.html

TS:   await resp.json()
来源：http://hz.316326.xyz/gtzkniaojo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtiaqcvfcc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhixingplan.top/gtpvqvazfy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtfhyetvfz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtgfkeheis.html

[L07] 处理 HTTP 状态码
来源：http://hz.xinyue.icu/gtliabfjjx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gthytgruyi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shangyingyoupin.top/gtwzttvbwm.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtbpgyggsi.html

TS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtreshmvfr.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangtech.top/gtpotmkfcv.html

Go:   resp.StatusCode
来源：http://hz.jianghu66.top/gtzgmvubfu.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtzatgppnd.html

C#:   (int)resp.StatusCode
来源：http://hz.xziqi.cn/gtqjqsdmke.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtpbxavqrl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.9152youxi.cn/gtavepesiw.html

PHP:  curl_multi_init() 系列
来源：http://hz.pengpengdd.cyou/gtpxvyeldo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtrifivaoi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtmkgabuur.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhaomingkeji.xyz/gtjpouuhke.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gthceierdk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtwnvrwnul.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tian-w.cn/gtivmzkxvf.html

================================================================================
来源：http://hz.hammf.cn/gtyptdjdsi.html

M. 命令行 / 进程 / 环境
来源：http://hz.tianlin.xyz/gtqcskdnnp.html

================================================================================
来源：http://hz.9152youxi.cn/gttgzltsts.html

[M01] 读取命令行参数
来源：http://hz.mhx1999.top/gtrtdhesmq.html

Py:   sys.argv[1:]
来源：http://hz.xinyue.icu/gtarcrnedh.html

PHP:  $argv;  $argc;
来源：http://hz.xinyue.icu/gtgeudzhlp.html

JS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtrpsxlscj.html

TS:   process.argv.slice(2)
来源：http://hz.shzxlz.cn/gthsjlgebe.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtibuorjvu.html

Go:   os.Args[1:]
来源：http://hz.jyoumei.cn/gttxjudrjo.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtvcottekq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yangfankeji.com/gtunplijok.html

[M02] 读取环境变量
来源：http://hz.jqgufenzy.top/gtxvfyodwo.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtzpcchqgz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtndvvbtey.html

JS:   process.env.HOME
来源：http://hz.andypj.xyz/gtnrayfwup.html

TS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtyqjgzomx.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtcpfxtyeh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gttsqfereq.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gttxoojvak.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gtzfvblhzl.html

[M03] 执行外部命令
来源：http://hz.xinyue.icu/gtgwwfkvli.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenjidiqi.icu/gticfrcjph.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtqtvcqgzt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtphevctlr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gthkdhfpoj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtopwjwqih.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtxijnlqjy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtwwmrwypm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtfswhowzz.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gtvtdkpsvz.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtcfkhypou.html

PHP:  getcwd();
来源：http://hz.jianghu66.top/gtgolpvill.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtaavpfqfd.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtebmvwlxf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.iojbl.cn/gtsktfeycp.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtubggjmnz.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtfvqpakul.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtsjaiazrv.html

[M05] 设置退出码
来源：http://hz.jyoumei.cn/gtcvmrdqmd.html

Py:   sys.exit(1)
来源：http://hz.jianghu66.top/gtuzegeosy.html

PHP:  exit(1);
来源：http://hz.cqqwz.cn/gtbilwwbui.html

JS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtxakcqcmp.html

TS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtklhqqrae.html

Java: System.exit(1)
来源：http://hz.tian-w.cn/gtsdtxdryu.html

Go:   os.Exit(1)
来源：http://hz.cdnleiting.top/gtmrtsldsu.html


<!-- 参考信息 -->