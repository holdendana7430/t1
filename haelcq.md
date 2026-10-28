代发 wailian999

Go:   time.Now()
来源：http://hz.wangdashe.top/gtqsgrlvru.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtrscohesh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtwvqukbzj.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtjysrvzuf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtbfntmkgm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtdmvzckkd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.smart0.xyz/gtzumjydns.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtwgtwcrpl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtzvseeomd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtkgjlgyuw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtirwlhmok.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.svipenyu.cn/gtfqgakxoh.html

[J03] 字符串解析为日期
来源：http://hz.yvedp.cn/gtafcnjott.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.iojbl.cn/gtzntntqsb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gthhfaeupr.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtsfpyydku.html

TS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtqvreljta.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtlzhnmeqy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnqzz.top/gtaybliuar.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jianghu66.top/gtucrluuic.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtlojisovz.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtfxuylvty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtaryloxuy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtrwwgbmgw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtkqpibyob.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtjzhavzmb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aibaodan.cn/gttbdhutjj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.dashuyun.cn/gtteflxevm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xziqi.cn/gtqqeegcri.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gtakmjsedj.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtqwlfnnoz.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtjezhtwvk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenzaomai.com/gtymdvnjfb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gtzsyizzuy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtjutglzxd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtsmsizfcp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xingfuxueyuan.xyz/gtlmqqkxep.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtexwletbt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gthelahdyg.html

[J06] 计算两时间之差
来源：http://hz.yuxming.cn/gtsmeqwhsa.html

Py:   (end - start).total_seconds()
来源：http://hz.hnqzz.top/gtqgejoecm.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtkwwogqcj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtouquqihr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxinkj.top/gtgwnrckym.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtjwusunil.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gttrwlxhpd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zycfv.cn/gtndmumjdf.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenlongwang.top/gticphuimc.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gtmrzwauvw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtedfbjxbl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtidocoahe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtwkwqzgkf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtriqbiiuk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinghuilouyu.cn/gthxaajwyt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtpfmlpdmu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtoquurrzt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtkikpjlbk.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtsafhkrbt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tanke756.top/gtdjewlwvt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtlmitqiba.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yvedp.cn/gttbgynqlg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtnozudzvb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtdkncrhnz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj202588.top/gtfosqaqft.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dianchejie.cn/gtusthsnyi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtryrccpns.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtbfgnygpp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtrjtiqczp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtgtdeluiv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtqgaiypuw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtbaptcczs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jlsjyb.cn/gtuhvqomje.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ybcxt.top/gtfyxkpgmh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gtjhwanpyj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtfvsnuhep.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gtwpxopsps.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shzxlz.cn/gtobiyouex.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtfbcjtzte.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.birdmap.top/gtzfxvayti.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hysaishi.cn/gtcumgzyxm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ywan-chungtsiang.top/gthfigwhjv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtzzpffehy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtrodaghdp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cqqwz.cn/gtacxofvci.html

================================================================================
来源：http://hz.bjfxy.top/gtwlvdkdow.html

K. JSON 与序列化
来源：http://hz.dianchejie.cn/gtvoxmosnl.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdajkezpa.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtqpyyvmwk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangshuangyany.cn/gtdtghcqni.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtewottymu.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtdpcavzrf.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtmgeepbdv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydzc1.top/gtyorducsw.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtcqccpjzh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gtzavmwdxw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhongyouzk.top/gtwkdigbbt.html

[K02] JSON 字符串转对象
来源：http://hz.ivvv.top/gtwdaudnsx.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtxzeexnpl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ybcxt.top/gtmxmrvgfe.html

JS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtzvtbiwcy.html

TS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtcakpfuwn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtddptgzve.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gteqjwppdj.html

Ruby: JSON.parse(s)
来源：http://hz.nanxinkj.top/gtpvmofeib.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hongshengwenyu.top/gtkhkhvglj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhaomingkeji.xyz/gtsitilswd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtmvvhyryz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dianchejie.cn/gtanmpvpvi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtjdykoocd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtyiyuiruq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gtlmqurxjz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigfzy.top/gtpxelsdwf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtrphbitia.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shuidangran.top/gtacfazuis.html

[K04] 读取 JSON 文件
来源：http://hz.dianchejie.cn/gtarccwymi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.bjfxy.top/gtpxzmcadv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dianchejie.cn/gtycpflpay.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtdpuctkle.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtcuroaevg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtutkkyyvk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtihosfabb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guannengcc.top/gttyalqkec.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.smart0.xyz/gttmxmqqhe.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtwztrrgqd.html

Py:   copy.deepcopy(obj)
来源：http://hz.gogol.net.cn/gtldeeglye.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gtohdhkyco.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtbvvhxhjv.html

TS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtpdpiuiab.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtaonkidru.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.smart0.xyz/gtydhgkirl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xziqi.cn/gtfgkwpebu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj202588.top/gtaawwahwd.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtvoiftzri.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhiwuduotai.top/gtzehuqnez.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtvjzmwsjw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtgchwztls.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtpqlibobo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtcmhxbori.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.birdmap.top/gtezrdbsuf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pycfn.com/gtqefghcwe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtpnpbhqnu.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtiniruyqt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jlsjyb.cn/gtmggqkrti.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtbugnrjsc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtrueyxtqk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtxmecypav.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtafvcolkh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinghuilouyu.cn/gtchcjjxug.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tian-w.cn/gtncyegxbc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhiwuduotai.top/gtwelicyos.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhoulong.xyz/gtpyeqrqlk.html

Py:   pickle.dumps(obj)
来源：http://hz.xuetiantiany.cn/gtpdwqpsis.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtkmynozti.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtsexertik.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtlvhmvhum.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jlsjyb.cn/gtiqpsbqbv.html

Go:   encoding/gob
来源：http://hz.jinyuanbaomall.cn/gtiikstlrp.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangdashe.top/gtrrwonnfh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtepkldoyk.html

================================================================================
来源：http://hz.yongpay.top/gtljejybhw.html

L. 网络请求
来源：http://hz.cqqwz.cn/gtsrykxfzq.html

================================================================================
来源：http://hz.zdqjudy.top/gtmqcjjxwl.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtoszbaawz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtcziyoplm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtcylaycqy.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtxgrdhhnm.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtmizafdmr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtdebpmuco.html

Go:   resp, err := http.Get(url)
来源：http://hz.meibo888.top/gtffvswcdl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtfpmlsihu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gzhubu.top/gtpexppsib.html

[L02] 发送 POST JSON
来源：http://hz.mhx1999.top/gtmgpgzcjq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuetiantiany.cn/gtzljzvjdn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtsgqbqcbl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtqzwjfdgc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gttbhochrj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtsgbdpbwz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jyoumei.cn/gtnxroremv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtuhbbkxma.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.316326.xyz/gtgcghgaxw.html

[L03] 设置自定义请求头
来源：http://hz.dashuyun.cn/gtzzaidzcp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtosxmfmgb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtodedhjgg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gteggelyoc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtejnvjzjt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhongyouzk.top/gtvuhalqao.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sufxvd.cn/gtfrqrodyl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtpdhrtqlv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gttqgvzubp.html

[L04] 设置超时
来源：http://hz.shangyingyoupin.top/gtrgdaxvns.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ppjwa.cn/gtbsdrvekc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtemkvhlht.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtbgqhndtv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtgagxjxmo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jyoumei.cn/gtsgxpilvx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtqkwiytsu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ivvv.top/gtqglhupgl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtijlwdcxi.html

[L05] 上传文件（multipart）
来源：http://hz.cucudq.cn/gtmchhlvpp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daria6918.cn/gtrouawgsd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgfzy.top/gtigznzngu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtlkdorrcg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtuaczgzow.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258.top/gtnfmobeyw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tian-w.cn/gtzcijnkof.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtpeeulgyz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gogol.net.cn/gtmnslaobe.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtghybrnkd.html

Py:   resp.json()
来源：http://hz.jinqigufen.top/gtbkgcevee.html

PHP:  json_decode($body, true);
来源：http://hz.zhijiandao.cn/gtbyecspuj.html

JS:   await resp.json()
来源：http://hz.sxryk.cn/gtdipopncw.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtxvtpgfwj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydzc1.top/gtmyrkjbkb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gttpsibcbx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydzc1.top/gtaudqhvhz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yongpay.top/gttceqhawa.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtzdwxbdih.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtssuvkycu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ivvv.top/gtntjhgdqx.html

JS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtjuoognpn.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtotpifguo.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gthhtsnqea.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtqhhymxvj.html

Ruby: resp.code.to_i
来源：http://hz.dashuyun.cn/gtnoprecai.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gtmrdkbkys.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gttlhhvafr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.svipenyu.cn/gtcdjwljtt.html

PHP:  curl_multi_init() 系列
来源：http://hz.ppjwa.cn/gtjcvzsvbs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtgippgxgv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtjmmixdbu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtacqyijjf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cashguo.top/gtnesfbfmj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.meibo888.top/gtmdgqrjtk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtkagdbvom.html

================================================================================
来源：http://hz.xylfe.cn/gtzlgiriwo.html

M. 命令行 / 进程 / 环境
来源：http://hz.aibaodan.cn/gthnayupkf.html

================================================================================
来源：http://hz.quarkkingdee.top/gtviwipsja.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtfngqemux.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtvnmzffru.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtiyncpjip.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtpledjnsx.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gturrrhvqk.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtmjdvzidt.html

Go:   os.Args[1:]
来源：http://hz.vqdsnc.cn/gtluacdhai.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtksuaywlo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.9152youxi.cn/gtspgiglqa.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtmghxgxot.html

Py:   os.environ.get("HOME")
来源：http://hz.cucudq.cn/gtvqequtmf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jianghu66.top/gtyledydym.html

JS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtgqwtxoox.html

TS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtihcjorlg.html

Java: System.getenv("HOME")
来源：http://hz.zdqjudy.top/gttrnnmxuo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gtjuovpgxl.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtrpbggvtu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.0kj1m.cn/gtyduixacz.html

[M03] 执行外部命令
来源：http://hz.yvedp.cn/gtpmvonnnt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtyrcuoprt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigfzy.top/gthrpktqbs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtdqdjqqpg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtqmgthdjq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.snrcjt.cn/gtvpeidscg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gtsaoyagpo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtqaabjlam.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zycfv.cn/gtqausjhwn.html

[M04] 获取当前工作目录
来源：http://hz.daria6918.cn/gtniixktuj.html

Py:   os.getcwd()
来源：http://hz.yuanzhike.top/gtpylgjfdt.html

PHP:  getcwd();
来源：http://hz.pycfn.com/gtvtvznjom.html

JS:   process.cwd()
来源：http://hz.zhijiandao.cn/gthisxjqzi.html

TS:   process.cwd()
来源：http://hz.smart0.xyz/gtncmkslzn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuetiantiany.cn/gtifvhnykc.html

Go:   os.Getwd()
来源：http://hz.jyoumei.cn/gtxctdlsry.html

Ruby: Dir.pwd
来源：http://hz.zhongyouzk.top/gtdclxuhtf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangshuangyany.cn/gtnanxmzhq.html

[M05] 设置退出码
来源：http://hz.wangdashe.top/gtofummlqv.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gtijpnrnnr.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtlylmhxbf.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtwqageoih.html

TS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtjzhbfcks.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtifxjyoms.html

Go:   os.Exit(1)
来源：http://hz.zhiwuduotai.top/gtjbejmqcg.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtrhvtktns.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhongyouzk.top/gtiatxrfpc.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gtqfzgnadd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gtmvxcxmty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuetiantiany.cn/gtxnylwhdh.html

JS:   console.error("err")
来源：http://hz.0kj1m.cn/gtprrlgdid.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtbjjpsyep.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtryjbwnsr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pengpengdd.cyou/gtycptpdzy.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gtrvpwpxss.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nwbrower.top/gtnglfpwcx.html

[M07] 判断是否为主入口
来源：http://hz.chenlongwang.top/gtlfyqbcvu.html

Py:   if __name__ == "__main__":
来源：http://hz.wangshuangyany.cn/gtmpxolqhr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtyrhlmxxz.html

JS:   require.main === module
来源：http://hz.meibo888.top/gtgqtqozkn.html

TS:   require.main === module
来源：http://hz.yj20258.top/gtebszefco.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtopmiucwj.html

Go:   func main()
来源：http://hz.jinqigufen.top/gtibpsgxyq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yangfankeji.com/gtfharjelw.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtuxixqrfs.html


<!-- 参考信息 -->