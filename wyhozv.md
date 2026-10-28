代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gaohongyu789.top/gtmvjxmers.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtiwtiflcr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtwqdjkdaz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gthmutwvyy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pycfn.com/gtsuwxwyru.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtcjtjhzkc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtixeytawi.html

================================================================================
来源：http://hz.chenlongwang.top/gthdzexwlf.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtoygpvptb.html

================================================================================
来源：http://hz.zdqjudy.top/gtdujhuaga.html

[J01] 获取当前时间
来源：http://hz.shuidangran.top/gtgpwvlszd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuetiantiany.cn/gtgyufxgzu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtapxrejdk.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtttzpzirw.html

TS:   new Date();  Date.now()
来源：http://hz.meibo888.top/gtxzvqejry.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tanke756.top/gtauzjxxld.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtbdjtxrxh.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtsrqhwnbo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtudasypej.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtinqzwhzc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtpgscstxi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtuveujwlk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtzliqrhog.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtsyhvhhie.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.9152youxi.cn/gtirvjrnna.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.feifeiyinyue.top/gtejoptxsk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtkkgbnaoq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtpngzydfq.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gtjyvwcndp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtmqwnroka.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yongpay.top/gtccafpado.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtsronyuki.html

TS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtoluupydx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtcmoshdfh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuanzx.com/gtlexbyqcd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj20258888.top/gtmpfjpiyr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gttdevybms.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gtrqqurgsi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtrxnenwdc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258.top/gtigqzzodm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gtgtnwhpel.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtqeloganx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangkeji.top/gthijwugst.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenlongwang.top/gtpfjkmlcb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhiwuduotai.top/gtsncajfps.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtnyljswwh.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigufen.top/gthealmpzt.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtdmjhrngi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtleevteko.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtqpjovaez.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtzmoppqel.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtywcskhdm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtlindiafd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgfzy.top/gtdmhxpose.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydjk.org.cn/gtwekriihl.html

[J06] 计算两时间之差
来源：http://hz.jiagoushi.top/gtevynhxix.html

Py:   (end - start).total_seconds()
来源：http://hz.svipenyu.cn/gtdylevjyp.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gtcoyavtnd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gtzmyfswko.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtothbwaoj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ybcxt.top/gtsfoqrkjo.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtappjludp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shzxlz.cn/gtyugdemif.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtxmmmauyx.html

[J07] 比较两个日期
来源：http://hz.jianghu66.top/gtvpyszfpd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtmnegesbi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtnefdhmdo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtkmrshobw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtsfzudorj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xingfuxueyuan.xyz/gtgmfcxxes.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtepqktvck.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtxvacdhiw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtloadjgzm.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtejhvzrto.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xingfuxueyuan.xyz/gthfftoqcg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gtvykramep.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gthbubhxqe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtaldmnvbm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinyuanbaomall.cn/gtahfwremq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinyuanbaomall.cn/gtysysskcs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gtdhfbotzk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gtzqxzjgue.html

[J09] 时区处理
来源：http://hz.redwolf501.top/gtwguawpoc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gthevaknzk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gtaklrsatp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtcokhvdmt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtedlsplxd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.andypj.xyz/gthmzczrib.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtvgdgnruv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtijuurplc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtghbuvnlk.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtquusajjh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtgzfrjbfm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigfzy.top/gtsmzpdzmq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtvfcthdue.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gtcgqjnqjz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.c1oappe.top/gttykpadjt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtlfowratk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shangyingyoupin.top/gtwmuwshwt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtpyefqtac.html

================================================================================
来源：http://hz.yonumen.top/gtthpclrai.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtzgkdsqnh.html

================================================================================
来源：http://hz.zhongyouzk.top/gtdvpfznhm.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtxsczqwwg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtciqbawuf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtprsmkhtb.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gttnwcbdct.html

TS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtepucfbbm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtilhdaikd.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gtfpvioltl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenlongwang.top/gtvnrkwajc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shuidangran.top/gtfzamdlci.html

[K02] JSON 字符串转对象
来源：http://hz.smart0.xyz/gtvkjtjauy.html

Py:   json.loads(s)
来源：http://hz.shuidangran.top/gtxnrqulwm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gttfpctudm.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtfyzeitdb.html

TS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtidkmzemt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtslomjawi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgfzy.top/gttgslafgo.html

Ruby: JSON.parse(s)
来源：http://hz.sweek.top/gtlhwliizq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtdxfxkfui.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtcgvgtnbg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.316326.xyz/gtxqvndnof.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtwsvqxxau.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtjjpjluyj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtbjwsrwlz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daxiang520.top/gtoexqwvrn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.andypj.xyz/gtqhvivpec.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtldtwbexa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gtablkgyvd.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtrwywsvae.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgfzy.top/gtwnjqenyc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gttmduphrt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtokzdwooa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtpnmiotzd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.vqdsnc.cn/gtipzsmssz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtcntpqtff.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sufxvd.cn/gtrmfyzxoj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gtzeyrmpzt.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gthxfqmxwq.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gtuhgrguiz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtlxrhyqvv.html

JS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtcmijilkt.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtyqvyjwaj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gtexewybcz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenlongwang.top/gtjwvctblb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zycfv.cn/gtbkqvzwlf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtzntruqdo.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtygsxpnff.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtqtakcybf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtdfldeqih.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtbziheblb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtqxoewfio.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtzxwrvwzq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtwxatnqou.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtniyafxvt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cqqwz.cn/gtldctxsbu.html

[K07] 进制转换
来源：http://hz.haohaochexian.top/gtgkngxhix.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtisgjjtjz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangtech.top/gtqrxlxkdk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtmzjjzwea.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtruknzqtr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtlvgqayve.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xylfe.cn/gtsoorrkyw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tianlin.xyz/gttmiwpbzw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sufxvd.cn/gtfzfpymre.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtsjgmvfep.html

Py:   pickle.dumps(obj)
来源：http://hz.ehwqpu.com/gthavidtnm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtdoqfunxa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtjdfbbitn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtrtrbmifg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.andypj.xyz/gtzwopdrps.html

Go:   encoding/gob
来源：http://hz.daria6918.cn/gtrosnhiyu.html

Ruby: Marshal.dump(obj)
来源：http://hz.jianghu66.top/gtogrgefns.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtovfvdbgc.html

================================================================================
来源：http://hz.cdnleiting.top/gtirpiupvm.html

L. 网络请求
来源：http://hz.yongpay.top/gtmcujiqdy.html

================================================================================
来源：http://hz.sxryk.cn/gtkypekmor.html

[L01] 发送 GET 请求
来源：http://hz.ydzc1.top/gtlupbhpyn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gttemqmmeg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtadolxyyc.html

JS:   await fetch(url)
来源：http://hz.fzhhl.top/gtiqmneznq.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtbcgwdlif.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.bjfxy.top/gtkbbpinsw.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gthzprrxkn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gttdbnpcir.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhongyouzk.top/gttvtcqjnt.html

[L02] 发送 POST JSON
来源：http://hz.yangfankeji.com/gtkvasihjj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtianylrrl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hfpthk.cn/gtjuihoaqq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtjfzsmeod.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtfvwpmisp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jqgufenzy.top/gtqcexgzav.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shangyingyoupin.top/gtnjhwvttx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gogol.net.cn/gtjqmadufu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtovnehozx.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtmtkfehgl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhaomingkeji.xyz/gtixtwbrxa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangkeji.top/gttgpvlwgc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtejsdtqtt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtmsakalxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yueranfly.top/gtwmtxnosv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtgeghnams.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.snrcjt.cn/gtwevpijib.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cashguo.top/gtcenzfvjr.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtpevwxsli.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuanzhike.top/gtwwtkhqyh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xziqi.cn/gtouugdlwf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtlfsoeqqb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtevvtgcpb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtamagcoit.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtdkrdfrfr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtlygqlewl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aizwys.cn/gtrlbpkaet.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtdkjbakjm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtcrjmmnxi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jianghu66.top/gtnsnjzvyr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtalgxclsc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtccrhtime.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangdashe.top/gtcznzhhbl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tanke756.top/gtqnpnvubp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtldjddhdt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yonumen.top/gtzwnlfswd.html

[L06] 解析响应为 JSON
来源：http://hz.xylfe.cn/gtgoxrezuz.html

Py:   resp.json()
来源：http://hz.zhijiandao.cn/gtbunchncc.html

PHP:  json_decode($body, true);
来源：http://hz.ehwqpu.com/gtouwjmlpd.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtclhwzfmt.html

TS:   await resp.json()
来源：http://hz.havefunace.top/gtjiklixss.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtfzswvnci.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtpnxdubae.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtzyogoqqd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtlweiszxf.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258888.top/gtjgxxltnh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xziqi.cn/gtfwolefqd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zycfv.cn/gtkxmkwosv.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtcinwjkoc.html

TS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtlpjcevlk.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtilakomku.html

Go:   resp.StatusCode
来源：http://hz.nwbrower.top/gtxrjtzvsk.html

Ruby: resp.code.to_i
来源：http://hz.chenlongwang.top/gtmklqigpj.html

C#:   (int)resp.StatusCode
来源：http://hz.yj202588.top/gtjaklakbr.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtnyocjohr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtlhhxnzrc.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gtyhgavwev.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtsphmcwpj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtkajqvcbr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtzvwvkhsy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cqqwz.cn/gtdofpymrs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtfekkdcah.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.52xcode.cn/gtucqhjbxk.html

================================================================================
来源：http://hz.chenzaomai.com/gtcwjumfvy.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtykhdoxol.html

================================================================================
来源：http://hz.xylfe.cn/gtmxszkvkq.html

[M01] 读取命令行参数
来源：http://hz.sufxvd.cn/gtksmrezsx.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtdlyxjsrr.html

PHP:  $argv;  $argc;
来源：http://hz.andypj.xyz/gtvfldrghu.html

JS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtzovlmyyn.html

TS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtumcinbzd.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtymmtboih.html

Go:   os.Args[1:]
来源：http://hz.gzhubu.top/gtdomflpby.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtqjqxisfe.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhongyouzk.top/gtfmbjkbqj.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gtbgjgswgo.html

Py:   os.environ.get("HOME")
来源：http://hz.haohaochexian.top/gtxqynwiyf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtyyvimekx.html

JS:   process.env.HOME
来源：http://hz.daxiang520.top/gtvskayeur.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtzyqhsyzm.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtwxqyzuvb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtlzduyvqf.html

Ruby: ENV["HOME"]
来源：http://hz.hammf.cn/gtqlmxbbkj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtzoqfkiwf.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtsctmkrti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sweek.top/gtrwrvfaid.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtuogcmuvc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gttpqsushf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtxjyldzvg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhongyouzk.top/gtvozqwtxp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuanzhike.top/gtkhiljsop.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gzhubu.top/gtoxythfvq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gtgqenskbu.html

[M04] 获取当前工作目录
来源：http://hz.zhengqikj.top/gtjynwftir.html

Py:   os.getcwd()
来源：http://hz.yangfankeji.com/gtitatxitk.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtvbmbsqnv.html

JS:   process.cwd()
来源：http://hz.yj20258888.top/gtvinaiczr.html

TS:   process.cwd()
来源：http://hz.yj202588.top/gtbttmxlec.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.c1oappe.top/gtaebwzwim.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtxglhlirn.html

Ruby: Dir.pwd
来源：http://hz.zhongyouzk.top/gtvcctcaok.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhijiandao.cn/gtpyeayyvq.html

[M05] 设置退出码
来源：http://hz.daxiang520.top/gtuxijvwry.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gtstdhljso.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtadqcwwhs.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtgsakdxte.html

TS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtomsckfid.html

Java: System.exit(1)
来源：http://hz.tian-w.cn/gthyoyevak.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtjeepldtr.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gttfvtgqcu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtbwlfslbf.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gtcqhvcpuf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtkfvfbvlc.html


<!-- 参考信息 -->