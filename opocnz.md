代发 wailian999

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtasmphtfz.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gtlcpzoxrr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.9152youxi.cn/gttaakdlue.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gtgqidhwlu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtzujhbirz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtxblymznl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtnwjtmnxg.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gtdfdgyvlt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtmpqrzfxi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sysykeji.top/gtxzquwgeh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gtvkcgdjxk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cqqwz.cn/gtoeigbbir.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtvemoywhu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hongshengwenyu.top/gtvxjwabjb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtshfmaqfo.html

JS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gteintlnfg.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtpbaldiaz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtmqgcigjq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yonumen.top/gtafkxitkf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtysqzaaem.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gotoacloud.top/gtvtejcaij.html

[J04] 时间戳与日期互转
来源：http://hz.zycfv.cn/gtsuhddiyp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gttvmsulrb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtqtipknfz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtgcirfukd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tianlin.xyz/gtldupbqza.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtgmqtszux.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gaohongyu789.top/gtatzhxfau.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtpqpyouxm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gtiunudgtp.html

[J05] 时间加减（加 7 天）
来源：http://hz.xylfe.cn/gtiuhjpjym.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtuqdwsjei.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hywenlv.cn/gthupcurmv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtclcfeftx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtaxgkfiqj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangdashe.top/gtkxvsyigw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xylfe.cn/gtaugqyjth.html

Ruby: Time.now + 7 * 86400
来源：http://hz.0kj1m.cn/gtmlzuhndh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtlpgxxhqi.html

[J06] 计算两时间之差
来源：http://hz.sxryk.cn/gtzepufiex.html

Py:   (end - start).total_seconds()
来源：http://hz.andypj.xyz/gtxrwvybie.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gtkbimvjhp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtdsvqhrnt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gtmdazsfcy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.redwolf501.top/gtqonoyxas.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtlaopawjd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtlhomitwh.html

C#:   (end - start).TotalSeconds
来源：http://hz.aizwys.cn/gtrtguvjfo.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtcqgkwkht.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtxmocanaj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtpqrtakqa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtegvtgwij.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtmysqydqe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtilerqqfp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pycfn.com/gtsvydpuof.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtsocepxim.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtwfpupqmw.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtrennllon.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenjidiqi.icu/gteonjqitn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtdqhzcopc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.feifeiyinyue.top/gtqzwofjuw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.bjfxy.top/gtowcpqxlv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cucudq.cn/gtfdixthew.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yangfankeji.com/gtrcydvxzf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tian-w.cn/gtxowxclsk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhongyouzk.top/gtpkvtedla.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtjehzikov.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.redwolf501.top/gtxcupcndz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtzfqlmtwi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtobooemjl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtlzlxeouw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.kuanghao11.cn/gtdzxdgrsn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hywenlv.cn/gtsllzyjnu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtrnecsijc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gtxarzowvh.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtfcprtdzc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.52xcode.cn/gtzvgusrwl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cdnleiting.top/gtorjrcfpc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangtech.top/gtmqvaihrj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gtwtcdigan.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gtuquihsmu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ehwqpu.com/gtatjogtxg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtbrfuvevd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhixingplan.top/gtxzctubwu.html

================================================================================
来源：http://hz.sufxvd.cn/gtxzuzymim.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gttzaedsla.html

================================================================================
来源：http://hz.sxryk.cn/gtuqtomlal.html

[K01] 对象转 JSON 字符串
来源：http://hz.cdnleiting.top/gtzunsysrn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtgljydmyh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtdmedmysy.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtkyhunmfi.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtivagosvt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shuidangran.top/gtjxmonfsv.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtonikqwog.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gttwybumll.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ywan-chungtsiang.top/gtzpfybizi.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtnjiccnhv.html

Py:   json.loads(s)
来源：http://hz.yj202588.top/gtnhkgoofy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtowdzpner.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtcfrsjwrj.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtzuhhvkja.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gteznhmodf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtqnpxthoj.html

Ruby: JSON.parse(s)
来源：http://hz.gzhubu.top/gtjxaopzlx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtouvjphkt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtcfibkbtx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtoorrqbjo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtjiocqsvs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtrrmxzyxa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gtaosmgrwo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtqaluftws.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtwvuenbrq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.smart0.xyz/gtvqckxcxg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtlmidzyao.html

[K04] 读取 JSON 文件
来源：http://hz.wangdashe.top/gtdjrxlsve.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtkhhxvrys.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtewurarbf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtczhdvhui.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtijocnhby.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gtphmsbevo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtospzkdgs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj202588.top/gtmsbhnfgj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnqzz.top/gtrxwyhjhl.html

[K05] 深拷贝对象
来源：http://hz.tian-w.cn/gtpmtyzywf.html

Py:   copy.deepcopy(obj)
来源：http://hz.daria6918.cn/gtaojkahgj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtukygreux.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtgnvdibbn.html

TS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gthrxfsucw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ehwqpu.com/gtbuuyprvl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xingfuxueyuan.xyz/gtgkxyacow.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtrnfdkvam.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtthvgapna.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtpdyqnscg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtqoypgbih.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtjnokqmyz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtnnhhzuep.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtxutmfebc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhongyouzk.top/gtxftsgkxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtdjklqyds.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gturbjstym.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtagepdjeu.html

[K07] 进制转换
来源：http://hz.aizwys.cn/gtpqslfjeh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtourlnmwz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.316326.xyz/gtrjyvkick.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtyiqgvalg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtmphzicqd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtwxeockqp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.andypj.xyz/gtjinvnnld.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhongyouzk.top/gtctjmjdxr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hfpthk.cn/gtwhtprkgy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtohlulsii.html

Py:   pickle.dumps(obj)
来源：http://hz.ivvv.top/gtcfbhyckc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhaomingkeji.xyz/gtaldahzgm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtrxklyutd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtsqnxyril.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtpxdbidpr.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtxsyydvdg.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnqzz.top/gtntohkubn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.dashuyun.cn/gtmwvwvnkh.html

================================================================================
来源：http://hz.tanke756.top/gtkiuknvqn.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gttjdzmohc.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwgjywdhf.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtehggfrps.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtfefuoxqj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gaohongyu789.top/gtqgnnoseb.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtvtuqxwnc.html

TS:   await fetch(url)
来源：http://hz.fengsongda.top/gtbnxyzuhq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gtzacwvhxm.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtqhyylmsb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jianghu66.top/gtkhpbxwwy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtpfdaogho.html

[L02] 发送 POST JSON
来源：http://hz.xziqi.cn/gtlabvxrae.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gtqyfxoqbb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtabeqmaox.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtihimcwpg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtwhehctde.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hywenlv.cn/gtkcbwfiqu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sweek.top/gtfifndctq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hywenlv.cn/gtneicypbs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtuhxphrdn.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtyuuaargb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gticlwetuc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtuohbmyrb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtqthsucgr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtrhmklgtr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnqzz.top/gtfsdlhvjj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtkpprapif.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dianchejie.cn/gtjqayxzhb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtobhbridd.html

[L04] 设置超时
来源：http://hz.andypj.xyz/gtuotnalel.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gtzfedbuxe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gtzzapmxpm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtozeaokpy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtqfabfabr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtdrvagxxo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ppjwa.cn/gtgkyckstg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigufen.top/gtvcxrlpya.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.meibo888.top/gtjgglwbpi.html

[L05] 上传文件（multipart）
来源：http://hz.tian-w.cn/gtwlkbqias.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cqqwz.cn/gtgdftioht.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtnakgjbrn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtbjxuhxpl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtmgctulcw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangdashe.top/gtkojzscoq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gogol.net.cn/gtkgnrkyld.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.iojbl.cn/gtvjwptiik.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtlnqahhfz.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtshadlfwn.html

Py:   resp.json()
来源：http://hz.yuanzhike.top/gtswmjyzvc.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtjqljzoxj.html

JS:   await resp.json()
来源：http://hz.hammf.cn/gtnqzmgbcq.html

TS:   await resp.json()
来源：http://hz.fzhhl.top/gtzyxwkrob.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hnxiangtu.top/gtcnxbrshq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxuanxn.top/gtszfjnfcx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtzaltubue.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xziqi.cn/gtvvtvwcyi.html

[L07] 处理 HTTP 状态码
来源：http://hz.ehwqpu.com/gttepumlhd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gteqdxugcv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangshuangyany.cn/gtqlblwacj.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtznuayaau.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtpotpuwvr.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtuvktfvxz.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtvrcnjhln.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtuavoxjkk.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtiwthkybp.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtaluwuaua.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cashguo.top/gtkhvnjjuf.html

PHP:  curl_multi_init() 系列
来源：http://hz.svipenyu.cn/gtgnljzrgh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtjtfumsyu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtwzbadxke.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigfzy.top/gtoxuecxoe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtcuhxevhn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtxlkitoto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ybcxt.top/gtbzwzgxrg.html

================================================================================
来源：http://hz.316326.xyz/gtuqpqggut.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtnaqhbpkz.html

================================================================================
来源：http://hz.guowangkeji.top/gtgibozclw.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtbdadcovg.html

Py:   sys.argv[1:]
来源：http://hz.smart0.xyz/gtyvqdexre.html

PHP:  $argv;  $argc;
来源：http://hz.mhx1999.top/gtvjtvayra.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gthqrfcaer.html

TS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gthutnklpr.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtgnxkugkw.html

Go:   os.Args[1:]
来源：http://hz.jinqigufen.top/gtfoehutzk.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtjbfmeyfi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtcjjyzani.html

[M02] 读取环境变量
来源：http://hz.chenlongwang.top/gtiwbauqvs.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtdvtpqfii.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.bjfxy.top/gtqfnvocub.html

JS:   process.env.HOME
来源：http://hz.hfpthk.cn/gtqlmlqrnh.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtyfttsrxs.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtydtwissd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtmzssxdme.html

Ruby: ENV["HOME"]
来源：http://hz.fzhhl.top/gtkpkprann.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guowangkeji.top/gtdafvfztu.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtjdydhjjo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydjk.org.cn/gtmffivrhu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cucudq.cn/gtjsqrtiuk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtrntovgwe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtzsglwpfx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtzcitqdrl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gaohongyu789.top/gttdqckyei.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtqmyyniku.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gtptnkmpmx.html

[M04] 获取当前工作目录
来源：http://hz.cucudq.cn/gtoosjiact.html

Py:   os.getcwd()
来源：http://hz.daria6918.cn/gthenwbdhz.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtgfaftxyy.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gtwqujhbhj.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtzvugwill.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtkpfxmdoj.html

Go:   os.Getwd()
来源：http://hz.cashguo.top/gtjangjzvd.html

Ruby: Dir.pwd
来源：http://hz.tanke756.top/gtldhessrk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tianlin.xyz/gtiefmiggf.html

[M05] 设置退出码
来源：http://hz.daxiang520.top/gtgcuigyng.html

Py:   sys.exit(1)
来源：http://hz.ydzc1.top/gtdrdqufut.html

PHP:  exit(1);
来源：http://hz.yuxming.cn/gtifonqjjp.html

JS:   process.exit(1)
来源：http://hz.ivvv.top/gtylqgroly.html

TS:   process.exit(1)
来源：http://hz.yongpay.top/gteadorsos.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtvpmffkff.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtivmtfaif.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtkurexmpp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sxryk.cn/gtsdzpfgmu.html

[M06] 向标准错误输出
来源：http://hz.ehwqpu.com/gtqneuwgey.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtxgetrsxu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtwgclngko.html

JS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtqhjcouur.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtqskicsrp.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtlbraemsq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gthqrgtwyz.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtjkhxycpd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sxryk.cn/gtcfcmyjap.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtvzonclil.html

Py:   if __name__ == "__main__":
来源：http://hz.yuanzhike.top/gtfqgfslox.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gthbplenlu.html

JS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtvokjuhgy.html

TS:   require.main === module
来源：http://hz.sweek.top/gtxkxepxvq.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtuoxsglvs.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gtwxlrsqic.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gtftmhuzvp.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtxdivawwm.html


<!-- 参考信息 -->