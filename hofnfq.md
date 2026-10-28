代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtrzhmljjr.html

JS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtgkwxfnzz.html

TS:   new Date();  Date.now()
来源：http://hz.jqgfzy.top/gtlqomabtu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtdluzdmxp.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtiobxidzs.html

Ruby: Time.now
来源：http://hz.yj20258.top/gtzbizpygy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gtpnpljrtp.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gthdhvjbdj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtvidescod.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtofgniyyi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.havefunace.top/gtggnepayz.html

TS:   d.toISOString()
来源：http://hz.jinqigufen.top/gtkyeuejzl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gtrdeuwyyw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtobowyluz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtktzucmks.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sweek.top/gtvknzzuof.html

[J03] 字符串解析为日期
来源：http://hz.yvedp.cn/gtzhsuddrh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtjodenkbs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gttiellgax.html

JS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtgzxzjtaq.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtcnglknwy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtpbzhnmat.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtvyapqncl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtgbuvvdrp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtugqldrez.html

[J04] 时间戳与日期互转
来源：http://hz.andypj.xyz/gtjxrbtdfw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtwenasgnf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtrehnrlzb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shuidangran.top/gtypfoeziv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sweek.top/gtmzhnpnbk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtuhgbeeqs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtwbhurkyw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sufxvd.cn/gtlcpanyfy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtzxmtwmsu.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhiwuduotai.top/gtsbaaaiza.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtutqrgepz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtxpwfrser.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtbruwuvja.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gthvvpcjaz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtywmrxvfc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtdlfowwal.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jlsjyb.cn/gtyqqnpddj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258888.top/gtaafovkgo.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtezdpvelx.html

Py:   (end - start).total_seconds()
来源：http://hz.quarkkingdee.top/gtyqaciiug.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gthvyjacsf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenlongwang.top/gtbnmossmo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtsugolqno.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gtqhofsefn.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtaskoaail.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangkeji.top/gtbjphxwac.html

C#:   (end - start).TotalSeconds
来源：http://hz.svipenyu.cn/gtqahybcss.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gtmedkxawp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtjfehozdm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jianghu66.top/gtdoaljqou.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtsaiehywt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gthwixjyit.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtwtjwtqne.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gtrjhjromy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtbjqxjphu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtqofyadka.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtpvokmliw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtwicuoizc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtussxngwe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gotoacloud.top/gtzevrqucr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.havefunace.top/gtwcebinas.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigfzy.top/gtivnuxmno.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtgokyiuhw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gtntbkxhpl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtznewutpj.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtpczhbxza.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtwzoeghon.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtzxlzqcgn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtbnwntbqk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtfssityeq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xinyue.icu/gtrevnomao.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtpqgpbiyk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtzcxksnvx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xylfe.cn/gttjdedltq.html

[J10] 取今天 / 本月第一天
来源：http://hz.cashguo.top/gtozmcqabr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtjoeuzqfb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtujtjlpkb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pengpengdd.cyou/gtoqcjuauh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gtravusjiw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pengpengdd.cyou/gtfbmaynyn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.vqdsnc.cn/gtvoljeqec.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtecdsyfdh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.aizwys.cn/gtlkxaxerc.html

================================================================================
来源：http://hz.ydzc1.top/gtqmvoxyri.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtxyuwnsqg.html

================================================================================
来源：http://hz.ppjwa.cn/gtopqmgfae.html

[K01] 对象转 JSON 字符串
来源：http://hz.cqqwz.cn/gtzyyselly.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtmzrbchuz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtoommbdtb.html

JS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtpdpgtuly.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtbiohstui.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtydonaqlj.html

Go:   json.Marshal(obj)
来源：http://hz.hnqzz.top/gttkxvkjee.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhiwuduotai.top/gttyvhczwu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guannengcc.top/gtypfyjqst.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtygombvty.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtkqdziqql.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenzaomai.com/gtabigqzgo.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtvwsrcmue.html

TS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtbopmlwfn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtccqwpdrz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtvefwuvxy.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtufbcuoct.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gtsuecasjl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guannengcc.top/gtgysfgcxv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtahgyscft.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtgszbpjqm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtojpcrubo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gttawnpkvl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gtbsfqqnxk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtgzgjznug.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtuwjfuhqw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtvnbrhelw.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtfpzqhoim.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gogol.net.cn/gthplypqef.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtggioaxtf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtiiyqnica.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtxullefea.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gterzavedk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gtcmtkaxsm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daxiang520.top/gtebvjvhoc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtztxhosmd.html

[K05] 深拷贝对象
来源：http://hz.ydjk.org.cn/gttehtjhec.html

Py:   copy.deepcopy(obj)
来源：http://hz.yongpay.top/gteuqvjrsf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.birdmap.top/gtcgtnkvta.html

JS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtdmxqoiuf.html

TS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtjvmyxrbv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtjebepzut.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.andypj.xyz/gthwqznvei.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daria6918.cn/gtfdmbqpub.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tanke756.top/gtnansbsfj.html

[K06] 解析 URL 查询串
来源：http://hz.svipenyu.cn/gtumxzkgoj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.meibo888.top/gttevvthfl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.52xcode.cn/gtcklcmrcu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtvcgumzhm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtsfqreodi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hammf.cn/gtvbmlbqcn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gteilovqba.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gthlvcdevx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gthmlydrhj.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtuutvijbs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gttofbtany.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gtrprbitqz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtophoaooa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtbudsiszp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtypcqqdvk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtpfuthpqt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gtopnxwzcq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtarncwxwk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtfubehedp.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgfzy.top/gtixsfnllv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.smart0.xyz/gtilhtxowr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtmiblwitj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtongqfqtm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtoeiyugtm.html

Go:   encoding/gob
来源：http://hz.yueranfly.top/gtuiwppgde.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtcqpsxyaj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtdlsxjlok.html

================================================================================
来源：http://hz.zhengqikj.top/gtnbqochan.html

L. 网络请求
来源：http://hz.pycfn.com/gttalqijub.html

================================================================================
来源：http://hz.xylfe.cn/gthiivwewl.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtajwbpeus.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhoulong.xyz/gtlbsoyxbf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtjdtrznik.html

JS:   await fetch(url)
来源：http://hz.jqgfzy.top/gtwuewjkfx.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtkwkgttyi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhixingplan.top/gtuhcndyyk.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gthhfuzfpc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ehwqpu.com/gtdvsgvqnt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhijiandao.cn/gtcwyyhiac.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtkotbomdl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cqqwz.cn/gtdspjlzhy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gtihljybjc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtafdlemkv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtigxcwbku.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhoulong.xyz/gtahfnjoki.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuxming.cn/gtdmkgqywv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gthskxpdsi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtnwtcygmu.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gtopzrrcpp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tanke756.top/gttcobfxze.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.mhx1999.top/gtnnbwisjg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gthaqdsuud.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtvywyopku.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtileeuvqo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtoowsrkgv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tian-w.cn/gtpjgisuov.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gzhubu.top/gtyrrfvpwo.html

[L04] 设置超时
来源：http://hz.hongshengwenyu.top/gtgqzlqdzn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtujlbiuvd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.c1oappe.top/gtpfdljtqz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtysxoafpn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gttvjbfwuw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenzaomai.com/gtkraumchy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtcmcnuxop.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daria6918.cn/gtrfwrvfxq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.316326.xyz/gtfjrumoof.html

[L05] 上传文件（multipart）
来源：http://hz.jiagoushi.top/gttdtzqlfe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xinyue.icu/gtbqjmfofd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtbcbbxkdq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtxyctdjov.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shuidangran.top/gtdcixzbmb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gaohongyu789.top/gtnyrxlray.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guannengcc.top/gtrpzqcqyx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ppjwa.cn/gtwtmauabm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangtech.top/gtffbnndhb.html

[L06] 解析响应为 JSON
来源：http://hz.yangfankeji.com/gtwntpkhhc.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtxfnvwxrz.html

PHP:  json_decode($body, true);
来源：http://hz.xinyue.icu/gtwzuzvrpw.html

JS:   await resp.json()
来源：http://hz.jqgfzy.top/gtapotlyxr.html

TS:   await resp.json()
来源：http://hz.mhx1999.top/gtuvmpihga.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtrisclexy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gtnajlaiqs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtnudhyxme.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuetiantiany.cn/gtlzxzvtch.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydzc1.top/gtpzwtomam.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.bjfxy.top/gtcodjzjix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ehwqpu.com/gtpjkuqpie.html

JS:   resp.ok;  resp.status
来源：http://hz.chenjidiqi.icu/gtcwfmoplu.html

TS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtubxcqive.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangkeji.top/gtbpnbctty.html

Go:   resp.StatusCode
来源：http://hz.cashguo.top/gtqdufrokm.html

Ruby: resp.code.to_i
来源：http://hz.hywenlv.cn/gtlqquwudo.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtygcgrafa.html

[L08] 并发请求多个地址
来源：http://hz.xinyue.icu/gtiuyqsvjp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.bjfxy.top/gtbhbhntfj.html

PHP:  curl_multi_init() 系列
来源：http://hz.cqqwz.cn/gtabeibqoh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtwsvofwxo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtsmynvwcx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtdzyhddyj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuanzx.com/gtexeareej.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.52xcode.cn/gtflxzqdce.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cdnleiting.top/gtkhxxauex.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtuhzcxhfg.html

M. 命令行 / 进程 / 环境
来源：http://hz.guowangkeji.top/gtkwaixayw.html

================================================================================
来源：http://hz.tianlin.xyz/gtahlrfpmp.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtggdtofhk.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtdhwkawck.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtcempuyal.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtqjmbmand.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtyyfupolz.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtebupqooa.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtfvatnyqp.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtzdbmfiol.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gteiukhyqq.html

[M02] 读取环境变量
来源：http://hz.jlsjyb.cn/gtuevdmrje.html

Py:   os.environ.get("HOME")
来源：http://hz.hysaishi.cn/gtfwuzmkwu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.birdmap.top/gtphgpfqot.html

JS:   process.env.HOME
来源：http://hz.zhiwuduotai.top/gtgavjlxtq.html

TS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtpdohgcum.html

Java: System.getenv("HOME")
来源：http://hz.ybcxt.top/gtdgjlwzno.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtfabyikjf.html

Ruby: ENV["HOME"]
来源：http://hz.guannengcc.top/gtkjgyqgxx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gthndejebp.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtxqzymnvq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtrpfvyxqy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtebsgsrmz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtlsxmiode.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtonetmusj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuetiantiany.cn/gtdbrbabsj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yueranfly.top/gtrakhposi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sxryk.cn/gtmxvtewnm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.havefunace.top/gtthiygvak.html

[M04] 获取当前工作目录
来源：http://hz.haohaochexian.top/gtuudghxuo.html

Py:   os.getcwd()
来源：http://hz.havefunace.top/gtuzxnfcsf.html

PHP:  getcwd();
来源：http://hz.zhoulong.xyz/gtphlxjiun.html

JS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtegkzjuvk.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtxtlnlhyf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hongshengwenyu.top/gtcwqkauok.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gtsogoyxby.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtksxblypx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtzsrogtlh.html

[M05] 设置退出码
来源：http://hz.yj20258888.top/gtapxxdfis.html

Py:   sys.exit(1)
来源：http://hz.jianghu66.top/gttlydpmdf.html

PHP:  exit(1);
来源：http://hz.jinghuilouyu.cn/gtvmptsvlt.html

JS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtbqwdmpua.html

TS:   process.exit(1)
来源：http://hz.jianghu66.top/gtzpwhzqoe.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtierptnbv.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtwebkykyh.html

Ruby: exit 1
来源：http://hz.shzxlz.cn/gtqyrtlkjm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gtxpwyljkg.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtitvqjkqf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtnidxqtrc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydzc1.top/gtgespxewn.html

JS:   console.error("err")
来源：http://hz.yangfankeji.com/gtyoifcwrd.html

TS:   console.error("err")
来源：http://hz.dashuyun.cn/gtswrxvapc.html

Java: System.err.println("err")
来源：http://hz.pycfn.com/gtiagbawnf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.iojbl.cn/gtrafkggzo.html

Ruby: warn "err"
来源：http://hz.jinghuilouyu.cn/gtmgtdxmuq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.aizwys.cn/gtpixafwev.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtedrursbq.html

Py:   if __name__ == "__main__":
来源：http://hz.dashuyun.cn/gtzncdvzel.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtmxrxibjp.html

JS:   require.main === module
来源：http://hz.ydzc1.top/gtmuzjujpn.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtubikdhfd.html


<!-- 参考信息 -->