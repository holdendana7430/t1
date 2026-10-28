代发 wailian999

Go:   time.Now()
来源：http://hz.yongpay.top/gtsuhpbzha.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtgazjljxl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtfugnaioy.html

[J02] 格式化输出
来源：http://hz.sufxvd.cn/gtsngbgbtq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtloprbkwk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtftimgjvu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gthchqshgi.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gthuypnohd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtnllucdry.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtvliuxfrq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtgtzwoamq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ybcxt.top/gtqqacdhhj.html

[J03] 字符串解析为日期
来源：http://hz.bjfxy.top/gtwrjccoje.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yueranfly.top/gtetbewcgr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtidimwehp.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gttjurjbdd.html

TS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtvtogolvs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtjnjntpkz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtoozkiyjb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtbopndpik.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.svipenyu.cn/gtwsepbfxo.html

[J04] 时间戳与日期互转
来源：http://hz.nanxuanxn.top/gtwcfskuxw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jlsjyb.cn/gtqkurvbwd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtmokeauag.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fengsongda.top/gtzvqyjwwu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtjriwkeee.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxuanxn.top/gtixwkmxzy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pengpengdd.cyou/gthdysktpa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtsogheqiy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xinyue.icu/gtwoqtwnju.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtlgmyyocb.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gtbvojxxxq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtiljvxkgr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtsqgjobte.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtbfqnokld.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gtsdyfjrip.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.kuanghao11.cn/gtomkmqkxx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jlsjyb.cn/gthlvhxrva.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zycfv.cn/gtbcdcmpcl.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gtlvrkaghe.html

Py:   (end - start).total_seconds()
来源：http://hz.cucudq.cn/gtajkmaolx.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtmkkykmch.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jlsjyb.cn/gtomoclkeg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtyanjjwbk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shuidangran.top/gtumfvrxdx.html

Go:   end.Sub(start).Hours()
来源：http://hz.shangyingyoupin.top/gtxjryceby.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cheryme.top/gtmguilygy.html

C#:   (end - start).TotalSeconds
来源：http://hz.havefunace.top/gtxgtcrrcd.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtegreedvg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtulqizjvz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gtkpspjfzw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtqoxgosuv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtzliifmlz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtzvhqjlrm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangkeji.top/gttskofeci.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtozitmzxn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtagkuhqob.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtbudweinf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtynfkfhtv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtblsnodcw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gtniohahmw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.iojbl.cn/gtbnjllijz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gtvjelmblw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtpqjawyon.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtqfhpfbnc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtityytzwy.html

[J09] 时区处理
来源：http://hz.chenzaomai.com/gtzibdwjfb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ppjwa.cn/gtsfouxkum.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtdejktakc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtxebviaeu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gthercyzws.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sxryk.cn/gtbtudktfn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gtcuzhqpck.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gtwphkyucc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtwqwravla.html

[J10] 取今天 / 本月第一天
来源：http://hz.hysaishi.cn/gtqyzikfrf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtyalzgrud.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guowangkeji.top/gtangxnhch.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.9152youxi.cn/gtkgwyptvy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtfhkkwxwu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtarbrtzbu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtzajmzbxj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yueranfly.top/gtxacocdwf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtityjicze.html

================================================================================
来源：http://hz.hammf.cn/gtwkhfzqmg.html

K. JSON 与序列化
来源：http://hz.yj202588.top/gtbsmpmmmo.html

================================================================================
来源：http://hz.xylfe.cn/gtsxiehqjn.html

[K01] 对象转 JSON 字符串
来源：http://hz.aibaodan.cn/gtyispkyyu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtpghnlzwu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtaldqpwth.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtbwfdwkcy.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtipqzxzgf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtxqpzwwyt.html

Go:   json.Marshal(obj)
来源：http://hz.c1oappe.top/gtwfjbmcax.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtiwlpvwdb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtkungrwjc.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtghtwwgvy.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gthqubwvkq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hysaishi.cn/gtkbbseebn.html

JS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtnmulrrwo.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtyvequwbu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hfpthk.cn/gtnrokqkfg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtxrwlioir.html

Ruby: JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtbnlfqiwh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtnogjuelp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtocvzzthv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtkmfxdzgn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtvmdsifbx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtyhxpicgu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtudnssztu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtfjajkoro.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtjntrlgvo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhixingplan.top/gtxoeidpfo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sweek.top/gttkffykss.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtztwngjgw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pengpengdd.cyou/gtuwpptzaw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtczsshhud.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtkbpplrxw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtqfwykxdd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtlrfwefum.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtkcwjwxmv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.smart0.xyz/gthlzwwtsh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuxming.cn/gthegidezq.html

[K05] 深拷贝对象
来源：http://hz.yongpay.top/gtzpbgtkfo.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgfzy.top/gtcnjkydqc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtrnoxciwc.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtpfhbipwo.html

TS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtvfnwokkj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nwbrower.top/gthhqgxyah.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sxryk.cn/gtkxunwrfu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gthluntmez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yangfankeji.com/gtmuypmxhr.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gtbfweniez.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtysfjjcse.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sysykeji.top/gtsfgjramy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtmrfujiog.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtsanlzcff.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.meibo888.top/gtbdjwhntj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sufxvd.cn/gtdalrwxeo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtvddvmkho.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.havefunace.top/gtgvrafrwo.html

[K07] 进制转换
来源：http://hz.aizwys.cn/gtzxlehhfp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ybcxt.top/gtoixzktpy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hammf.cn/gtpgtfxfgg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangdashe.top/gtjcmyzgpw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtwnbpabgl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtzusqozvc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fzhhl.top/gtikakoyjb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258.top/gthzawuoij.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ppjwa.cn/gtatbnqlaq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sxryk.cn/gthdyhufqw.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtiavftfvx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxinkj.top/gtuhbikynr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtmqgcfgjw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtgdaodecq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuetiantiany.cn/gtorurwkid.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtlwzvsprl.html

Ruby: Marshal.dump(obj)
来源：http://hz.aizwys.cn/gtszfefgos.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shzxlz.cn/gtxivmdfzs.html

================================================================================
来源：http://hz.jlsjyb.cn/gtpolozdzn.html

L. 网络请求
来源：http://hz.nwbrower.top/gtugeaxvtt.html

================================================================================
来源：http://hz.mhx1999.top/gttfywyyrg.html

[L01] 发送 GET 请求
来源：http://hz.shzxlz.cn/gtypdbusym.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guowangkeji.top/gtthduodzw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtowznlsbj.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gttofrvwug.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gtcaixfolg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtllsxfcfg.html

Go:   resp, err := http.Get(url)
来源：http://hz.yangfankeji.com/gtyysvukym.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hammf.cn/gtkrvdjgat.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shzxlz.cn/gtktgyckch.html

[L02] 发送 POST JSON
来源：http://hz.nanxuanxn.top/gtumfhnjmu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gzhubu.top/gtmbkuazug.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinqigfzy.top/gtvsrlmzga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj202588.top/gtdoixzgtx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gteabbcbue.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.snrcjt.cn/gtpdwxsjzt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yvedp.cn/gtrqhcvznc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtwykofdjf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ivvv.top/gteqndtfdi.html

[L03] 设置自定义请求头
来源：http://hz.iojbl.cn/gtpmjolsyr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtnvhaorvg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gotoacloud.top/gtxozlhlsr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtkgdnmglg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtzhpzzeyt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtylgsndqd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtbylixfjp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cdnleiting.top/gttovweexc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtzxudyucz.html

[L04] 设置超时
来源：http://hz.sufxvd.cn/gtfvgbmegk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtbhxnhocx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtbblnbowr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtvneceffc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtlecvdoev.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtcfmuxdzi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.iojbl.cn/gtruazzqcg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtatalhupe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtqqsiipkp.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtouovvvmx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtixyeehpt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.feifeiyinyue.top/gtuusbdyvt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtcvbewjgk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtcbvrhyju.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ppjwa.cn/gtmigtweja.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtzoheupjl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtaltqqxmq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtsdpgoiav.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtrptscjgg.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtzfkjjcsd.html

PHP:  json_decode($body, true);
来源：http://hz.tian-w.cn/gtzhtlakiq.html

JS:   await resp.json()
来源：http://hz.ehwqpu.com/gtkeumdnih.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtcfhrpujy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.meibo888.top/gtdhetxnme.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yvedp.cn/gtnbhtxkbk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtoxaiumwi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shzxlz.cn/gtykzdnyxq.html

[L07] 处理 HTTP 状态码
来源：http://hz.meibo888.top/gtepdusmss.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gtetvenmou.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.redwolf501.top/gtadnkkrvv.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gteyndnfhl.html

TS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtvxpnrogn.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gtwxplghiw.html

Go:   resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtyfwrgkla.html

Ruby: resp.code.to_i
来源：http://hz.cucudq.cn/gtrkqjyplt.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtggtannef.html

[L08] 并发请求多个地址
来源：http://hz.chenjidiqi.icu/gtkcofdngo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenjidiqi.icu/gtkxkeiitb.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtzqxftaow.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtqxzilxpz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtaydsmmmh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gtareojcfq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxuanxn.top/gtswzpxkhf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtjbchehds.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.bjfxy.top/gtfqfreooe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgebclkun.html

M. 命令行 / 进程 / 环境
来源：http://hz.ywan-chungtsiang.top/gtyhycytnh.html

================================================================================
来源：http://hz.chenzaomai.com/gtwenoxvtx.html

[M01] 读取命令行参数
来源：http://hz.52xcode.cn/gtlplysazs.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gthltktaho.html

PHP:  $argv;  $argc;
来源：http://hz.zdqjudy.top/gtepeehelv.html

JS:   process.argv.slice(2)
来源：http://hz.yueranfly.top/gtkcpoetut.html

TS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtqrjvwhjt.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgfzy.top/gtcdaekfdw.html

Go:   os.Args[1:]
来源：http://hz.yvedp.cn/gtsbmwdvug.html

Ruby: ARGV
来源：http://hz.hywenlv.cn/gtslxjtoxk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yanxiufei.cn/gtgtbyhrzu.html

[M02] 读取环境变量
来源：http://hz.jqgfzy.top/gtonplytwf.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gthidumwlw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gtxepmwuxk.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtdjmkxvkq.html

TS:   process.env.HOME
来源：http://hz.xylfe.cn/gtncwxltdl.html

Java: System.getenv("HOME")
来源：http://hz.dianchejie.cn/gtrpqkqqkv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tanke756.top/gtijnmuslo.html

Ruby: ENV["HOME"]
来源：http://hz.hnqzz.top/gtovmepdjq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtjogsxqhs.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtdlkrmjkv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.meibo888.top/gtrjrdwxpo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xziqi.cn/gtdzjrgznb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtzkpebcsb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtgjfskeip.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shuidangran.top/gtsvvgyhfb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xziqi.cn/gttmbqwjnj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.daria6918.cn/gtpeikrkce.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pengpengdd.cyou/gtfwivkkrs.html

[M04] 获取当前工作目录
来源：http://hz.shangyingyoupin.top/gtmddbbnav.html

Py:   os.getcwd()
来源：http://hz.shangyingyoupin.top/gtwhdjwidi.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtgzxfetcj.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtcmxrqjty.html

TS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtaicpbbsv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtdruhidhx.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtavznsckj.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtczpdvngj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.mhx1999.top/gtrkhbwndy.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtdmmvfwij.html

Py:   sys.exit(1)
来源：http://hz.ivvv.top/gtazsbzmre.html

PHP:  exit(1);
来源：http://hz.zycfv.cn/gtdnpoeggk.html

JS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtmaunnrmp.html

TS:   process.exit(1)
来源：http://hz.hnqzz.top/gtiuusjxox.html

Java: System.exit(1)
来源：http://hz.hfpthk.cn/gtvlpysgbs.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtuuyjbpkq.html

Ruby: exit 1
来源：http://hz.feifeiyinyue.top/gtbzhfwmtc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnqzz.top/gtudpcvxle.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gttqvmqhxa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtovbvnedc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gaohongyu789.top/gtxvcgjevs.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtdoslrjdw.html

TS:   console.error("err")
来源：http://hz.guannengcc.top/gtxchcdmjx.html

Java: System.err.println("err")
来源：http://hz.hnqzz.top/gtipilntgv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj202588.top/gtgvwfurmj.html

Ruby: warn "err"
来源：http://hz.jyoumei.cn/gtlkzpbjpe.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnxiangtu.top/gtrmqyhvwp.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gtdombiiie.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gttcpodxzr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtrzsweprb.html

JS:   require.main === module
来源：http://hz.zycfv.cn/gtrxeltici.html

TS:   require.main === module
来源：http://hz.ivvv.top/gtnflilhyz.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gtdpniyeja.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtxhnepwnj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gtkhclttfy.html

C#:   static void Main(string[] args)
来源：http://hz.ydzc1.top/gtqawqzvss.html


<!-- 参考信息 -->