代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtxrualnbo.html

JS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtgumfsqtx.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gttvbgtpdj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtzlnfbpso.html

Go:   time.Now()
来源：http://hz.shanyushiyangtech.top/gtevstqyum.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtamjexvwn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtjzrvrcsv.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtirxqttmz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtiauodrrz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gttkcyecwy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.quarkkingdee.top/gtufvbqtzz.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gteheknxgo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.iojbl.cn/gtblfolrgb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gthbguhobh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtjnilrmnr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.svipenyu.cn/gtvgdsmvie.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtniuzidex.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtokumrllh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgfzy.top/gtydpmqufk.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtpwfsstnz.html

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtxofxckpb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtgmigsghw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.haohaochexian.top/gtttakdwhm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtbsqsomnm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtqvyocknl.html

[J04] 时间戳与日期互转
来源：http://hz.nanxuanxn.top/gtmmswbeht.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhiwuduotai.top/gtkuczffah.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.redwolf501.top/gthakyhrdu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sweek.top/gtpnwyiibu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.c1oappe.top/gttxqdpzmt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.dashuyun.cn/gtkwejrvzf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gtfvmbirro.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxuanxn.top/gtlhfxkuiz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtokirmrgp.html

[J05] 时间加减（加 7 天）
来源：http://hz.dashuyun.cn/gtnbnomllr.html

Py:   now + timedelta(days=7)
来源：http://hz.zdqjudy.top/gtjzgemlwp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtdrhhkxyh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtrhivbgny.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtuaqehoff.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cucudq.cn/gttyjqnbib.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yueranfly.top/gtxzindccz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtimyiprvj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nwbrower.top/gtsjqfmdxh.html

[J06] 计算两时间之差
来源：http://hz.svipenyu.cn/gttzabygql.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtfaeibfcw.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhongyouzk.top/gtxhebpcbp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtbfzvhfdr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tanke756.top/gtgblrjcke.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtuhxjjexl.html

Go:   end.Sub(start).Hours()
来源：http://hz.ehwqpu.com/gtmrtmlfyg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtjlofdcbs.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gtioofpddc.html

[J07] 比较两个日期
来源：http://hz.cucudq.cn/gtjqzkimcc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtobwzdmix.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.52xcode.cn/gtfupwxshg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtmsggttyi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtibtadsiq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtolbkcipr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pengpengdd.cyou/gtxeohjzbg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtckkobjkm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtlwklmufc.html

[J08] 提取年月日与星期
来源：http://hz.pycfn.com/gttwogcucr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tian-w.cn/gtkppkkdpe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ehwqpu.com/gthxvaenvt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tianlin.xyz/gtyevzqlbw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gthmwdooph.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtovfwqjjs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtotrclqwh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtxxrshmoy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gtxubwafcc.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gthyaohglw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daxiang520.top/gtzjnqwnal.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtriztwlvv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtdowfgtrt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gttnixunxb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cashguo.top/gtpnzmmsrm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dianchejie.cn/gtmuthyeki.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtykkhquhg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.pycfn.com/gtcztivbcz.html

[J10] 取今天 / 本月第一天
来源：http://hz.guannengcc.top/gtitwgvlyn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hammf.cn/gtcawfywkq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtjuygbrny.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yongpay.top/gtvzcdnwto.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258.top/gtjvnqjubq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinyuanbaomall.cn/gtmyzngwka.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtuoqaisra.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtazjvtthv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daxiang520.top/gtciudneqj.html

================================================================================
来源：http://hz.svipenyu.cn/gtlgqzfyor.html

K. JSON 与序列化
来源：http://hz.tanke756.top/gtwoidqedy.html

================================================================================
来源：http://hz.snrcjt.cn/gtragvumpk.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtenenwlme.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtuygpeupo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtrvjyioir.html

JS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtbumvnucc.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtjhqjxdmm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.meibo888.top/gtymsrvczr.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258.top/gtgoewfbyw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtkjytukna.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ybcxt.top/gtjykpyknr.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangkeji.top/gtbdovnghz.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtpvklttxz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shangyingyoupin.top/gtjvlgalwx.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtfroxmtsq.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gthpahcrzi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yuxming.cn/gtoeiuigag.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtnprirrul.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtmolwbqas.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigfzy.top/gtzvlzuaob.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtkozseaxd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtvkpjnapv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtyhawmuvc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtpwoprzfd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtgyuqabyp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gotoacloud.top/gtynbxurwi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fzhhl.top/gtiuapfpup.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.andypj.xyz/gtbpavtiin.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangkeji.top/gtevuoucwh.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtftdzpoay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gtmwqkzgiq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shuidangran.top/gtqcdcpsyc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtijmygsen.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtasxrqbkt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xuetiantiany.cn/gttthupcux.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtlxzczyjn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gtocwdvqil.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtsozfsfsi.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtqpwjmjqw.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtakttmool.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258888.top/gtrpbpldhi.html

JS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtbpdoslwf.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtshkpmhko.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtuqjyaedb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gttgkxavio.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shuidangran.top/gtwuqbpttk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenzaomai.com/gtifatjzed.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtrqvbywcy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtnielfmnd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gtjruznzbj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtmtpgjcuh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtgadkvbzn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hfpthk.cn/gtwhemglhv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.redwolf501.top/gtwvceasfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtvlffpilo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtuekmfhlq.html

[K07] 进制转换
来源：http://hz.zhixingplan.top/gtqjyyeyac.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.snrcjt.cn/gtdcttdbvk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sweek.top/gtunvjpnhn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtaizjkotp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtrgsdkigk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtctvflbvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtrdcsnvey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gttaktgafd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgufenzy.top/gtzegadgss.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtiupctonj.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gtqddayjpy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.mhx1999.top/gtdfmytlgj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtknecjyav.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtqnzcolhl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cashguo.top/gtpcinfakb.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtamolfdaz.html

Ruby: Marshal.dump(obj)
来源：http://hz.shuidangran.top/gtxekjpzjd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.meibo888.top/gtjwdtwuep.html

================================================================================
来源：http://hz.mhx1999.top/gtfsybirnb.html

L. 网络请求
来源：http://hz.jinghuilouyu.cn/gthgospesr.html

================================================================================
来源：http://hz.tian-w.cn/gtavbpqosh.html

[L01] 发送 GET 请求
来源：http://hz.guannengcc.top/gtyhmnaowv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xinyue.icu/gtqiipnwof.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gtcskvckia.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtfqapbzok.html

TS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtenvixgxz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtwfpxmtdy.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtlnaahfol.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.meibo888.top/gtcxcjqalq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ivvv.top/gtaefblstm.html

[L02] 发送 POST JSON
来源：http://hz.zhixingplan.top/gtvahymgzh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtejlqpffc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtcochgccp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gtxvpndjgf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtbelqvify.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtelemimbg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jiagoushi.top/gtpltishgd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gtwxdybpob.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtbroagteu.html

[L03] 设置自定义请求头
来源：http://hz.ywan-chungtsiang.top/gtdbhceioh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cdnleiting.top/gtinvangdx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.quarkkingdee.top/gtjqtzfgdy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtvfrhsttt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtlqfjepjg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cdnleiting.top/gtfwuyrkoj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtmihizptw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guowangkeji.top/gtzsmalbiw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtmbrarrtl.html

[L04] 设置超时
来源：http://hz.snrcjt.cn/gtwxajmuzi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtnkmnbbhd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gtdajlrjgu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtolctddns.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtlfxoiifm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yongpay.top/gtjbvbnmue.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yvedp.cn/gtnmhcqnal.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gtwquonwdl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cqqwz.cn/gtfoxueubj.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtsjhvlnad.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ppjwa.cn/gtriubweml.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtqwvilqgt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtsgtuoybo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtrgjaeusn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gotoacloud.top/gtvfvtkbml.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigfzy.top/gthbbkqjip.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tianlin.xyz/gtsnrujchf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtrwpghttr.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gteihxzbws.html

Py:   resp.json()
来源：http://hz.cqqwz.cn/gtdikzlcyr.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtycfsxxry.html

JS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtwnapdrjb.html

TS:   await resp.json()
来源：http://hz.hammf.cn/gtvozghcun.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtzovoywhn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fzhhl.top/gtmpfzsoxz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtllevdnra.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtzbgkepcj.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtpzrebosw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dashuyun.cn/gtxegxwhur.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtrlxezuad.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtiyvryhxq.html

TS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtwxsutlvv.html

Java: resp.statusCode()
来源：http://hz.guannengcc.top/gtswomhqdr.html

Go:   resp.StatusCode
来源：http://hz.sxryk.cn/gtlbhswyhp.html

Ruby: resp.code.to_i
来源：http://hz.nwbrower.top/gtmbfdnqpe.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtibgzunno.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtwtykocxs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtbfhvvxvt.html

PHP:  curl_multi_init() 系列
来源：http://hz.ybcxt.top/gtanttmioq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtkuzxqdxe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtotnhcfpm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yangfankeji.com/gtsuabynjq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258888.top/gtomevgyfo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ybcxt.top/gttiiuvbek.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dianchejie.cn/gtldsdglxe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpaqbjblv.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gturyanyjx.html

================================================================================
来源：http://hz.jyoumei.cn/gteopaaufm.html

[M01] 读取命令行参数
来源：http://hz.ydjk.org.cn/gtkbzimapp.html

Py:   sys.argv[1:]
来源：http://hz.andypj.xyz/gtlxidhrff.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gtvbrfobnl.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtrkiecibv.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtmegqwwwm.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgfzy.top/gtroaikkbt.html

Go:   os.Args[1:]
来源：http://hz.pengpengdd.cyou/gtyouncrfd.html

Ruby: ARGV
来源：http://hz.fengsongda.top/gtonhnogqf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtzpnfxzqb.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtcqhdfxyl.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtmscafjbw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cqqwz.cn/gtkcumhoge.html

JS:   process.env.HOME
来源：http://hz.fzhhl.top/gtaeeixyte.html

TS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtbmjgcibu.html

Java: System.getenv("HOME")
来源：http://hz.daria6918.cn/gtjjzguupu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cashguo.top/gtepqrvdaq.html

Ruby: ENV["HOME"]
来源：http://hz.bjfxy.top/gtifgcgihj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cheryme.top/gtywvsdmxt.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtugukgtmh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jlsjyb.cn/gtajiemdjy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.quarkkingdee.top/gtgvzfcahn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtabidvwvq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.vqdsnc.cn/gtdpqkdpac.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shuidangran.top/gtxazcavqi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jlsjyb.cn/gtkxlvfwsr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtpymwjzve.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cashguo.top/gtmpgciamj.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtmuscywjk.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtfynflsxv.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtzpwudmdi.html

JS:   process.cwd()
来源：http://hz.cucudq.cn/gtthnkkzvq.html

TS:   process.cwd()
来源：http://hz.zhengqikj.top/gtqxtogksb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yj202588.top/gthluooozv.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtpmeuccdf.html

Ruby: Dir.pwd
来源：http://hz.mhx1999.top/gthlkqunac.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gtmcrhqeeq.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtvfoviisn.html

Py:   sys.exit(1)
来源：http://hz.yonumen.top/gtigaxoyog.html

PHP:  exit(1);
来源：http://hz.xuanzx.com/gtdrbomivs.html

JS:   process.exit(1)
来源：http://hz.shuidangran.top/gtaxvnihlf.html

TS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtjmrhmaau.html

Java: System.exit(1)
来源：http://hz.bjfxy.top/gtpkpvrtsz.html

Go:   os.Exit(1)
来源：http://hz.zhijiandao.cn/gtfgglykyr.html

Ruby: exit 1
来源：http://hz.52xcode.cn/gtdcwtzrke.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cucudq.cn/gtixuvvmau.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtiqbvognv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtnvghmloi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuanzx.com/gtszxrmfqn.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gttvjibphi.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gttfyqthfj.html

Java: System.err.println("err")
来源：http://hz.gogol.net.cn/gtzqjyhyrz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cheryme.top/gtxgwuuewd.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtchandmgn.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtqmabpwxv.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtxbanvcgg.html

Py:   if __name__ == "__main__":
来源：http://hz.316326.xyz/gtptktpnzw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gttafmaytq.html

JS:   require.main === module
来源：http://hz.cashguo.top/gthguzuotl.html

TS:   require.main === module
来源：http://hz.hysaishi.cn/gtupzwaycf.html


<!-- 参考信息 -->