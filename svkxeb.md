代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daria6918.cn/gtiawkuuqa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pycfn.com/gtiebdujsf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtsgazakfj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhengqikj.top/gtgtxuzsxl.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtmuvkjugv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gtatyudefi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jlsjyb.cn/gtebpiznyk.html

JS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtjzinfgii.html

TS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtjruiqypl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtemwboijd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtwgtjaqhb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtzvbtmupm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cdnleiting.top/gtmewsisqh.html

[J04] 时间戳与日期互转
来源：http://hz.jinghuilouyu.cn/gtglocbjky.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtcyqpayjy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zdqjudy.top/gtklviunfv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuetiantiany.cn/gtnjywkekb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtddgcubwg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.iojbl.cn/gtlbhgilzv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenzaomai.com/gtmugctgtx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sxryk.cn/gtuururpcg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xylfe.cn/gtxmgrfrpq.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtimhunjsq.html

Py:   now + timedelta(days=7)
来源：http://hz.iojbl.cn/gtynxxnwoq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtzapewook.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtrlbrbopg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtqwtqdxnb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xingfuxueyuan.xyz/gttcbbfmev.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xylfe.cn/gtpbtngbtt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxinkj.top/gtjtlzukaa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtjcwoomfn.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gtjvjyblvl.html

Py:   (end - start).total_seconds()
来源：http://hz.vqdsnc.cn/gtzunxnyww.html

PHP:  $end->diff($start)->days;
来源：http://hz.mhx1999.top/gtssgywxzw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtxwspygqu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jlsjyb.cn/gttoxwulkj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gtlhuecohs.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258888.top/gtsdgybfzl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtbuypaldw.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtjrkcdodu.html

[J07] 比较两个日期
来源：http://hz.jlsjyb.cn/gtcqtnteqc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtzjixcpzd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ehwqpu.com/gtwmdfvaaz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtdzgovakh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtqfelclsm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gaohongyu789.top/gtvogecrgu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gtdepjfgfh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtenhmcdtc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gttkshnoan.html

[J08] 提取年月日与星期
来源：http://hz.ehwqpu.com/gtwbctcbvp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtwublzspm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtmpmtabzj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nanxuanxn.top/gtlfodftwz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gthncqhgps.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtehyemkpt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.snrcjt.cn/gthounhnaw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtbbzzdakg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtlsamzyqc.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtgggmpgdu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtqmagpzsy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtgtwjnlgi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtvbgtrbhj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtykujqsqm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhixingplan.top/gtanuhmlnh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtayuppptx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtpklynqbm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtteiejcgp.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgfzy.top/gtjjumdrcy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gthkcfapou.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtgcmmbliw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gttfztdsia.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gthattttlf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ppjwa.cn/gtbjtjagba.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yonumen.top/gtnqoxijna.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtrixrrnlp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtvqognozc.html

================================================================================
来源：http://hz.yuxming.cn/gtvaaxuswm.html

K. JSON 与序列化
来源：http://hz.jinqigufen.top/gtfszmawqi.html

================================================================================
来源：http://hz.fzhhl.top/gthufdeiwx.html

[K01] 对象转 JSON 字符串
来源：http://hz.tian-w.cn/gtkoyhitcv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtppsbelsg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtykdgcsxw.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gthnuvbjmr.html

TS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtqojepoly.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ehwqpu.com/gtahjyxpol.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtplevirni.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtmcaollwl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtvlofjbrb.html

[K02] JSON 字符串转对象
来源：http://hz.zycfv.cn/gtenaeddxl.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtqfxsiemh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtrftnzzsq.html

JS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtulwwwshg.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtkbvvyzdc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yanxiufei.cn/gtqvgnlgvi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtkymrsoqe.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtfzblbaxd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtedgtyedg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gaohongyu789.top/gtvknkusbk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gteficdniz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtnodpqljn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtcahvgeae.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtgeapqimc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuanzx.com/gtdexynmfj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.haohaochexian.top/gtswmlagpt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtoqdheytf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtpcxhogby.html

[K04] 读取 JSON 文件
来源：http://hz.quarkkingdee.top/gthpsfretb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.9152youxi.cn/gtzucmbeuw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuxming.cn/gtwmzwkayw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtvgzvrbjp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shangyingyoupin.top/gtswxkeuyu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gotoacloud.top/gtfxynhcdi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtuzrjrxhl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ivvv.top/gtuevcanxq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtqmtenldx.html

[K05] 深拷贝对象
来源：http://hz.0kj1m.cn/gtudmplkch.html

Py:   copy.deepcopy(obj)
来源：http://hz.zdqjudy.top/gtsahuantx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sufxvd.cn/gtzutuxauy.html

JS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtbywaghoj.html

TS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtnvccarsj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hysaishi.cn/gtpcbjipeh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtbsldgxpk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gtgkmyjcgv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuanzx.com/gtrqlpismw.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtdkhfxdpa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtnnfvviai.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtfmouifpk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtxgozfxno.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtpvvokzcx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtyoklsybz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ppjwa.cn/gtphppnvbw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gtgcwrcsgv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtqeahxgry.html

[K07] 进制转换
来源：http://hz.yonumen.top/gtpamdjvhh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sxryk.cn/gtjttzuoxc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aibaodan.cn/gttzukyzbh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtrwfvyouy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtrbnnscsj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtweikujtn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtivdbdwco.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tanke756.top/gtwbodjeth.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtgfznyqdj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gtmhwwycwk.html

Py:   pickle.dumps(obj)
来源：http://hz.wangdashe.top/gtknkpzrbf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.birdmap.top/gtfutukbzo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtxtsqavmh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtiqeorquy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtlygttmgz.html

Go:   encoding/gob
来源：http://hz.jyoumei.cn/gtbgyxwenf.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhoulong.xyz/gtcmnbfqyt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtidulzicg.html

================================================================================
来源：http://hz.nwbrower.top/gtkcdgmetx.html

L. 网络请求
来源：http://hz.nanxinkj.top/gtsqzjhycu.html

================================================================================
来源：http://hz.mhx1999.top/gtkifcruvc.html

[L01] 发送 GET 请求
来源：http://hz.daxiang520.top/gtwbnujacc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtqspzhejw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtjplnvraa.html

JS:   await fetch(url)
来源：http://hz.sxryk.cn/gtixztmink.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtptbbpaiv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jlsjyb.cn/gtmhztbsst.html

Go:   resp, err := http.Get(url)
来源：http://hz.feifeiyinyue.top/gtfphjqhug.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtssvwikdl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tian-w.cn/gtgjgzyofx.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtetotwsxq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtfvmafeku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtrwnbvtgs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtydzqmens.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtnzyhypky.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtilyjxpxh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtjywdadnj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gthygwxclg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sysykeji.top/gtfqtpwmpq.html

[L03] 设置自定义请求头
来源：http://hz.pengpengdd.cyou/gtwufrahff.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtyhqqanzi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnxiangtu.top/gtetyzdqdj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtkkdpwppw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtsglwyedw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenlongwang.top/gthszhoiws.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtelrmdjrh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.andypj.xyz/gtqwyqwbvw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtpugrmtqp.html

[L04] 设置超时
来源：http://hz.shanyushiyangtech.top/gtwfarqvuo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yueranfly.top/gtnqtjbuqz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gaohongyu789.top/gtcoyxupco.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtkepkmjuz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtwkhejxev.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.mhx1999.top/gtxojyjuha.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtrraswcsl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.9152youxi.cn/gtbbieirwl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yueranfly.top/gtstkwuhek.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gteprkbktt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.0kj1m.cn/gtwoljkwle.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daria6918.cn/gtdydqqxlh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtckrsnaiw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtjltmxifv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhijiandao.cn/gtrqeiskxt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhengqikj.top/gtwejvgztu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.kuanghao11.cn/gtuvkhzinr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gthqcdyins.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtryboqfot.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtfhdnybom.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtlguibpis.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtghbtljez.html

TS:   await resp.json()
来源：http://hz.cqqwz.cn/gtmngjwlez.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zycfv.cn/gtkbevanfm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.0kj1m.cn/gtgbianxyq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.haohaochexian.top/gtelhgrwkq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gtncuznkyw.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtyrxhatei.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aibaodan.cn/gtzyzwarbq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuxming.cn/gtzxkazpbk.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtndbjnvkp.html

TS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gteuziktxo.html

Java: resp.statusCode()
来源：http://hz.zhixingplan.top/gtvrswsgbm.html

Go:   resp.StatusCode
来源：http://hz.gaohongyu789.top/gtsvndqrnl.html

Ruby: resp.code.to_i
来源：http://hz.jinghuilouyu.cn/gtrykrkdcl.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtwhpnrykb.html

[L08] 并发请求多个地址
来源：http://hz.fzhhl.top/gtdiegzbdk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.kuanghao11.cn/gtnzgeiuln.html

PHP:  curl_multi_init() 系列
来源：http://hz.hfpthk.cn/gtzsctlbkk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtkkmbxcig.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtevnqqyyj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtyircfclj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gtultbukuu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sxryk.cn/gtyoinsaum.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.snrcjt.cn/gtdeptemhs.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthdbmvmnz.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtshfplovb.html

================================================================================
来源：http://hz.yj202588.top/gtzlyjoywf.html

[M01] 读取命令行参数
来源：http://hz.cashguo.top/gtvfmcxnus.html

Py:   sys.argv[1:]
来源：http://hz.sysykeji.top/gtvzjwmgfb.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtewzhkenq.html

JS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtpxnwdtnp.html

TS:   process.argv.slice(2)
来源：http://hz.316326.xyz/gtkzmdutht.html

Java: args 数组（main 方法参数）
来源：http://hz.feifeiyinyue.top/gtpwfghtxg.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtkhhlppiw.html

Ruby: ARGV
来源：http://hz.yj20258.top/gtokgjsbcp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtqooqylgw.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtewsewreg.html

Py:   os.environ.get("HOME")
来源：http://hz.xuanzx.com/gtbtjppkts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtizyuttyk.html

JS:   process.env.HOME
来源：http://hz.shuidangran.top/gtgcpslppi.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtuervbtuj.html

Java: System.getenv("HOME")
来源：http://hz.ywan-chungtsiang.top/gtimenkmpy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gtikknfnpa.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtviutleyx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fzhhl.top/gtgcrrdkob.html

[M03] 执行外部命令
来源：http://hz.xingfuxueyuan.xyz/gtklcpkuhv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.havefunace.top/gtxgjessbf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtddatzwpc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtpfgjdgvk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtulduwcca.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cqqwz.cn/gtsnpsgeym.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuanzx.com/gtanfbhncw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aizwys.cn/gtmxfewfum.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hfpthk.cn/gtnscsuztv.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtbhqlelxi.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtdqvkflkm.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtmxabfibh.html

JS:   process.cwd()
来源：http://hz.daria6918.cn/gtsomhftcf.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtlvdybkpr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fengsongda.top/gtcaxheiog.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtxatesvqv.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gthmyrswws.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.redwolf501.top/gtyjsdnpvv.html

[M05] 设置退出码
来源：http://hz.yueranfly.top/gtndtcjnny.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtwmrqvuex.html

PHP:  exit(1);
来源：http://hz.zhaomingkeji.xyz/gtkeokelxo.html

JS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtuubrdsfr.html

TS:   process.exit(1)
来源：http://hz.xylfe.cn/gtajddpiit.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtflqyrxlg.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtmevvjhpo.html

Ruby: exit 1
来源：http://hz.yanxiufei.cn/gtalvpuczr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtzdpszrzz.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gtzrjhvwny.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtygopdrit.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtkikxgpqp.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtkawsbldn.html

TS:   console.error("err")
来源：http://hz.redwolf501.top/gtoofiikyk.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtedimqgsi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gtmyuovexi.html

Ruby: warn "err"
来源：http://hz.vqdsnc.cn/gtyhznvmsy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtptpcpxsu.html

[M07] 判断是否为主入口
来源：http://hz.yj20258888.top/gtzinuuyzi.html

Py:   if __name__ == "__main__":
来源：http://hz.guannengcc.top/gtfewsdwjc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtgfbpohoq.html

JS:   require.main === module
来源：http://hz.ydjk.org.cn/gtyuwxwshs.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtpnsbbtus.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtoghjlmiw.html

Go:   func main()
来源：http://hz.cqqwz.cn/gtgkejbmnk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hnxiangtu.top/gtlhqyaioe.html

C#:   static void Main(string[] args)
来源：http://hz.xinyue.icu/gtbwqnlczr.html

[M08] 获取系统与运行时信息
来源：http://hz.ywan-chungtsiang.top/gtrzcudley.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhoulong.xyz/gthkasmbcx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shuidangran.top/gtapmhwbpw.html

JS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtlaazljlq.html

TS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtjzfhtqgm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtjkbgjxls.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cheryme.top/gteuxjwspg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fengsongda.top/gtnmxzvjxd.html


<!-- 参考信息 -->