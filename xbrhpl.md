代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gttojqtrco.html

JS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtydabtong.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtocqbmigl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuanzx.com/gtjzrvzxch.html

Go:   time.Now()
来源：http://hz.zdqjudy.top/gtggsvttis.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtbghewazi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtuqnprget.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtalkikkwl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtwqsdlmco.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtsnepadbi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.smart0.xyz/gtziprlobj.html

TS:   d.toISOString()
来源：http://hz.pengpengdd.cyou/gtviijuylf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtswbqyiph.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daria6918.cn/gteuqgxwee.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtoqpblbeq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxinkj.top/gtdosqdsih.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtwbksagji.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ybcxt.top/gtqfqonohp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtnfvcwkwl.html

JS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtltdhrlmx.html

TS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtydenvouu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj202588.top/gttpicuyah.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xuanzx.com/gtppsxiexq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtjxrnugnn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aizwys.cn/gtbmvcugct.html

[J04] 时间戳与日期互转
来源：http://hz.shzxlz.cn/gtkughpqaf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigfzy.top/gtlbmiiqbw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtfpvtjxhd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenlongwang.top/gtolifoyqj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangtech.top/gtgysghlat.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sxryk.cn/gtpqsamapt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ydzc1.top/gtvcantyty.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gtdytrorsx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgfzy.top/gtjoejiwlu.html

[J05] 时间加减（加 7 天）
来源：http://hz.9152youxi.cn/gtviruwpig.html

Py:   now + timedelta(days=7)
来源：http://hz.hfpthk.cn/gtjqvbygxq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.haohaochexian.top/gtcnbjwqge.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtuugdfjuu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtpjhafill.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtscqxqmrf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gttmayhueb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yueranfly.top/gtyccqfifr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtfwvgdwmt.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtgwlrxnte.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gthecrebpw.html

PHP:  $end->diff($start)->days;
来源：http://hz.ywan-chungtsiang.top/gtztklpkit.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtzonawvpe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtvwydyttx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.meibo888.top/gtthefxtnx.html

Go:   end.Sub(start).Hours()
来源：http://hz.hfpthk.cn/gtmhvjvgos.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangkeji.top/gtljcpkkxy.html

C#:   (end - start).TotalSeconds
来源：http://hz.ehwqpu.com/gtdsmzwzyf.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gtiezydgdr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtixenoaie.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtmwvvelik.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtzoivpupl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtjnejtstn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtsfpbesbk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtnzlydvxv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtrwbgjwvn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gttmvizehi.html

[J08] 提取年月日与星期
来源：http://hz.wangdashe.top/gtspxzeeae.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigfzy.top/gtqkhlvmvl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.0kj1m.cn/gtecijttle.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtiwiyqkob.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhengqikj.top/gtpudsivig.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtwgwewupw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ppjwa.cn/gtyqvmlppi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtazjbemgw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xinyue.icu/gtwxdbhaxs.html

[J09] 时区处理
来源：http://hz.quarkkingdee.top/gteqbjdwot.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ppjwa.cn/gtxyubwhfs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtlhomwyji.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtvtsdfmmz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtgcabxuuq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtdeiskpzp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangdashe.top/gtqiwevevx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtnerrrmwc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtlkstgnev.html

[J10] 取今天 / 本月第一天
来源：http://hz.guowangkeji.top/gtfmuzalwd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtxhglwped.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fengsongda.top/gtssluxwue.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenlongwang.top/gtembgadhp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.snrcjt.cn/gtrfziaazu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenzaomai.com/gtedcqqxcn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.0kj1m.cn/gtdljmefdv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gotoacloud.top/gtbhsdwkdt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.9152youxi.cn/gtvrjuhxwh.html

================================================================================
来源：http://hz.jiagoushi.top/gtwturrbjr.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtpdqohzei.html

================================================================================
来源：http://hz.yuanzhike.top/gtintrivzk.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtxliwgkpo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtkyebkvzo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gticyfyalw.html

JS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtapnsrpig.html

TS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtkpdmdqrd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sweek.top/gtlwrewwlq.html

Go:   json.Marshal(obj)
来源：http://hz.aibaodan.cn/gtpvuzncnt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gtokynhmdw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtvhwpejbr.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtwskcxfwo.html

Py:   json.loads(s)
来源：http://hz.snrcjt.cn/gtgdfcevii.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhengqikj.top/gtcezcbzos.html

JS:   JSON.parse(s)
来源：http://hz.daria6918.cn/gtbsltylrv.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtlvvpqbmo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhaomingkeji.xyz/gtfsgihsgx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtbolhiknl.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gtrtdfjxzh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zycfv.cn/gtipexkush.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.bjfxy.top/gtwdmobrzq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtjeoksssg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtmuitmzem.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gtquwhoepv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtonzrtkss.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gtgytlzccu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtwyeqdmkb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtkvjfjmmd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.quarkkingdee.top/gtrhjavkzr.html

[K04] 读取 JSON 文件
来源：http://hz.ydjk.org.cn/gtetflzfwp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtjnndhnyg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtgdqvjoqo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtfiyeaxmi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtlhsutljl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aibaodan.cn/gtbmhscuqp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtrhzlzjru.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtltytsfeb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtgzxxbnah.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gtmxcbmeua.html

Py:   copy.deepcopy(obj)
来源：http://hz.ppjwa.cn/gtywmayhwb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtliqhulih.html

JS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gthdhjguqz.html

TS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtyeuxebbz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtzbbsowkp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jiagoushi.top/gtnykfnwto.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gthjvkcrod.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shzxlz.cn/gtmolmniqz.html

[K06] 解析 URL 查询串
来源：http://hz.jianghu66.top/gtrkbbfhbz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gtmsbrrxig.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgfzy.top/gtqicbkwhz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gttuinvheo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtavanrwyz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtmayhrpua.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtkxvncgbd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtguodcfuu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtawrczuun.html

[K07] 进制转换
来源：http://hz.hongshengwenyu.top/gtedchleez.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tian-w.cn/gtidtxkmde.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gthrkpfquw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtwyemgysn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtabsdxbnl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtcdmtvbez.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gthcysnjks.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtegjdcckq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtyxxmtixd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hysaishi.cn/gtwkfrcacg.html

Py:   pickle.dumps(obj)
来源：http://hz.snrcjt.cn/gtwnvyhzrh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuanzx.com/gtrqhotezr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtflgorkcw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gttvwwptuw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gtyqpprauz.html

Go:   encoding/gob
来源：http://hz.gzhubu.top/gtnnertmrv.html

Ruby: Marshal.dump(obj)
来源：http://hz.yangfankeji.com/gtvjgsriwy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangshuangyany.cn/gtfobjyzvc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbddvncwq.html

L. 网络请求
来源：http://hz.ivvv.top/gtdtkalpgn.html

================================================================================
来源：http://hz.cqqwz.cn/gtrsibnyxz.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gtziarrsuw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtqdcbjesv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gtfobsrbyt.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtojfkuqtx.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtjftailoo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuxming.cn/gttakviqad.html

Go:   resp, err := http.Get(url)
来源：http://hz.ivvv.top/gtzxnkffsj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gttdwtkgom.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtsbhjcukt.html

[L02] 发送 POST JSON
来源：http://hz.yvedp.cn/gtqjkgioms.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gtcithvpcb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pycfn.com/gtlhpjrsfw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ivvv.top/gtlwawfjay.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtefqpyhwd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258888.top/gtptjouuae.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydjk.org.cn/gtayigopyv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhongyouzk.top/gteuntquwn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhongyouzk.top/gtauaadxcp.html

[L03] 设置自定义请求头
来源：http://hz.jinqigfzy.top/gtivlrkllz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtyddmfvvx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtkthfbxbm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtdrleymhn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtpcpvyhxw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtzdkldfmv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.bjfxy.top/gtbrjmcrke.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.birdmap.top/gthnjygiho.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtjokdojok.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtjnbzlype.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gtscotgvge.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.vqdsnc.cn/gtjbhnhwxl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtivsvhfor.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtqnuykado.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sweek.top/gtnvdzhupl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.316326.xyz/gtoaqjrvxq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258.top/gtzxuwznkr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hysaishi.cn/gtsxvrivzr.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtypbhekgk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenzaomai.com/gtlexfmkll.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.quarkkingdee.top/gtgpcglsdo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtnfujhsif.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtjmzahaxh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtuawlpvlk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gteuizxroi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.bjfxy.top/gtcnurglld.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtujmhwcxc.html

[L06] 解析响应为 JSON
来源：http://hz.guowangkeji.top/gtrbehrtoe.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtwmefuxii.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtvfbxkfmm.html

JS:   await resp.json()
来源：http://hz.sufxvd.cn/gtdrnqamee.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtqwbafyjd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtpvxqvbdf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aizwys.cn/gtvalyfjxl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gtvvkvejhm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtmyrisdtn.html

[L07] 处理 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtwtgyaxkk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigfzy.top/gtaxtsngut.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jlsjyb.cn/gtqvslculo.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtwqjbsnkc.html

TS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gttxfcghas.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gtknnprljs.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtpdlcyqhg.html

Ruby: resp.code.to_i
来源：http://hz.zhengqikj.top/gttgudmnld.html

C#:   (int)resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtqwtxcans.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtaiqmquuw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtwyswvwsi.html

PHP:  curl_multi_init() 系列
来源：http://hz.sufxvd.cn/gthkeqroao.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtuyjgnajr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtkpqqmpqu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jlsjyb.cn/gtriabgohc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xingfuxueyuan.xyz/gtjiyisnmg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtiwwrcscx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gtwsdfmzoh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzxrbmpql.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtibdcoeua.html

================================================================================
来源：http://hz.haohaochexian.top/gtulxwyrdq.html

[M01] 读取命令行参数
来源：http://hz.chenjidiqi.icu/gtecomwbxe.html

Py:   sys.argv[1:]
来源：http://hz.jianghu66.top/gtrsvebvgz.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtmdrjenik.html

JS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtvlyjbhid.html

TS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtkqfjvhdr.html

Java: args 数组（main 方法参数）
来源：http://hz.daria6918.cn/gtikwlqcoz.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtpygtekwx.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtbluzshfg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.redwolf501.top/gteycrmotj.html

[M02] 读取环境变量
来源：http://hz.xylfe.cn/gttffodhpz.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtojnrbfuw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cdnleiting.top/gtilemwgig.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gtqgvbvndn.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtbqnaferm.html

Java: System.getenv("HOME")
来源：http://hz.chenlongwang.top/gtpixiprlk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tanke756.top/gtdvbteumg.html

Ruby: ENV["HOME"]
来源：http://hz.chenjidiqi.icu/gtqpqkejrc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxinkj.top/gtcesiwegm.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtwscmbrmm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gzhubu.top/gtgtpjvxfc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtnqjdtfhd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtqzqnbeei.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtxlvrqice.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigfzy.top/gtqmicrvrj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gtygqjkhum.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.havefunace.top/gtmbzoeuue.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtqwuuxsvx.html

[M04] 获取当前工作目录
来源：http://hz.yongpay.top/gtzsuyjwfi.html

Py:   os.getcwd()
来源：http://hz.jianghu66.top/gtfeopdkxi.html

PHP:  getcwd();
来源：http://hz.snrcjt.cn/gtaxxthmwq.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtsgasditn.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtidysezij.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gtamskiacg.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtqzmfsour.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtgwaqibfh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtxcwblume.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtztzhkhcm.html

Py:   sys.exit(1)
来源：http://hz.snrcjt.cn/gtkmxwysqf.html

PHP:  exit(1);
来源：http://hz.yvedp.cn/gtjhqrvwcn.html

JS:   process.exit(1)
来源：http://hz.tian-w.cn/gtztllhxbb.html

TS:   process.exit(1)
来源：http://hz.xylfe.cn/gtdgmjywpw.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtfsnrumsm.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtybfwayhq.html

Ruby: exit 1
来源：http://hz.jinyuanbaomall.cn/gttbzqtijf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sweek.top/gtjtududxc.html

[M06] 向标准错误输出
来源：http://hz.xuanzx.com/gthqvutgkl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtmpklvdzy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangkeji.top/gtmrjitbqb.html

JS:   console.error("err")
来源：http://hz.daria6918.cn/gtahrgkirk.html

TS:   console.error("err")
来源：http://hz.ybcxt.top/gtmtkktzic.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtykvtwwbb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gtjsnyvpfo.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtbyzyjsbz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jiagoushi.top/gtpiurqwtv.html

[M07] 判断是否为主入口
来源：http://hz.9152youxi.cn/gtqccvhwjp.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtzfnrxjzi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daria6918.cn/gtcftlrhju.html

JS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtoegvyrpn.html

TS:   require.main === module
来源：http://hz.zhengqikj.top/gtrzorbjrk.html


<!-- 参考信息 -->