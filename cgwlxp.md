代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtzgygqopd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtikicyrhz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtlkmhursj.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtcqbddidt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtnqojzdtc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yongpay.top/gtjqaofctg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtrocbsqxi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shzxlz.cn/gtbnberzbw.html

[J03] 字符串解析为日期
来源：http://hz.chenjidiqi.icu/gtltkhvwcd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhiwuduotai.top/gtjbaowqdz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtoyqjteaf.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gthcyliykv.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtqtdmzdzm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtjgonqnxu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgufenzy.top/gtwhvragmo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtfjtjdhao.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gtoetndvgr.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gtuvktkmqu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.bjfxy.top/gtdeghuozw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtztdideja.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nwbrower.top/gtdxvbvcao.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtmtgmjsci.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhongyouzk.top/gtizzkdjre.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhijiandao.cn/gtdjkprtwc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtjjnpidle.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.redwolf501.top/gtmsbfxbil.html

[J05] 时间加减（加 7 天）
来源：http://hz.gzhubu.top/gtgmxcxtlo.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtrdagselm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydjk.org.cn/gtcjjezlft.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gttxkgdvlv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gttplrfmug.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ybcxt.top/gtgabsfnpf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtfxskghxg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenlongwang.top/gthehmvjmc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtrqrrtflo.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtjkdbttop.html

Py:   (end - start).total_seconds()
来源：http://hz.dianchejie.cn/gtjfafesri.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtokzfjoyq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gtcipzzgqj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtszjagmui.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangkeji.top/gtoefpxymx.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtspqcpcsc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtkljvswfy.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gtikbghkhu.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gtrxgnnswt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtkzngoofu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yonumen.top/gtyiuxcmvl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtvxndrkgy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtzkokabvp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yueranfly.top/gtbrfdqzlq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cqqwz.cn/gtlbzburra.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtgopvulot.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtkktkaiaf.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gtjfyxvlfw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtzvpuowqc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gtpucgfrbn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtagpmkuoy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hysaishi.cn/gtzgzzbwpn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtmcjegiuo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtovcmmiwp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ydzc1.top/gtkcjvilfl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.mhx1999.top/gtwfwmxxjq.html

[J09] 时区处理
来源：http://hz.kuanghao11.cn/gtiejgsrbm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gtpqykdwcn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtuezjysyl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtppftstrn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtspqohuuw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtsllsigfu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtfipfxoqd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gtsahualad.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hfpthk.cn/gtxufylsiv.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtkuzwgzle.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shanyushiyangtech.top/gtmmbqyjkw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtozemjjxk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xziqi.cn/gtvdqoxbmt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gthlsuxbcf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtuvplidku.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtseifjmqf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtvdtevzsj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jiagoushi.top/gtyzwsxkla.html

================================================================================
来源：http://hz.ydjk.org.cn/gthdhayplf.html

K. JSON 与序列化
来源：http://hz.cashguo.top/gtbctbosgo.html

================================================================================
来源：http://hz.0kj1m.cn/gtfsyeyyqe.html

[K01] 对象转 JSON 字符串
来源：http://hz.hywenlv.cn/gtlrvowefk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtpqvnvrgl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtqtvdjgxq.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtvttxcvcn.html

TS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtpydxrukz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtbxzzitzy.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtnhrwvwic.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtraskrqum.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtpsbbgmwh.html

[K02] JSON 字符串转对象
来源：http://hz.hongshengwenyu.top/gtnhbcvivp.html

Py:   json.loads(s)
来源：http://hz.meibo888.top/gtvgvbxpkr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtgaiomdyb.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtgkwomtxk.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtcbumxblv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cucudq.cn/gtxtdhuzqq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtocyqiqiz.html

Ruby: JSON.parse(s)
来源：http://hz.0kj1m.cn/gtwojwoqcn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.bjfxy.top/gtcwvzbotz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtwzjxxoww.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hammf.cn/gtswwzmrpz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtucdxtbnn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtfypubyig.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtsksirefe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pycfn.com/gthyyaxgmf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtyxuhyrth.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.quarkkingdee.top/gtncvbpxlu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gtnotrobqx.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangtech.top/gtrxobyafh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtcxxrpkab.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtirdexovc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtbcmfrsbg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtxrqkzepa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258.top/gtnfpffrki.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtsaswliku.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtpwxgwino.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtsrrqbpah.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtjbzfgjdc.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtgcytgyqn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.daria6918.cn/gtpachsovx.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gtmaeesnni.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtdathubaz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ywan-chungtsiang.top/gtwrdhzpkl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangkeji.top/gtvxwqwoxl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtyiatjrkh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtoxinzjka.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtadllfpva.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258888.top/gtjfjvqclw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtydyeiytf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtentnoeaz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtjhwflgnt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtkbeuksxd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenzaomai.com/gtmgbatudb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtwerytsdi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daria6918.cn/gtxznromby.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtmafqjrro.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gtuzftfovd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.vqdsnc.cn/gtylvaxqwi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtboilluvw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtzkuqfbsf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sweek.top/gtkhccpniy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtugoysyst.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gtedswetdp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hongshengwenyu.top/gtgchmpwrh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sweek.top/gtanafmkjd.html

Py:   pickle.dumps(obj)
来源：http://hz.xuanzx.com/gtovwfpamv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtwkcjkvxp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtgohxvbur.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtzcvglkwu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtldrjjeqm.html

Go:   encoding/gob
来源：http://hz.guannengcc.top/gtcxyjoohl.html

Ruby: Marshal.dump(obj)
来源：http://hz.xingfuxueyuan.xyz/gtdbpmvvak.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daxiang520.top/gtoxmhvcqw.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpegqrmnv.html

L. 网络请求
来源：http://hz.yanxiufei.cn/gtdtbmrdgk.html

================================================================================
来源：http://hz.9152youxi.cn/gtgzrbheeq.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtfokzoqoz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gtnyvlzhmh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xinyue.icu/gtmmfkxpcc.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtwgtibuni.html

TS:   await fetch(url)
来源：http://hz.smart0.xyz/gtbloqzrha.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtjgpsopgs.html

Go:   resp, err := http.Get(url)
来源：http://hz.sxryk.cn/gtfrmyouma.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sxryk.cn/gtiywpjvzw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gtdhwuyldv.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtaaocwvxd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xinyue.icu/gtxdoqttpv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangkeji.top/gtriwzabsu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtdkryfpxc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtqxuvciiw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yongpay.top/gtmzjqbtcs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gttugplnin.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yangfankeji.com/gtesdifblu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guannengcc.top/gtsroiopnr.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gthkhgjpby.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinyuanbaomall.cn/gtzsljdcjo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtbftumssk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtdwaipsjk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtmmbzgmwp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shangyingyoupin.top/gtlvpthmna.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.iojbl.cn/gttaxhipzm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gtsrzjfmtz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtwaqlkkgm.html

[L04] 设置超时
来源：http://hz.chenlongwang.top/gtqwqhztcw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.52xcode.cn/gtvxqgjabf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yonumen.top/gtyitrgsnv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtklflycrd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtvuigetqd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gtgrumcwka.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhoulong.xyz/gtimuqumtr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shangyingyoupin.top/gtmrrwrtib.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yonumen.top/gtwnigqlmh.html

[L05] 上传文件（multipart）
来源：http://hz.pengpengdd.cyou/gtcvnvqbdo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.meibo888.top/gtzcgytfsq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gotoacloud.top/gtsftvsoid.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtvngwjovi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtbnsgoino.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuxming.cn/gtuyzaixui.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuanzx.com/gtiboosrky.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtxeauwgdy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinyuanbaomall.cn/gtaanwgcyh.html

[L06] 解析响应为 JSON
来源：http://hz.smart0.xyz/gteavvxrvs.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtmwmccxmh.html

PHP:  json_decode($body, true);
来源：http://hz.yueranfly.top/gtrkbuqpmi.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtwhtoovdc.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gtrqrwckjv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtkhxsdhuv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gtggleggsp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.316326.xyz/gtndbasnsg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fzhhl.top/gtduldzuvg.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gtxwuxvsfe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtiewjwvvo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtvheaqfhp.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtxobwjkjy.html

TS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtrrmeoutc.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtzukpwtxj.html

Go:   resp.StatusCode
来源：http://hz.snrcjt.cn/gtwqasksdr.html

Ruby: resp.code.to_i
来源：http://hz.yonumen.top/gtuhpbcxrj.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtyceffwkw.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtvuxnjimv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj202588.top/gtlnwbmgkb.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtffhogdit.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtudchuttp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtdsfdwcwe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtckhnmjpm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtooaipwkb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtknfrvhml.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gtdzafphnz.html

================================================================================
来源：http://hz.bjfxy.top/gtoposrdvv.html

M. 命令行 / 进程 / 环境
来源：http://hz.meibo888.top/gtbelgywfn.html

================================================================================
来源：http://hz.wangdashe.top/gtnooafoqy.html

[M01] 读取命令行参数
来源：http://hz.chenlongwang.top/gtgvbwkjmq.html

Py:   sys.argv[1:]
来源：http://hz.smart0.xyz/gtmsetthxu.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtkqhrwplu.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtoblvippn.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtfyvycafj.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtxmdpzmwz.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtlbixkzvd.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtmijqekrc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj202588.top/gtizkwfwed.html

[M02] 读取环境变量
来源：http://hz.xuetiantiany.cn/gtmucplesv.html

Py:   os.environ.get("HOME")
来源：http://hz.sufxvd.cn/gtkwwytosf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtivtevilm.html

JS:   process.env.HOME
来源：http://hz.yj202588.top/gtofvbulgw.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gtjqigstyc.html

Java: System.getenv("HOME")
来源：http://hz.jqgufenzy.top/gtfjacgaax.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtuqoczsnp.html

Ruby: ENV["HOME"]
来源：http://hz.sweek.top/gtqnfwsnii.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ywan-chungtsiang.top/gtzudeccur.html

[M03] 执行外部命令
来源：http://hz.ydzc1.top/gttxvbpoha.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guannengcc.top/gtzphqmshh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.bjfxy.top/gtujwrycjs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtkxmhyecy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtqcktzivb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ivvv.top/gtgvbsorto.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gtutpbajgi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cheryme.top/gtkrraccfq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jiagoushi.top/gthlzpxkym.html

[M04] 获取当前工作目录
来源：http://hz.wangdashe.top/gtivmstsbg.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtfjjcydie.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gtumybpwkl.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtfitktvuq.html

TS:   process.cwd()
来源：http://hz.daria6918.cn/gtnnljniii.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yongpay.top/gtryonkjlc.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gtmfjwtkbf.html

Ruby: Dir.pwd
来源：http://hz.andypj.xyz/gtonumcplz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtvxnbscqm.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtcysfmjjo.html

Py:   sys.exit(1)
来源：http://hz.9152youxi.cn/gtpzaqhsmy.html

PHP:  exit(1);
来源：http://hz.ppjwa.cn/gtadljxpud.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtfntmmjje.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtvtzbugvb.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtygdffxoh.html

Go:   os.Exit(1)
来源：http://hz.fzhhl.top/gtlvjzmgaj.html

Ruby: exit 1
来源：http://hz.jianghu66.top/gtnslyrjxq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gotoacloud.top/gtspvhqsia.html

[M06] 向标准错误输出
来源：http://hz.yueranfly.top/gtzpcealzo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtxqlbtbey.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gtorzoalar.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtivfhnejc.html

TS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtgutezynw.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtpxtpkudv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daxiang520.top/gtpfehpzxc.html

Ruby: warn "err"
来源：http://hz.sxryk.cn/gtdneapfbw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtuhdqiexp.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtcpqvfmky.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtvfxaznpr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gtrgaswpeo.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtuyoywfpg.html

TS:   require.main === module
来源：http://hz.nanxuanxn.top/gtikjdhodk.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtxdrvlnyc.html

Go:   func main()
来源：http://hz.chenlongwang.top/gtdxsaqbsu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gthlqhobsq.html

C#:   static void Main(string[] args)
来源：http://hz.gotoacloud.top/gtwntawkww.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gtunlebokg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hammf.cn/gtmfymwbaj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daria6918.cn/gtbifspdts.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtssygfbhd.html


<!-- 参考信息 -->