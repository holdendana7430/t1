代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtcwejykqj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtwcxdlhgr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shuidangran.top/gtpwgzytyc.html

TS:   d.toISOString()
来源：http://hz.xingfuxueyuan.xyz/gtyluptnpk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gtnowbrvmn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtzxgkgoum.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtvtpsexjq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.52xcode.cn/gtwxofxlqv.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtovxpnudu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ydzc1.top/gtcbovkzzd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gtwqwbknxp.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtmsufgapp.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtpkfjtaao.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtdchfqfnp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gtnndnnsmf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtmrhwbjrc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuanzx.com/gtfztgvqfy.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtfjfzvwcs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.52xcode.cn/gtrpbfhjlh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtcltaymvy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtvuldsfhh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.haohaochexian.top/gtnmlcsfgw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.svipenyu.cn/gtjfezbhsg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.svipenyu.cn/gtuwgvwnrw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.redwolf501.top/gtxcscimsw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangkeji.top/gtqkqmmsii.html

[J05] 时间加减（加 7 天）
来源：http://hz.yonumen.top/gtgrynpitx.html

Py:   now + timedelta(days=7)
来源：http://hz.dianchejie.cn/gtxlfiqgjk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxuanxn.top/gtcbxvqlpj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtdpjplxds.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtsdwptzox.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ywan-chungtsiang.top/gtcfuorgew.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgfzy.top/gtxahmxyub.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gtjoasqiaz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dianchejie.cn/gtnlohnrqz.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtoshtvisx.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtdcrhrmpu.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gtjqjdheld.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtllicykwm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.redwolf501.top/gtxjcxomfc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgfzy.top/gtqgrupfix.html

Go:   end.Sub(start).Hours()
来源：http://hz.kuanghao11.cn/gttuqzszpy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hammf.cn/gtqhuoypae.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtaycpsvlr.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtjwxvgclf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtcdtivrkn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jianghu66.top/gtdeeuyneo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gttrkaslxo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtbujjmnql.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gtqquygloq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtztsusspi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtuzudhdud.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtkvjxgsys.html

[J08] 提取年月日与星期
来源：http://hz.tian-w.cn/gtlnmmxwic.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xziqi.cn/gtdokcvvef.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxuanxn.top/gtdzybvxff.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtfdjevcxx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zycfv.cn/gtguksctac.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gtjbdraawa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtkshbsuue.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtdxpdbfuf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtlxeqgstz.html

[J09] 时区处理
来源：http://hz.birdmap.top/gtiwksclhc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtmvvxmpbs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtxikccatn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtdktqxfwz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtpuzgffuf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtfjwjandw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ppjwa.cn/gtgqddacgs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtisplxbci.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtvpzhxhnj.html

[J10] 取今天 / 本月第一天
来源：http://hz.sysykeji.top/gtvxsocntp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jyoumei.cn/gtqsjqvwdt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtouandyjf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.haohaochexian.top/gtsufbcfhx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ywan-chungtsiang.top/gtdtjiuxtw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gtniaoravt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhixingplan.top/gtwhzyecai.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtcqwsmmpa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sxryk.cn/gtcyvpxzia.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlmosclhl.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gtkczupvra.html

================================================================================
来源：http://hz.ppjwa.cn/gtvwgndtep.html

[K01] 对象转 JSON 字符串
来源：http://hz.pycfn.com/gtfzerssud.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtdefjfpvq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtytocwecb.html

JS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtgqqhguwl.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtwxzcyixr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.svipenyu.cn/gttmyqsngv.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtwzxbghuk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtotpvyoex.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtdpnaqohr.html

[K02] JSON 字符串转对象
来源：http://hz.zhaomingkeji.xyz/gtovlujvcm.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangtech.top/gtkhmrevye.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinghuilouyu.cn/gtfdrakqxv.html

JS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtgdgihkjg.html

TS:   JSON.parse(s)
来源：http://hz.dashuyun.cn/gtezihycgl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sweek.top/gtzzdfurkr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtvihvmwfn.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtdocwhjjw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gtfhluhgsh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gterpuquwy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtqixjtbmw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtryeaiuok.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtpytuvzrh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtisgpyynd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yonumen.top/gtdxkrmejj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtqepfdxlm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.c1oappe.top/gtrqbxchgc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtfpelinbe.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gtvqxtpwlo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtsqjyamwf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtfldkkxct.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtywmypieq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtsxxrgoxu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yongpay.top/gtpxmzohtd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtipklyaum.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xinyue.icu/gtqdhiekbq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hfpthk.cn/gtbevfjgod.html

[K05] 深拷贝对象
来源：http://hz.yanxiufei.cn/gtyyfenhkk.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigufen.top/gtbmcwwetw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.iojbl.cn/gtyaiswjio.html

JS:   structuredClone(obj)
来源：http://hz.zhengqikj.top/gtjfbgvdmd.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtvvlbzqrq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.9152youxi.cn/gtcymvnpib.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yongpay.top/gtzrxzgjfa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jiagoushi.top/gtvbgbgkzw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guannengcc.top/gtuguucvsi.html

[K06] 解析 URL 查询串
来源：http://hz.gotoacloud.top/gtndjeynby.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sweek.top/gtpkyysoqk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hongshengwenyu.top/gtogljojtj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtwkqvmnof.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtkgnqppzh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guannengcc.top/gtntxoqnaa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtmqmzgdzs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtlsqnncjf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtrjrfvefl.html

[K07] 进制转换
来源：http://hz.0kj1m.cn/gtlukjaxhg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.nanxinkj.top/gtemvkpnui.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.0kj1m.cn/gtdflrkfni.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtglschmwq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtkjatghgl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtjncirfwz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuanzx.com/gteoezvvgb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtcntguvch.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtrcvuuugt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dashuyun.cn/gtwrllntcj.html

Py:   pickle.dumps(obj)
来源：http://hz.birdmap.top/gtrgzgssmo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtvjiiibnt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtgvgfxkdd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtbikxscwr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gttqkvchwo.html

Go:   encoding/gob
来源：http://hz.316326.xyz/gtlfwjhvge.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenjidiqi.icu/gtmzrogbbp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtnzsjpnfr.html

================================================================================
来源：http://hz.tanke756.top/gtshiflvtn.html

L. 网络请求
来源：http://hz.zhoulong.xyz/gtrlankubp.html

================================================================================
来源：http://hz.yvedp.cn/gtyfnpedjm.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtvxjlythn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtokgilhjb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtqmatvmjm.html

JS:   await fetch(url)
来源：http://hz.guannengcc.top/gtkdejwugl.html

TS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtprerewzz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dianchejie.cn/gtpvduhomr.html

Go:   resp, err := http.Get(url)
来源：http://hz.hongshengwenyu.top/gtbcnooezd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jiagoushi.top/gtaplbcbtt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtpeyudyfd.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtbuoebdca.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhixingplan.top/gtdwbvopkr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.haohaochexian.top/gtvswqtdpa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtywkqqhpg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtbjzecsze.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangshuangyany.cn/gtfvwlebvc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.svipenyu.cn/gtsluefptb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnqzz.top/gtasmrnksr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.0kj1m.cn/gtsdmrflnv.html

[L03] 设置自定义请求头
来源：http://hz.0kj1m.cn/gtrjrkengy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtruabovqn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yanxiufei.cn/gtmjnyqinz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtgktabuwa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shangyingyoupin.top/gttjmsztdc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtlucoyyko.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtjajodfem.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtxpnkjquv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtwxlfohug.html

[L04] 设置超时
来源：http://hz.daria6918.cn/gtuwszpzzx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuxming.cn/gtmtrrwrur.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuxming.cn/gtjddquaup.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtyspmbdlj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtjliguhak.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ppjwa.cn/gtzduyqbsd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hysaishi.cn/gtxnygeqkv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sxryk.cn/gtcnhvalfu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gogol.net.cn/gtxoszlczz.html

[L05] 上传文件（multipart）
来源：http://hz.jinqigfzy.top/gtmkmsgfcz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenjidiqi.icu/gtkvxyrpxg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtieaeiaak.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtswigbtgc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtsomcsevp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yonumen.top/gtffqckdzp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtuurwbpjv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuxming.cn/gtsqrlzxnv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtjmxyhsfb.html

[L06] 解析响应为 JSON
来源：http://hz.haohaochexian.top/gthmttbgyk.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gthpgzwfiy.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtstvxsiwf.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtuhilfngm.html

TS:   await resp.json()
来源：http://hz.52xcode.cn/gtwoelejlp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenzaomai.com/gtjvpjqlhu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtshhtaqxe.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtjseeodsf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sweek.top/gtmjtiallm.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhixingplan.top/gtchpvvqqz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhoulong.xyz/gtsxjfwkld.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtorkhvqlh.html

JS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gthmrsfqgo.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtxxqohylw.html

Java: resp.statusCode()
来源：http://hz.dianchejie.cn/gtiignicff.html

Go:   resp.StatusCode
来源：http://hz.mhx1999.top/gtcyykybjh.html

Ruby: resp.code.to_i
来源：http://hz.zhoulong.xyz/gtesudrfiw.html

C#:   (int)resp.StatusCode
来源：http://hz.smart0.xyz/gtmbwrzpdx.html

[L08] 并发请求多个地址
来源：http://hz.ydzc1.top/gtylnujfka.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hywenlv.cn/gtzfqsnzuw.html

PHP:  curl_multi_init() 系列
来源：http://hz.c1oappe.top/gtvzxxpktg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtygifuodq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtwtqipior.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gthhvnlkzv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yj20258888.top/gtjbkyaxnd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gtovtimwsh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.svipenyu.cn/gtgyhxeiae.html

================================================================================
来源：http://hz.hammf.cn/gtudvmyeim.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gtmojapwxx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkkrexugw.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtiatifhpu.html

Py:   sys.argv[1:]
来源：http://hz.jiagoushi.top/gtuasefjfq.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtrhjblbao.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtyigzclbe.html

TS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gthpkbmhlp.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gthcpazvoy.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gtbpcbihmk.html

Ruby: ARGV
来源：http://hz.guowangkeji.top/gtashlypiu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.haohaochexian.top/gtyrboeiwh.html

[M02] 读取环境变量
来源：http://hz.9152youxi.cn/gtajjadptf.html

Py:   os.environ.get("HOME")
来源：http://hz.haohaochexian.top/gtwwcpptir.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.quarkkingdee.top/gtzyezhamj.html

JS:   process.env.HOME
来源：http://hz.sxryk.cn/gtblwhpbxh.html

TS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtufqsuvbs.html

Java: System.getenv("HOME")
来源：http://hz.0kj1m.cn/gtbrbzyeps.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jianghu66.top/gtjfaycwuc.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtsovjztoj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gttkxcchum.html

[M03] 执行外部命令
来源：http://hz.sweek.top/gtiyxgcsww.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtpatpehxv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jlsjyb.cn/gtpvjkmiis.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtajzzbsun.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtqlmcflsa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gzhubu.top/gtrvertral.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtdnfpmsjn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.andypj.xyz/gtzlhwtlgc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fengsongda.top/gthothdaop.html

[M04] 获取当前工作目录
来源：http://hz.yongpay.top/gttsebehin.html

Py:   os.getcwd()
来源：http://hz.zdqjudy.top/gtxcqpcunx.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtzrkbhngc.html

JS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtmpqupfkp.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtdytklsij.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daxiang520.top/gtmsxhrbzh.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gtzxvaulwh.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gtvomfpouz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtnbrapqrg.html

[M05] 设置退出码
来源：http://hz.mhx1999.top/gtejoufpjh.html

Py:   sys.exit(1)
来源：http://hz.hnxiangtu.top/gtgjyygkzn.html

PHP:  exit(1);
来源：http://hz.nwbrower.top/gtmptppysn.html

JS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtvzcdqxzu.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtwypeeypc.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtphshkudf.html

Go:   os.Exit(1)
来源：http://hz.zhongyouzk.top/gtyomprsdq.html

Ruby: exit 1
来源：http://hz.smart0.xyz/gtjejyzedy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtwtlmxbyx.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gtpxhzqlqy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dianchejie.cn/gtuqibsoez.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jlsjyb.cn/gtxgaefvwe.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtpgxsmpyq.html

TS:   console.error("err")
来源：http://hz.cheryme.top/gtublkieds.html

Java: System.err.println("err")
来源：http://hz.nanxinkj.top/gtegcoasux.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtuqgpwfha.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtoxtmvjaa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtapbhrwes.html

[M07] 判断是否为主入口
来源：http://hz.xziqi.cn/gtsuwnahdp.html

Py:   if __name__ == "__main__":
来源：http://hz.sweek.top/gtmekcmuvc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhiwuduotai.top/gtxvdxgrlo.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtvflnmfwm.html

TS:   require.main === module
来源：http://hz.jinqigfzy.top/gtbqwgogda.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtwqtlxcjf.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gttfeqmhfg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtiynenrby.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258.top/gtgjbyzbda.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtpuigkfra.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtuwznxcpk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtqftdzbbp.html

JS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtoifxowpi.html


<!-- 参考信息 -->