代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtmqjeuzou.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxuanxn.top/gtajlskotr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtsjceqosw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hysaishi.cn/gtyxuzqpvv.html

[J03] 字符串解析为日期
来源：http://hz.c1oappe.top/gtjxwdmdio.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.birdmap.top/gtmpilcwpv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtzwsebzia.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtjzvtfead.html

TS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtfehojdel.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jyoumei.cn/gtfwrbodmn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtnrhkscdi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtnxpzzgpn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtmdzizxvn.html

[J04] 时间戳与日期互转
来源：http://hz.fengsongda.top/gtrydczszy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtdwqvztre.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtjjztqkeq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gttngqvspy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuetiantiany.cn/gttexmskxu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtczwdzhvv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.snrcjt.cn/gtpwnnhlyk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gtndhvanrx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenjidiqi.icu/gtwfjiycex.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtwebkicih.html

Py:   now + timedelta(days=7)
来源：http://hz.vqdsnc.cn/gtovkhichg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gteqmnzbtb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtkjzcocth.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtjquogymo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aizwys.cn/gtszukimsg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtaqkzglqj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cheryme.top/gthxuyvomh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangkeji.top/gtwsruynxk.html

[J06] 计算两时间之差
来源：http://hz.birdmap.top/gtntrbnwzu.html

Py:   (end - start).total_seconds()
来源：http://hz.pengpengdd.cyou/gtmgsbarmb.html

PHP:  $end->diff($start)->days;
来源：http://hz.shzxlz.cn/gtfnegetlu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gthiyqnzgj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtzqbkuoga.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hongshengwenyu.top/gtrbeiuxya.html

Go:   end.Sub(start).Hours()
来源：http://hz.daria6918.cn/gtxhnguset.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtovtzhdpq.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhongyouzk.top/gtgspaymsj.html

[J07] 比较两个日期
来源：http://hz.pycfn.com/gtvgxidedb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtveppidml.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cqqwz.cn/gtnasuscwq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gtvnrzjnyf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtijrsmzpq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtjyxqfbqy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtdivjboqo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtpepeqokg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtoqxznrlj.html

[J08] 提取年月日与星期
来源：http://hz.dianchejie.cn/gtphzgmtii.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shangyingyoupin.top/gtdesmnjas.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtdyhjjtua.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtiwegzfsf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtvmrjybvz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sweek.top/gtuupuenzz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj202588.top/gtpvjuorcw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigfzy.top/gtxxbdmtur.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtyvucbpou.html

[J09] 时区处理
来源：http://hz.ydzc1.top/gtchlsjgbm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shangyingyoupin.top/gthasjngtl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gtogkeztzi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtlupsscms.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtpouqwqkb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxuanxn.top/gttcahzzaj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtpwrggvah.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtjmunmuyb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daria6918.cn/gtuaswkvay.html

[J10] 取今天 / 本月第一天
来源：http://hz.52xcode.cn/gtqvnbioov.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gtiarrqdiy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtjlsftttm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtbwphaqlo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guannengcc.top/gtvwbnpnxn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258888.top/gtdpckewbx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuetiantiany.cn/gtaejymynp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cashguo.top/gtrnimfewv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gtoeifsfej.html

================================================================================
来源：http://hz.sufxvd.cn/gtypygbsay.html

K. JSON 与序列化
来源：http://hz.yangfankeji.com/gtckmbblxd.html

================================================================================
来源：http://hz.daria6918.cn/gtuckgokrr.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtyjzwiyhq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtpntnvpte.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtkohokncm.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gthnhgtzeb.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtrzjbtdqt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtsavsynvp.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigufen.top/gttihxbpec.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hfpthk.cn/gtealnfwrj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jyoumei.cn/gttyjssent.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtehfehaud.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtbygdoohh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guowangkeji.top/gteklnylwv.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtfitakxzs.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtmleeqful.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgufenzy.top/gtkucyfwll.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtmdlozgjk.html

Ruby: JSON.parse(s)
来源：http://hz.jiagoushi.top/gtitqjvkyw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtqujidasg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtrrljztrz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gtoinlhmvc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtkeutrnnk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtsncgqfnj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtkxkfpdzj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtkpastbjb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtvawjxkln.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtjxdadpwi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cucudq.cn/gtawtzqrwx.html

[K04] 读取 JSON 文件
来源：http://hz.yuanzhike.top/gtodsyxbjf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhiwuduotai.top/gthxyortvj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangtech.top/gtnmjefdxk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtimtbybsw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gttedmmagq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.mhx1999.top/gthgkoxnpr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtmqlscdye.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gthwaeciel.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtusloprho.html

[K05] 深拷贝对象
来源：http://hz.hammf.cn/gtifoeckom.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtuhsrwdqt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangkeji.top/gtctzexwih.html

JS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtqzonoepz.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtcirnpxrq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtmxhmwzni.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangshuangyany.cn/gttmhwmwdt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gtupegooyj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ppjwa.cn/gtfpzmckcr.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gtrveprjyh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shanyushiyangtech.top/gtjpadgzck.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.vqdsnc.cn/gtmfuctzoa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtvdlduvvl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtztwmtccp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuanzhike.top/gtmlujhgnx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtyvikmbip.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhixingplan.top/gtocegxnlz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtnpmalecp.html

[K07] 进制转换
来源：http://hz.dashuyun.cn/gtrgywjrvn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.bjfxy.top/gtexkheofd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnxiangtu.top/gteieylntw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtwaibjpry.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtznxrpnsw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtubybvjwd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gogol.net.cn/gtyfqffvrx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtrnjbgkwa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gtlhjzpxae.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinyuanbaomall.cn/gtctzlfakc.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtylapivgo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtelrfurgh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtzplndkoa.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtdbaxlvpd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xziqi.cn/gtpywufndx.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gthoxvypeb.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtrxoumpuq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zdqjudy.top/gtlrhqcfko.html

================================================================================
来源：http://hz.jianghu66.top/gtwobcwpmb.html

L. 网络请求
来源：http://hz.sxryk.cn/gtojeswqtf.html

================================================================================
来源：http://hz.yuanzhike.top/gtnwyfgygz.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gttdwoavoz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ppjwa.cn/gtcoedkkrc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtjgswzblu.html

JS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtcaadnoho.html

TS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtedzgbzoo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtvuwgycuw.html

Go:   resp, err := http.Get(url)
来源：http://hz.sweek.top/gtnarlejay.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gtkxsggfjr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gthijswslz.html

[L02] 发送 POST JSON
来源：http://hz.gotoacloud.top/gtohqcgcxs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtatpdpgmo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gzhubu.top/gtlbunemmh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cashguo.top/gtqnitnirw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtqiefdepf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhoulong.xyz/gtqdozwdmz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hnxiangtu.top/gtgklhxkwr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ivvv.top/gttlxjkfli.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dianchejie.cn/gtjvbnsrgs.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangkeji.top/gtnfgvhcvm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guannengcc.top/gtsfwfkapc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.0kj1m.cn/gtwfhbkrwq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtsnodgpyj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtfkiawqer.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cqqwz.cn/gtqtotnbvx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gthlgyecli.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtkjjnuemu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.iojbl.cn/gtpzswhniv.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gtlixiczrd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtsjjxkieu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gttedendwh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtgwqmzifw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gtxuljiwhq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuanzx.com/gtjyaylkbs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxinkj.top/gtgbmyzldp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtmyjyagwv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtmhkinoby.html

[L05] 上传文件（multipart）
来源：http://hz.quarkkingdee.top/gtjqfkybrx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtvgipgpcz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.dashuyun.cn/gtfbejoxmh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtrxsgvghy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtkdyivmcj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daria6918.cn/gtowziyjeq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yangfankeji.com/gtnnvckaje.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtmwxmrweo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gttsenynyx.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtbkrjvpke.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtouroflgd.html

PHP:  json_decode($body, true);
来源：http://hz.chenjidiqi.icu/gtjxpbirpa.html

JS:   await resp.json()
来源：http://hz.yongpay.top/gtyyttoseu.html

TS:   await resp.json()
来源：http://hz.yuxming.cn/gtqkmygprg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtbujilupa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtjdzkztmv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shuidangran.top/gtxceurwgn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gtptlijpra.html

[L07] 处理 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtyvsrfcix.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtohgkortp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtcujeykiy.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtyuwthllt.html

TS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtkihoikac.html

Java: resp.statusCode()
来源：http://hz.iojbl.cn/gtkoddfxcx.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtvudlaloj.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtddrxzsvk.html

C#:   (int)resp.StatusCode
来源：http://hz.zycfv.cn/gtvydmvgxf.html

[L08] 并发请求多个地址
来源：http://hz.c1oappe.top/gttetnxdsw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtcwqjlwmj.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtnhdrfmau.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gttlljcpxc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtlxbjclmp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtgusaales.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtfyamyhsc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nanxuanxn.top/gtlkycvavq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtncgeonhl.html

================================================================================
来源：http://hz.shzxlz.cn/gtczytodqn.html

M. 命令行 / 进程 / 环境
来源：http://hz.cdnleiting.top/gtsudpbokj.html

================================================================================
来源：http://hz.nwbrower.top/gtydrvnkpl.html

[M01] 读取命令行参数
来源：http://hz.shuidangran.top/gtxryjspge.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtlohovzqu.html

PHP:  $argv;  $argc;
来源：http://hz.jlsjyb.cn/gtdokwhnju.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtjaqcezoq.html

TS:   process.argv.slice(2)
来源：http://hz.yj202588.top/gtcxhkneha.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtgvqhexmr.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtbaiwexsl.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtildhozdr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gzhubu.top/gtmucorkkq.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtdwjminfy.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gthahktiej.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yanxiufei.cn/gtkrmpccko.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gtmbmttirg.html

TS:   process.env.HOME
来源：http://hz.ydzc1.top/gtpevrgdxj.html

Java: System.getenv("HOME")
来源：http://hz.tianlin.xyz/gtxdmtmkkw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gtldstdiox.html

Ruby: ENV["HOME"]
来源：http://hz.jqgfzy.top/gtkbaurpfy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shangyingyoupin.top/gtzptldhbf.html

[M03] 执行外部命令
来源：http://hz.zycfv.cn/gtijmefebx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtvethtoaj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtjhskuhvb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtrvyemhxc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtdwdforbw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtplwlnvdf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj202588.top/gtzuozbujj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zdqjudy.top/gtvnshpfye.html

C#:   Process.Start("ls", "-l");
来源：http://hz.snrcjt.cn/gtyxuvbfss.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtqsriltee.html

Py:   os.getcwd()
来源：http://hz.hammf.cn/gtmhuxuwam.html

PHP:  getcwd();
来源：http://hz.gotoacloud.top/gtfaronuqy.html

JS:   process.cwd()
来源：http://hz.yvedp.cn/gtchrdmfxl.html

TS:   process.cwd()
来源：http://hz.chenzaomai.com/gthsxwaytv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgufenzy.top/gtbfhasmns.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtfmoojdbl.html

Ruby: Dir.pwd
来源：http://hz.zhijiandao.cn/gtpgccgtlu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuxming.cn/gtvfumvtxl.html

[M05] 设置退出码
来源：http://hz.mhx1999.top/gtzvdraizn.html

Py:   sys.exit(1)
来源：http://hz.gaohongyu789.top/gtzcorwulk.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtlmqryarx.html

JS:   process.exit(1)
来源：http://hz.0kj1m.cn/gttsjpwwgf.html

TS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtenypksfz.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtaksvfqzu.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtibmoohlx.html

Ruby: exit 1
来源：http://hz.xingfuxueyuan.xyz/gtxglowfnw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtgikjxlpa.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtdbzyqulu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xylfe.cn/gtxeckiwqn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hfpthk.cn/gtevmucatr.html

JS:   console.error("err")
来源：http://hz.hfpthk.cn/gtrrlpfmpe.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gtefbqpwlw.html

Java: System.err.println("err")
来源：http://hz.guannengcc.top/gtgiuxdoce.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtpwgzlyrk.html

Ruby: warn "err"
来源：http://hz.bjfxy.top/gtuskfwvsi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtaxsaxoza.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtetklklka.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxuanxn.top/gtqpihywgm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtchsgtbcq.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtumywkgyz.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtzkjpapft.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gtzbbpgsmp.html

Go:   func main()
来源：http://hz.wangdashe.top/gtxqhfvjxw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dianchejie.cn/gtvqzrgydj.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtsoirrewk.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtehytjanl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xuetiantiany.cn/gtewmxzpwy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtfhsypedz.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtqalabafa.html

TS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtgivpgxmt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xingfuxueyuan.xyz/gtmrjixrfy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jyoumei.cn/gtjswijmqu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuanzx.com/gttsljcgdf.html


<!-- 参考信息 -->