代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtccwmrvlb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtnejphucj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zdqjudy.top/gtagdfcwiq.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtxsffcvij.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gteqwfgyks.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxuanxn.top/gtiaxjijhg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtjjcvnzqp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.quarkkingdee.top/gtxnhtvcfu.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtwhwxczrv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.andypj.xyz/gtbgisqwxw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtqpmfdalh.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtavvtbdip.html

TS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtqdvolxep.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtsepkxoyk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtftkedmkh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtmwnvlayp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yongpay.top/gtrhmturcm.html

[J04] 时间戳与日期互转
来源：http://hz.ydzc1.top/gtvhdddkyj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtfgtgzlyz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gtgjxrltlu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guowangkeji.top/gtpotmkdbw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtwqbjlvtx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtmvqoqjnt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.birdmap.top/gtgpbbjyms.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gotoacloud.top/gtrtvjxupc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtviwtlocc.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gttzhwfcdq.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gtvtfzpxjr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtkhtmxifq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtsuxtnppe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtykrrnbqt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gtzapevyqv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gtwdrzjrmu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtrokzqddk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtdqdaayde.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangkeji.top/gtvfbrjxjs.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gtrtpyhkhe.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtlahvaryx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtqaxhspad.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuanzhike.top/gtxsunikjg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.iojbl.cn/gteixifczn.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtdtbmebde.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtstujqbar.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgufenzy.top/gtyjswqfnh.html

[J07] 比较两个日期
来源：http://hz.316326.xyz/gttwfqxmyd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtmeifauez.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tianlin.xyz/gtetpwkopn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtwqxdwofm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtaxqbjjqx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtancqkskp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daria6918.cn/gtrznsrxed.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtbutsrnlx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtteyaitwx.html

[J08] 提取年月日与星期
来源：http://hz.zhijiandao.cn/gtjfnqvsiq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtvbrfumow.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shuidangran.top/gtdascizlg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cqqwz.cn/gtgxiipxds.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.feifeiyinyue.top/gtmudmbxlb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hammf.cn/gtkrpatjri.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtrxdauaaz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yueranfly.top/gtqxpyklfd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydjk.org.cn/gtpssynfwd.html

[J09] 时区处理
来源：http://hz.pengpengdd.cyou/gtyaybauab.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cqqwz.cn/gtorrdraht.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtxlzkmhcq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gteuofafai.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gthrebersl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtusuegysj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtgxmkgluj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtlbtizatd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sweek.top/gtuvgphwqm.html

[J10] 取今天 / 本月第一天
来源：http://hz.ivvv.top/gtcubjshjr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtyoivuobx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtuyqbnwoe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghu66.top/gtxquiazmj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jqgfzy.top/gtonqmcqsh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ppjwa.cn/gtfkwmcauq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtfuhkxygm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinghuilouyu.cn/gtnqhvejny.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xinyue.icu/gttwbfgsvr.html

================================================================================
来源：http://hz.gzhubu.top/gtnczsskgx.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtvijccmhr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdjtvejip.html

[K01] 对象转 JSON 字符串
来源：http://hz.iojbl.cn/gtcfozvops.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtvatijvzv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtbjtftqkd.html

JS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gtnguocoba.html

TS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtkiyxuhed.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtjfoglsbf.html

Go:   json.Marshal(obj)
来源：http://hz.jianghu66.top/gtyvmcdisu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gthuheiefw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtqeztnncw.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtauxmxanz.html

Py:   json.loads(s)
来源：http://hz.aibaodan.cn/gtjrwnesku.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangkeji.top/gtznybcqqm.html

JS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtqppbvzfl.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtjktxvamm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtnjbtjoeu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gtmeudqdks.html

Ruby: JSON.parse(s)
来源：http://hz.snrcjt.cn/gtluaptlgu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xinyue.icu/gtjqswrjjq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenzaomai.com/gtviliwwmi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtqzccdvni.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtnsgqpmpd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtlnnslpml.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtdswbabdp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gtexjxkmcn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtpfncmfjq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtbmcueiiz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gthhluinwj.html

[K04] 读取 JSON 文件
来源：http://hz.guowangkeji.top/gtyhmxsiyq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guannengcc.top/gtcdtaufyl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sweek.top/gtipzzriyx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtttwvhkrz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtdzruipnq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jianghu66.top/gtwhzwmvse.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtfjkarkif.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtyvnxjkbd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gthwwlvqoj.html

[K05] 深拷贝对象
来源：http://hz.hnxiangtu.top/gtigsbeegg.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhijiandao.cn/gtwcedxemc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hywenlv.cn/gtmtsdoqpk.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtyxocbblk.html

TS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtwlgmzvgv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxuanxn.top/gttuufdgge.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.mhx1999.top/gtjitorhmz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shuidangran.top/gtbdbmjews.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yanxiufei.cn/gtmzkhowxu.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gtjznyjfal.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gtqpbokfwt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.birdmap.top/gtwbpqbuul.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtedmzwsxs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtyeqvvaps.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gttbzwtjdc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.quarkkingdee.top/gttxyruoqr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.c1oappe.top/gtnnsaigqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gaohongyu789.top/gteczuqpux.html

[K07] 进制转换
来源：http://hz.svipenyu.cn/gthpluyvhc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtevllsqqb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtoghmgbzx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtgxbdnpvy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtkuxsdzwf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gttcetnhhw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gtdkvdfzlq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtdwgyjksm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tian-w.cn/gteyeweiib.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtxxczyvwd.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gtqyzufdsy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jyoumei.cn/gtujsjncna.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtgfrqrewv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtnkrbzayo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pengpengdd.cyou/gtrspypbgw.html

Go:   encoding/gob
来源：http://hz.shzxlz.cn/gtlgxnlahh.html

Ruby: Marshal.dump(obj)
来源：http://hz.gogol.net.cn/gtdednnhrs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtinwovpna.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzsvaktgc.html

L. 网络请求
来源：http://hz.shuidangran.top/gtaupoouok.html

================================================================================
来源：http://hz.haohaochexian.top/gteqkdoucx.html

[L01] 发送 GET 请求
来源：http://hz.bjfxy.top/gtnxjhfjqr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tianlin.xyz/gttzmbaiml.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gthcgltnge.html

JS:   await fetch(url)
来源：http://hz.hammf.cn/gtmzaxdlbk.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtwdjfwvmg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dianchejie.cn/gtkvfnfyly.html

Go:   resp, err := http.Get(url)
来源：http://hz.shzxlz.cn/gteniqvsjh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinyuanbaomall.cn/gtfwuymgsn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtjcndmean.html

[L02] 发送 POST JSON
来源：http://hz.yuxming.cn/gtbwhprvgw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtjtyspfjw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtfqwaljia.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtcmfajoth.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtypnjbpgm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zycfv.cn/gtzcvbhqvj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hysaishi.cn/gtspiiqgdb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangdashe.top/gtkltopmsf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jianghu66.top/gtbzpvmrfd.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtriavetny.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daria6918.cn/gtchksgmtp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuetiantiany.cn/gtsljiokch.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtjapddfls.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtohdcbstm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guannengcc.top/gtifnuqaib.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtzrsistab.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gogol.net.cn/gtphvsdecu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtvxuustau.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gttlwpjqmc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gzhubu.top/gtsftgfwck.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtuglnscrx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtqavmanhl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ybcxt.top/gtxuezolsu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gtacatcyyy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tanke756.top/gtuhnjdcpm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhengqikj.top/gtnjgspxew.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtzudmukuj.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtkxhgblnz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtkfbqkbwe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tanke756.top/gteolpnycx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gzhubu.top/gtorfbeuct.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtbzlwbhcx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gteqjlqopc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhongyouzk.top/gtryuboepz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dianchejie.cn/gtoyftqzoq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.redwolf501.top/gtqgudhznj.html

[L06] 解析响应为 JSON
来源：http://hz.yonumen.top/gtkxywunlv.html

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtumtnjxcx.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtyxtnfhox.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtqwggqcaz.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtlozhngom.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.quarkkingdee.top/gttipiupds.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tian-w.cn/gtsutdvmpo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtuhazeshe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtlznxkcgy.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtkyvozoxw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtwhrmlkot.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtezwjylle.html

JS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtxmfhwiqu.html

TS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtldddlvxx.html

Java: resp.statusCode()
来源：http://hz.chenjidiqi.icu/gtarkvcyzc.html

Go:   resp.StatusCode
来源：http://hz.yuanzhike.top/gtxwfcmspy.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtrvlunmbc.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtwmkjhohb.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtqapijvuu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.andypj.xyz/gtmsilddqj.html

PHP:  curl_multi_init() 系列
来源：http://hz.316326.xyz/gtvfwfodzf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtzxfyotwv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtixfpfyuj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tanke756.top/gtmzlxcehh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtlwjsvflp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sweek.top/gteiqbmqrg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daxiang520.top/gtpaoqwgsu.html

================================================================================
来源：http://hz.zdqjudy.top/gtgpbdxrnc.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtgnlewobv.html

================================================================================
来源：http://hz.jianghu66.top/gtukhtnksm.html

[M01] 读取命令行参数
来源：http://hz.shuidangran.top/gtfohqwdfx.html

Py:   sys.argv[1:]
来源：http://hz.ydzc1.top/gtvtbdfriu.html

PHP:  $argv;  $argc;
来源：http://hz.316326.xyz/gtnqsvoglx.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtkocdnwfs.html

TS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtyyhcipax.html

Java: args 数组（main 方法参数）
来源：http://hz.mhx1999.top/gtsopxaszr.html

Go:   os.Args[1:]
来源：http://hz.gogol.net.cn/gtwhdxrxgq.html

Ruby: ARGV
来源：http://hz.mhx1999.top/gtfyxoohqq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cdnleiting.top/gtftcenvcz.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtsftbghkx.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtycbxiuzw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cdnleiting.top/gtgwoncrmu.html

JS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtyutjltff.html

TS:   process.env.HOME
来源：http://hz.andypj.xyz/gthhqvbequ.html

Java: System.getenv("HOME")
来源：http://hz.smart0.xyz/gtufusviow.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtgyfnoauz.html

Ruby: ENV["HOME"]
来源：http://hz.sysykeji.top/gtgkzfhtdo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hysaishi.cn/gtvlsrxamz.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gtqmdcylbl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtzmlzvyvn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.kuanghao11.cn/gtrqcgnghl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gtowwoudva.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtjxximguj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.feifeiyinyue.top/gtckbjmshy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yanxiufei.cn/gtxvppswgk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sysykeji.top/gtljkiwuvi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sweek.top/gtanvtxent.html

[M04] 获取当前工作目录
来源：http://hz.pycfn.com/gtdkkrzimp.html

Py:   os.getcwd()
来源：http://hz.chenzaomai.com/gtxjwklaec.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtzoqshvyc.html

JS:   process.cwd()
来源：http://hz.bjfxy.top/gtrvergvok.html

TS:   process.cwd()
来源：http://hz.smart0.xyz/gtafcxnzah.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.quarkkingdee.top/gtocgyfxzj.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gtinfdnibf.html

Ruby: Dir.pwd
来源：http://hz.xuetiantiany.cn/gtjyulqujb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.haohaochexian.top/gtzoziyuey.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gtubhklfvc.html

Py:   sys.exit(1)
来源：http://hz.cqqwz.cn/gtnlvhxyas.html

PHP:  exit(1);
来源：http://hz.aibaodan.cn/gtmpizpeiz.html

JS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtdbzzimzd.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gteeuqrggl.html

Java: System.exit(1)
来源：http://hz.xinyue.icu/gtsnsuhvwg.html

Go:   os.Exit(1)
来源：http://hz.yuanzhike.top/gtekiushys.html

Ruby: exit 1
来源：http://hz.xuetiantiany.cn/gtsapznajh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.feifeiyinyue.top/gtvggquyyq.html

[M06] 向标准错误输出
来源：http://hz.yj20258888.top/gtrtamaegp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtpdwmmlqs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ybcxt.top/gtessaqtpq.html

JS:   console.error("err")
来源：http://hz.shzxlz.cn/gtyugunhku.html

TS:   console.error("err")
来源：http://hz.tanke756.top/gtaclfptaz.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtgoeyhgvl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenlongwang.top/gtawypvefq.html

Ruby: warn "err"
来源：http://hz.smart0.xyz/gthttxbuaf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnxiangtu.top/gtxllntozs.html

[M07] 判断是否为主入口
来源：http://hz.haohaochexian.top/gtfuawkpdv.html

Py:   if __name__ == "__main__":
来源：http://hz.hysaishi.cn/gtumwecgjs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtpsejiasb.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtmzyspauz.html

TS:   require.main === module
来源：http://hz.dianchejie.cn/gtyhljresw.html

Java: public static void main(String[] args)
来源：http://hz.zhongyouzk.top/gttqbfvtrm.html

Go:   func main()
来源：http://hz.pycfn.com/gtnxnuqtqk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtlinlmsxo.html

C#:   static void Main(string[] args)
来源：http://hz.xylfe.cn/gtuyelfepz.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtbtrjgzli.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangtech.top/gtukplmxnz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cqqwz.cn/gtryymatqu.html

JS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gtovpnvaun.html


<!-- 参考信息 -->