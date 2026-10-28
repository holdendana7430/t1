代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtkpfrzgdw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtticqevfv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtkuqjhznj.html

TS:   d.toISOString()
来源：http://hz.xingfuxueyuan.xyz/gtrtkwceqc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxinkj.top/gtpenshpxd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtreenarpa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtakpxshfi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtewlmnhyi.html

[J03] 字符串解析为日期
来源：http://hz.cheryme.top/gtgggajidd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtxwtehycw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhengqikj.top/gtezykcjfk.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtryxqmbhz.html

TS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtbkffkngo.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtorrbtvvi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtjvjbdwbl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtpjsfsuyr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtkfiqqyzi.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtixadvkjc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtrnttnlvr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.52xcode.cn/gtifcdoykx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gzhubu.top/gtdrwfylqg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jiagoushi.top/gtubmlewwi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhixingplan.top/gtxiqgxcpa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daxiang520.top/gtujbngyjm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.quarkkingdee.top/gtuoolqzya.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shzxlz.cn/gtnruebrlu.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtxxddtbsy.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtwuadjrzj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtuoklsaxs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtgzrurrfd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtqstmqmbh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtwfinotyw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gtetzmeqhh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtnkxqmqia.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aibaodan.cn/gtilvsgswf.html

[J06] 计算两时间之差
来源：http://hz.redwolf501.top/gtwpybxvob.html

Py:   (end - start).total_seconds()
来源：http://hz.guannengcc.top/gtggdcwopp.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtkrmatqcl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtmihhabpl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gtlsjqtnec.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtjbyjmocp.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydjk.org.cn/gtxmcwafgy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtonfrhkmv.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtvslxcosg.html

[J07] 比较两个日期
来源：http://hz.ivvv.top/gtppuxocsj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtmvlkjpkh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtfhuzmkds.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtkfvkdkej.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtfkjueadl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258888.top/gtrxieceza.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cashguo.top/gtdzsxwtpz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gttebjzloc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtsvvorotd.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gtulhtygcf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guannengcc.top/gtnibgvlbk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtlrenomks.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.birdmap.top/gtbbzqbffe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.bjfxy.top/gtcypzdhbr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtqfqljgwu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigfzy.top/gtndfvwiyz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtoxuvgbfp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtfstuqqii.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtcklefxqo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtzvqwnhpz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtpnfyhwef.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtknvoqxga.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtwvsbbqor.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.0kj1m.cn/gtgzvmnoel.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gtnpqvpska.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtbmpzqkef.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gtguooabnf.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gttibtyznd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sweek.top/gtwehyejtg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gtzcfnnrlm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yueranfly.top/gtmppgomtd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtrbtscfsu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtiefymbbv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhixingplan.top/gtvnzqwloz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtglrefeex.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtupygwtax.html

================================================================================
来源：http://hz.gaohongyu789.top/gtwhkfzzjj.html

K. JSON 与序列化
来源：http://hz.guannengcc.top/gttzsvwqze.html

================================================================================
来源：http://hz.sxryk.cn/gtdvumdzhf.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhongyouzk.top/gtxfavpxjy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtopmdvklu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtgjvtmqik.html

JS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtwxqgzvkk.html

TS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtuvvrxmgv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtzdrthzek.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtsrpqkdor.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtgnizybgd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtuihstcac.html

[K02] JSON 字符串转对象
来源：http://hz.xziqi.cn/gtkivunldi.html

Py:   json.loads(s)
来源：http://hz.hywenlv.cn/gtaymsgkho.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gtksggbkys.html

JS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gttbqmnuww.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtubzetvqc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtmxugeijl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtokuvhmcd.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtzrkjepvk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sysykeji.top/gtqbtwfjpq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tian-w.cn/gtiimhkvhm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtpmhjpwrn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtuehypoqb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtbrxezmiv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtghgablnk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gthftsdnud.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtpbudxail.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nwbrower.top/gtktksvatg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtrdtrishx.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gttjeajvgn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtjupxdfni.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangtech.top/gtgmumintx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gthkbtltuu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtrdohgrvj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtpswuhriw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtynasemjm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gttdabretf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtpvdylhqj.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gtamhmrfde.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtqedzowor.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtvfrzgypd.html

JS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtzasusxdh.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtfgetaolc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtpuraopsy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhiwuduotai.top/gtahqqysyr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtlsnjhmox.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtnfbyqllu.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gtanokfgxr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.meibo888.top/gtpmizcmam.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtmrvuybhp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtukkshwpu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtdujdswhb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtnvvamqle.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gtmuxaouyv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gthbldpyty.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gteydvnkbf.html

[K07] 进制转换
来源：http://hz.xinyue.icu/gtuyhtiozp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtbaeyghli.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.iojbl.cn/gtbpfpacjt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtskznkwkr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtgjgrobxc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gttyvxzaxq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuanzhike.top/gttmpridfa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gtkwnjokfi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gtmlginnvk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gthbckbytf.html

Py:   pickle.dumps(obj)
来源：http://hz.cheryme.top/gtvwwnxppz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtgxsppkrh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtnzumiqzg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtfxepkxpa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yangfankeji.com/gtmnydqsjv.html

Go:   encoding/gob
来源：http://hz.yangfankeji.com/gtrmtwkqjp.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtclsqitub.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtfhmvcnqn.html

================================================================================
来源：http://hz.gogol.net.cn/gtoqqkqjhq.html

L. 网络请求
来源：http://hz.zhiwuduotai.top/gtifrmxppb.html

================================================================================
来源：http://hz.nwbrower.top/gtpfufvtxp.html

[L01] 发送 GET 请求
来源：http://hz.zhoulong.xyz/gtrwpqfrbz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gzhubu.top/gtdybruvxi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtjeoktmam.html

JS:   await fetch(url)
来源：http://hz.xylfe.cn/gtqzsfosaa.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtcyrpgysh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhaomingkeji.xyz/gtxkkhrpdy.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtrhrghyni.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtjhbzwzns.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.redwolf501.top/gtcvzlopek.html

[L02] 发送 POST JSON
来源：http://hz.hammf.cn/gtwpquxrpl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtkikdvrgx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtpazkqsxw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gttwnwmvwn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtmkkudcmj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sufxvd.cn/gtkbdpmcft.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtbvfzqrjc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gtlumhqezu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtzoklrwfl.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtpvxntfyw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtzrgavuiu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ivvv.top/gtqzfpbmgt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gthownvadr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtwjbzlkwv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtzuhvkbsu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtihtrutiw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenzaomai.com/gttyorpjve.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtrfjmmmsz.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gtixxcggig.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gtfwfqyslp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cucudq.cn/gttqftcdrq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.redwolf501.top/gtpbvqfwcf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtsdtugiuq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gteboeggib.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtfnebontk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtjhnhetec.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fengsongda.top/gtzhordtwy.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gtlnnilnfh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gtqfdrqtde.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cqqwz.cn/gtdxdvynpz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gthdmhplfj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtyshuwwfx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtjechcmuz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gtfguztvfj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtqwhzytcz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtyoscvgic.html

[L06] 解析响应为 JSON
来源：http://hz.xziqi.cn/gtubavlkem.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gthpmyxywu.html

PHP:  json_decode($body, true);
来源：http://hz.ivvv.top/gtotfjnujl.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtnstdfvvo.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtnusihsed.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtewptrvuk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yueranfly.top/gtpurllori.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sysykeji.top/gtfwnodwqf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.c1oappe.top/gtyvkjemqz.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtrhwkbtgu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xziqi.cn/gtenlrynwb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtjocqkaoc.html

JS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtvbgylvau.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtmytvwmaj.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gtwwivriqh.html

Go:   resp.StatusCode
来源：http://hz.c1oappe.top/gtljvddjut.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gthigmyfqz.html

C#:   (int)resp.StatusCode
来源：http://hz.9152youxi.cn/gtyfdfjvqu.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gtjuqxoojl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shzxlz.cn/gtgveooppq.html

PHP:  curl_multi_init() 系列
来源：http://hz.fzhhl.top/gthpttlimn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtqhtkmuhm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtzedgvamh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cdnleiting.top/gtypzaowtu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pengpengdd.cyou/gtwkqcofkl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtaxasbuxu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtldqjxyal.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtndsiunuv.html

M. 命令行 / 进程 / 环境
来源：http://hz.bjfxy.top/gtbgodcitn.html

================================================================================
来源：http://hz.nanxinkj.top/gtowdryyby.html

[M01] 读取命令行参数
来源：http://hz.jianghu66.top/gtddwbepxz.html

Py:   sys.argv[1:]
来源：http://hz.ydjk.org.cn/gtaympdnst.html

PHP:  $argv;  $argc;
来源：http://hz.c1oappe.top/gtxqvduzsp.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtqfeoeriw.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gttqrwmzas.html

Java: args 数组（main 方法参数）
来源：http://hz.wangdashe.top/gtgurkowsu.html

Go:   os.Args[1:]
来源：http://hz.hnqzz.top/gtfhwgegsd.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gtjqdurofn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cashguo.top/gtoffyfski.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtgjmdofjt.html

Py:   os.environ.get("HOME")
来源：http://hz.zhongyouzk.top/gthnwvwlzm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tian-w.cn/gteeudizll.html

JS:   process.env.HOME
来源：http://hz.52xcode.cn/gthjifulev.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtactncuzr.html

Java: System.getenv("HOME")
来源：http://hz.snrcjt.cn/gtjzqqgmlv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhijiandao.cn/gtxrdgnkhi.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtukktxfti.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhoulong.xyz/gtyaaeklvm.html

[M03] 执行外部命令
来源：http://hz.zhaomingkeji.xyz/gtjibppiry.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtfbfijtqh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.birdmap.top/gtiwrzpcfw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtqwmhocmi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dashuyun.cn/gtgvywdajn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtdxpiawqj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zycfv.cn/gtlyklmmlh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtaavhywqi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.snrcjt.cn/gthidwqcki.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gtrmhhpuwp.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gtruxzjwnu.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtnuicraid.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtngapvrdd.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gttyemodyk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxuanxn.top/gttsvgdzvi.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gtqgrpvvci.html

Ruby: Dir.pwd
来源：http://hz.havefunace.top/gtcokduyhr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnxiangtu.top/gtjoudyfhz.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtwnhlbylq.html

Py:   sys.exit(1)
来源：http://hz.havefunace.top/gtcuxjobgx.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtbphriwqe.html

JS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtugjmwpjm.html

TS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtmdbltgay.html

Java: System.exit(1)
来源：http://hz.sufxvd.cn/gtzjqftueo.html

Go:   os.Exit(1)
来源：http://hz.aizwys.cn/gtfftarqzr.html

Ruby: exit 1
来源：http://hz.birdmap.top/gtphypckkt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gttcmlrrff.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gtckiaztsi.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tianlin.xyz/gtrkddpatc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gteklytxgt.html

JS:   console.error("err")
来源：http://hz.ppjwa.cn/gtjzwmitmo.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtbwklsofl.html

Java: System.err.println("err")
来源：http://hz.birdmap.top/gttdrtobvk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gterdjzrcy.html

Ruby: warn "err"
来源：http://hz.yuanzhike.top/gtupikukwv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtuwnnemgq.html

[M07] 判断是否为主入口
来源：http://hz.jinyuanbaomall.cn/gttyzylcab.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtpshsaczf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yanxiufei.cn/gtqvkhfhpl.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtrbyxmlzn.html

TS:   require.main === module
来源：http://hz.gaohongyu789.top/gtzsrwemdh.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtpsvuqkcs.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtxvtcjeze.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hongshengwenyu.top/gtblsvidnd.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtjqcwtgzz.html

[M08] 获取系统与运行时信息
来源：http://hz.gogol.net.cn/gtdkvrlusb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj20258888.top/gtduabkyko.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gtgacvdqxl.html

JS:   process.platform;  process.version
来源：http://hz.yueranfly.top/gtjofwwejm.html


<!-- 参考信息 -->