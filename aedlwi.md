代发 wailian999

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtjelihiwd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthokhnktq.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtpeipkybf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhijiandao.cn/gtwxkdjzyr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtytnlclje.html

JS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtaogccmid.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtofffqpun.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhoulong.xyz/gtkjrierxy.html

Go:   time.Now()
来源：http://hz.yangfankeji.com/gteodijlgf.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtjnfkcemg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtknnwzwxy.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtobuccwod.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtgcnwukni.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtxdklbgfn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.snrcjt.cn/gtpdkrkngn.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtlkustkxh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtecavfyhm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtncxnpsfi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtjgktlyot.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtodlahxul.html

[J03] 字符串解析为日期
来源：http://hz.cheryme.top/gtdlzubtsg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtqrludqfu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtnjbvmyls.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtvdeptdcc.html

TS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gttobzhcwj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtlcgrzzfd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gthhqafapm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtkoufcjla.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtkyypldjv.html

[J04] 时间戳与日期互转
来源：http://hz.zhijiandao.cn/gtacfpynhn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtxikcyida.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tanke756.top/gtyniviede.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dianchejie.cn/gtbuiybskk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cucudq.cn/gtwvfgzzcq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tian-w.cn/gtspaqwqye.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gotoacloud.top/gtwxmqhzbv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtgxoclgmz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinghuilouyu.cn/gtzmvcscuf.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtemlnromt.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtmcycwyrh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtrvcuimgs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtrpxafzex.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtejdooqqd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daria6918.cn/gtkxkjdsql.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xylfe.cn/gtktgzmhal.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtlflbrydz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zycfv.cn/gtydbhpzwj.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtrmhuvfvl.html

Py:   (end - start).total_seconds()
来源：http://hz.shangyingyoupin.top/gttbjfamji.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnqzz.top/gtmseoytba.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sufxvd.cn/gtsjqugpck.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ybcxt.top/gtaadaivqw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.birdmap.top/gtwikdpdhj.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtydpcfbgz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtpfgdresy.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gthecavhda.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gtljmquovy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtlgravgkb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtsdqoejyv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtamgojspr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtkjrfgqye.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhixingplan.top/gthqkktmso.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pengpengdd.cyou/gtlwkfqxtd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtjozmxahj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtzebijejf.html

[J08] 提取年月日与星期
来源：http://hz.316326.xyz/gtgqvmzimw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258888.top/gtavdofnhg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtdccwwolk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.havefunace.top/gtmczauvbf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuanzx.com/gtncukchpj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.smart0.xyz/gtjbrtheka.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinyuanbaomall.cn/gtluzhvdzh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtcgfaarqa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtmuelxvfc.html

[J09] 时区处理
来源：http://hz.cucudq.cn/gtdavvdium.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtxhoeacgl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinghuilouyu.cn/gtdrmczhha.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtotubunrg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtxzpdlztq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sysykeji.top/gtjkaqvoww.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenzaomai.com/gttjhybzsc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yangfankeji.com/gtjgvxlwln.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenlongwang.top/gtspccepjs.html

[J10] 取今天 / 本月第一天
来源：http://hz.guowangkeji.top/gtxrblxftl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtltxuifpk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gttbswzsnn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuetiantiany.cn/gtpiukszjy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gteskpjdln.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gthtocwrvu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinghuilouyu.cn/gtckxzmjsa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangkeji.top/gtcekcydrb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuxming.cn/gtbmucokuh.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtuauptrpm.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gtadhlcrsx.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtpapwnlkq.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtnibnpujg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtwnoikzdw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtwnuvjfet.html

JS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtiosbgxdz.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gttdwabsog.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.mhx1999.top/gtjfsdufmi.html

Go:   json.Marshal(obj)
来源：http://hz.mhx1999.top/gtnkgymbrm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj202588.top/gtzseovzfl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gtzqbtuxjn.html

[K02] JSON 字符串转对象
来源：http://hz.yangfankeji.com/gtfrnickqh.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtplothnbq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtcwfniwes.html

JS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtjkmdawkn.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtusxolmup.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtqwvyqrko.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtbvbuonse.html

Ruby: JSON.parse(s)
来源：http://hz.dashuyun.cn/gtifknfbbr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgfzy.top/gteuasnnml.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtfccmjinq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtdujxskkj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtunvqovex.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtrajazkmt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtrmophpao.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenzaomai.com/gtrakwjiuc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtqaadvenh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pycfn.com/gtakulckad.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtqztoadhh.html

[K04] 读取 JSON 文件
来源：http://hz.pycfn.com/gtsneatuzh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtnpneswry.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtmbjfosoj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guowangkeji.top/gtuzrzsvdk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtofqhqzbu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtatdksmnw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtpdzckmde.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtkbcskvqw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.c1oappe.top/gtseuvxsyn.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtulxesfqu.html

Py:   copy.deepcopy(obj)
来源：http://hz.cqqwz.cn/gtjufgnokq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangdashe.top/gtbyggicsg.html

JS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtvirbzwjj.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtlmkjoxos.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.smart0.xyz/gtbudnutpq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sysykeji.top/gtdtguadfm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtdtfssmcv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yueranfly.top/gtftszyxuj.html

[K06] 解析 URL 查询串
来源：http://hz.cheryme.top/gtffymhaut.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtracklgpg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.316326.xyz/gtcdhfdmvt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtzrghuovt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtbdpyuhsm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtwawshhnu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sufxvd.cn/gtrhtbosnr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtynjurjvk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtofgbobnr.html

[K07] 进制转换
来源：http://hz.chenzaomai.com/gthmbllarj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guowangkeji.top/gtbaxwgidx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xylfe.cn/gtlntbsiio.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtofjmmrvk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtsprrkhwg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gttjyyykfs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jianghu66.top/gtrfjfyuhj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtpazucspz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ivvv.top/gtezjappev.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aibaodan.cn/gtfwbfbqgx.html

Py:   pickle.dumps(obj)
来源：http://hz.shuidangran.top/gtmyagvruk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtqcfkprpv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gttavwhiez.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtilrnpgba.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gttearxnsj.html

Go:   encoding/gob
来源：http://hz.shzxlz.cn/gtnhhojusp.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gtifwnhddr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtstjhnaqc.html

================================================================================
来源：http://hz.guowangkeji.top/gttjpwdpzv.html

L. 网络请求
来源：http://hz.daria6918.cn/gteoepguot.html

================================================================================
来源：http://hz.redwolf501.top/gtjbeigmyt.html

[L01] 发送 GET 请求
来源：http://hz.xinyue.icu/gtoqpmaeuy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gtmqnwvbqe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydjk.org.cn/gtpsvifzdz.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gteacjoglx.html

TS:   await fetch(url)
来源：http://hz.sweek.top/gtllxjlwja.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtqhfpdslx.html

Go:   resp, err := http.Get(url)
来源：http://hz.shanyushiyangtech.top/gtljifldnn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtaugvybwu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtzniwenbn.html

[L02] 发送 POST JSON
来源：http://hz.ydzc1.top/gtqjrvvdte.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenjidiqi.icu/gtdnjjopwh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinghuilouyu.cn/gtwljsxrnp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtlmxestso.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtbqhhuusr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtardmthec.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yanxiufei.cn/gtcmypjatu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtbofvxhma.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.0kj1m.cn/gtuafdsgqi.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtiuknptcu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jiagoushi.top/gtmritblob.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.iojbl.cn/gtbnnzweli.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhiwuduotai.top/gtnwjmfbjm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtpvctxcry.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gtytjxuxbv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gttpwuxqnu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fengsongda.top/gtednmguwj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtdcqgmdor.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtscvwksbr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gtnsxxrocu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gzhubu.top/gtaomiymad.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtmvgdexms.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtivonjlqt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtyakquttx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hnqzz.top/gtsixqiyun.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.snrcjt.cn/gtdhsexcss.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtrlhbnuyp.html

[L05] 上传文件（multipart）
来源：http://hz.c1oappe.top/gtijrhqrlk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxuanxn.top/gtehxapltp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gttjqasiki.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gttndvyhdj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtymjynkqq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtmurmtgkz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jyoumei.cn/gtgsuytxsm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtjnrlsuyw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sweek.top/gtfydzgrrc.html

[L06] 解析响应为 JSON
来源：http://hz.nanxuanxn.top/gttnhndqkh.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gtbvalxnln.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtsfdmlble.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtadxsfgff.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtlgumzsxz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yonumen.top/gtqhvjwgjx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtttzeblkw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtvpwmgfoi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtsqvrouri.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtwrvjschv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ybcxt.top/gthzkpoqgw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhiwuduotai.top/gtfwjchgng.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtsenqgqys.html

TS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gtfvawllln.html

Java: resp.statusCode()
来源：http://hz.xziqi.cn/gtgnivlrlk.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtgwimfpzw.html

Ruby: resp.code.to_i
来源：http://hz.yj202588.top/gtjkykfsnt.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtpgbofjss.html

[L08] 并发请求多个地址
来源：http://hz.xuanzx.com/gtfcpafkpz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtcnidqvtv.html

PHP:  curl_multi_init() 系列
来源：http://hz.quarkkingdee.top/gtvcfzgrzj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gthmyzdymy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnqzz.top/gtwjuivvos.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xinyue.icu/gtlqrnzuah.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhongyouzk.top/gtvfjzywju.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.316326.xyz/gtszufslra.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtyssiyalt.html

================================================================================
来源：http://hz.cqqwz.cn/gtpyjrlxys.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtfeprxphc.html

================================================================================
来源：http://hz.pycfn.com/gtjixdgkiz.html

[M01] 读取命令行参数
来源：http://hz.pycfn.com/gtfiyqmxjb.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtzwlkdglp.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtdrdosjjn.html

JS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtlyoocpwp.html

TS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtvhcvkgzl.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtltrlpzrx.html

Go:   os.Args[1:]
来源：http://hz.guannengcc.top/gtpsghentk.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtypocefby.html

C#:   args 数组（Main 方法参数）
来源：http://hz.c1oappe.top/gtcagqkftr.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtabbfhjtr.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtscgvnabg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gtzypbvbjq.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gtitetswqh.html

TS:   process.env.HOME
来源：http://hz.yuxming.cn/gthmrptrba.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangtech.top/gtyekkwexl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cdnleiting.top/gtosjawiik.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gthqbzcpea.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dianchejie.cn/gtcbmzzrso.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtfpwrinpw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhengqikj.top/gtzwlmdzlq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtrcbarsvr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtcwcsectm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hnxiangtu.top/gtlrmooxei.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cashguo.top/gthjyhrrdh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gogol.net.cn/gtcefenwtf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtwawrzeqt.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtfaxztalg.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtkmwrgdfe.html

Py:   os.getcwd()
来源：http://hz.hywenlv.cn/gtshbuebyl.html

PHP:  getcwd();
来源：http://hz.birdmap.top/gtihjkqagy.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtfocswhxr.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtkndootlc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtwpiaypfb.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtwtafsdfp.html

Ruby: Dir.pwd
来源：http://hz.zhixingplan.top/gtizernaic.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtccpgbvcs.html

[M05] 设置退出码
来源：http://hz.guowangkeji.top/gtgmzszwms.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gtpzqjhgys.html

PHP:  exit(1);
来源：http://hz.ywan-chungtsiang.top/gtiutlhuwv.html

JS:   process.exit(1)
来源：http://hz.yuxming.cn/gtgyqstrga.html

TS:   process.exit(1)
来源：http://hz.birdmap.top/gthaggrqoy.html

Java: System.exit(1)
来源：http://hz.hammf.cn/gtkbvdltef.html

Go:   os.Exit(1)
来源：http://hz.jiagoushi.top/gtamzutipm.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtkrqxutlu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuanzx.com/gtohyqqkac.html

[M06] 向标准错误输出
来源：http://hz.wangshuangyany.cn/gtpwgvyzai.html

Py:   print("err", file=sys.stderr)
来源：http://hz.0kj1m.cn/gtgpjcezzf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xylfe.cn/gthmedjkpz.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtwteouhfg.html

TS:   console.error("err")
来源：http://hz.pycfn.com/gtwgtblhsm.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtlksxrstl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtknfoqiea.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtxflpagoe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtjhmhybqw.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gtdbmnlnmr.html


<!-- 参考信息 -->