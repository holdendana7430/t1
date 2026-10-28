代发 wailian999

Go:   time.Now()
来源：http://hz.daxiang520.top/gtukjwhcwu.html

Ruby: Time.now
来源：http://hz.zycfv.cn/gthaiusqfe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtweysqolo.html

[J02] 格式化输出
来源：http://hz.kuanghao11.cn/gtpadrdlgf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtrpzebljw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtgnsrmcuq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtsbqpkdeo.html

TS:   d.toISOString()
来源：http://hz.yvedp.cn/gtusvdwdkf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jyoumei.cn/gtdmjtwvyr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.c1oappe.top/gtdbquqbnx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtqzaofhvc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gtfrcdkvnh.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtjwsodbow.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ivvv.top/gtjvykexrh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yanxiufei.cn/gtprwkbios.html

JS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtotkunseo.html

TS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtcgyybebk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gtrxeyvquk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtvhkfskss.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtmkmjfeoj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gttuqguqer.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtcxilybxw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtubyladpe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtlfpwgyxx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jiagoushi.top/gtpbqionjv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtvtuwvluq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gtesenoaxc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.quarkkingdee.top/gtubhekpym.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtsfmmnlpa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtwybijjhl.html

[J05] 时间加减（加 7 天）
来源：http://hz.quarkkingdee.top/gtpyqpeaen.html

Py:   now + timedelta(days=7)
来源：http://hz.zdqjudy.top/gtzardenot.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtjmeccgru.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtcsaagesp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtktbcrndm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgfzy.top/gtowhkarue.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtaxdsyxsk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gteiquktzz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sysykeji.top/gtaoogsazk.html

[J06] 计算两时间之差
来源：http://hz.hammf.cn/gtwfvswcaw.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtxijemhth.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtwtswdwzg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtdhbxusfk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxinkj.top/gtewwjwoqs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtouyekkis.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigufen.top/gtmaqbriit.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtjkghofqa.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangdashe.top/gtiywsyetb.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gtwpozrxfr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtxupoqntm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtrnepxabf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtrjbfsuyc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gttzxgofjk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtpluslfsw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtcwwsekyt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gterfxvzpq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtznloqjuf.html

[J08] 提取年月日与星期
来源：http://hz.zhoulong.xyz/gtmiqkfwnt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jianghu66.top/gtxbovlwan.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gtouapuqqv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.svipenyu.cn/gtksvjaift.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sufxvd.cn/gtzqbptlhu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258.top/gtzjnqbnlf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtngmqkgif.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj202588.top/gtbkeiuiwf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtpeijdelp.html

[J09] 时区处理
来源：http://hz.hnxiangtu.top/gtnfwmqcph.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtjjtwjvmf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dashuyun.cn/gtfjquqouq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtlcoliigz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtoyygpmji.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtakmoetwz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtrwjvrvhh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258888.top/gtllgrcpiw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daxiang520.top/gtgwwdnxzb.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtsqxmpnhx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtatitqgik.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtcdpciwoj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtrpdcxosq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.feifeiyinyue.top/gtotcdtenm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtvyrmqafy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gtfdewxlma.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gtaqbrdsup.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.havefunace.top/gtexiipqxh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtlbrmxlxq.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gtytpdxmdj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjopdvjkb.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gttltugquk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtnvzrukda.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jiagoushi.top/gtppdtjtes.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtmwzessio.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtrjytqvfq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.havefunace.top/gtqgvadxdi.html

Go:   json.Marshal(obj)
来源：http://hz.yueranfly.top/gtncbdpuna.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gogol.net.cn/gtlexwbjvx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtucmmrcss.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtfvewwdqb.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtafponaiq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.kuanghao11.cn/gtvqikuwry.html

JS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gtjnbaxlut.html

TS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtvrhauykv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daxiang520.top/gtgnenmudj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtbeozhyhd.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtgsxnrqci.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtggcbmdbi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.andypj.xyz/gtanfviczy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtvkkcmoxa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtnvcuwrtw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtjxejoivo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtooreyjca.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtejpmarhr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dianchejie.cn/gtkqxgispw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gtkjatvbbe.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jyoumei.cn/gtnqtwaoef.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gtyofhpsra.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daria6918.cn/gtcogtawkx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtbrygnkbv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtecmeqbwv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gthqncteqr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtbsubfsfy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtkvcjvoeb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gtwakrbeoc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtvoznsiwk.html

[K05] 深拷贝对象
来源：http://hz.zhixingplan.top/gtcwsiqovp.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtjipfttfw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gtgklshzue.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtujfgngza.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtekrpwpqs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtgvdlzmpi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.andypj.xyz/gtahebfkie.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.feifeiyinyue.top/gticvxeaaa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gtdzgcgvou.html

[K06] 解析 URL 查询串
来源：http://hz.quarkkingdee.top/gtdklahjau.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtmbipjtvw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtybbqzccs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtokrkwejk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gthqjtgtvu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtdnrojkrg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.316326.xyz/gtxlnjlsia.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtoemyxkbh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fengsongda.top/gtppouqvgx.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtffvsefgj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yvedp.cn/gthpfnvrcg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zdqjudy.top/gtpetnvsqp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtmkrtekqa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtdqcdlrzi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtspzrmdmt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtgwhymzyz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtkayqbahk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gtwsxspeyk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtvmlniyjy.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtrnwztvmr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtxyhqtnlz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtfbdjyzyf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtaryakyyo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuanzhike.top/gtyleuxign.html

Go:   encoding/gob
来源：http://hz.xuetiantiany.cn/gtnlbwhxbv.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gtuhpxoewc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cqqwz.cn/gtkhaktqhf.html

================================================================================
来源：http://hz.ivvv.top/gtgxzrnaad.html

L. 网络请求
来源：http://hz.yj20258888.top/gtfmvnbyee.html

================================================================================
来源：http://hz.xylfe.cn/gtndwukecs.html

[L01] 发送 GET 请求
来源：http://hz.gzhubu.top/gtifychzgx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258.top/gtmkfugech.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gttcaltdfn.html

JS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtlbwlzvun.html

TS:   await fetch(url)
来源：http://hz.shuidangran.top/gtmlecypcg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtspikkfka.html

Go:   resp, err := http.Get(url)
来源：http://hz.vqdsnc.cn/gtxxytyqmj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gogol.net.cn/gtvcggcctx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tianlin.xyz/gtadcmmnum.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtmdfbjnkf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhongyouzk.top/gttlhnyqwf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtmsztrlch.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gttyaqygud.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtfvsjovbp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinghuilouyu.cn/gtkbxbnkit.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtfoptrskk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hywenlv.cn/gtbtlieqwb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cheryme.top/gtaeqfywgo.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtnfhmqibc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gaohongyu789.top/gtlquzmmbf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtdqzxznrl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtkjbtkgnj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtpujzcjwt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gtvxjboidq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gttysubpuj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ivvv.top/gtrhkauqou.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtomivojsj.html

[L04] 设置超时
来源：http://hz.quarkkingdee.top/gttkxzskna.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtmmkywaye.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtvdjhwijs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtnofyhuxc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtdgpbkdmj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gotoacloud.top/gtevirzinh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtzvyzcrci.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtahnhfypz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yonumen.top/gtuldpznwh.html

[L05] 上传文件（multipart）
来源：http://hz.yonumen.top/gtyaduljbq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtxtydvcdn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.andypj.xyz/gtnjihldwb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtplfrgfpw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtcyzzecwu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenlongwang.top/gtqqdarkjz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxuanxn.top/gtfguxqdty.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtmsvpergx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtcszjtxxq.html

[L06] 解析响应为 JSON
来源：http://hz.jqgufenzy.top/gtwlvqxiix.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gttzkeldmm.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtcrqitlri.html

JS:   await resp.json()
来源：http://hz.guannengcc.top/gtwcxmzyyq.html

TS:   await resp.json()
来源：http://hz.sweek.top/gttamhscgx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xylfe.cn/gtqqgrnkkc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtigufxckq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenjidiqi.icu/gtuzfgyojs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yangfankeji.com/gtzgbyhyat.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtkjicavcf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jiagoushi.top/gtxnhbddyq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gtlntsfuiv.html

JS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtlxmdonov.html

TS:   resp.ok;  resp.status
来源：http://hz.sysykeji.top/gtrockvmxc.html

Java: resp.statusCode()
来源：http://hz.aibaodan.cn/gthatwshbl.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtysuulpfk.html

Ruby: resp.code.to_i
来源：http://hz.zhoulong.xyz/gtroceuvlw.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtthnfbjib.html

[L08] 并发请求多个地址
来源：http://hz.yuxming.cn/gtltfkhrnu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxinkj.top/gtwkqklkwp.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gtypihoina.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dashuyun.cn/gtoccsuuae.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtfcdwzcvz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtejmbpheu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zdqjudy.top/gtnvutngtx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hammf.cn/gtylfvtpwe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nwbrower.top/gtfowaaphe.html

================================================================================
来源：http://hz.havefunace.top/gtucoubctb.html

M. 命令行 / 进程 / 环境
来源：http://hz.cheryme.top/gtdfkdiest.html

================================================================================
来源：http://hz.tianlin.xyz/gtmprbnixz.html

[M01] 读取命令行参数
来源：http://hz.hammf.cn/gtwsxrlaoi.html

Py:   sys.argv[1:]
来源：http://hz.daria6918.cn/gtwflctfze.html

PHP:  $argv;  $argc;
来源：http://hz.ywan-chungtsiang.top/gtecklblfq.html

JS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtbtbszghh.html

TS:   process.argv.slice(2)
来源：http://hz.jinyuanbaomall.cn/gtmmxafcjv.html

Java: args 数组（main 方法参数）
来源：http://hz.yj202588.top/gtfycgtbgl.html

Go:   os.Args[1:]
来源：http://hz.ppjwa.cn/gtnvnujebz.html

Ruby: ARGV
来源：http://hz.cdnleiting.top/gtatnrqlkq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jianghu66.top/gtvgadxyfs.html

[M02] 读取环境变量
来源：http://hz.yonumen.top/gtgvyhnoqq.html

Py:   os.environ.get("HOME")
来源：http://hz.yvedp.cn/gthcnwjeno.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtrgjqsjsp.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtkguebpcs.html

TS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtvazdtzmw.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtcpunkotl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhixingplan.top/gtdnjbcnoi.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtcyzaqjyq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tanke756.top/gtjxjwhvmb.html

[M03] 执行外部命令
来源：http://hz.mhx1999.top/gtvvfddusk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gtwncwjvxr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ppjwa.cn/gtzeapsmsq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtkszufctf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hammf.cn/gtkmtwzzcl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtzgsktaat.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhongyouzk.top/gtpnegdmyt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtbynccyvb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxinkj.top/gtsqlysyav.html

[M04] 获取当前工作目录
来源：http://hz.zhixingplan.top/gtehxijusn.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtctdqdkma.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtpkodwfgu.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gttmhuzwvz.html

TS:   process.cwd()
来源：http://hz.jinqigufen.top/gtvczytcbc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guowangkeji.top/gtjknggxvx.html

Go:   os.Getwd()
来源：http://hz.havefunace.top/gtrtdovrzk.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtqheyhvia.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuxming.cn/gtgmcczqmb.html

[M05] 设置退出码
来源：http://hz.jiagoushi.top/gtcokhaxnl.html

Py:   sys.exit(1)
来源：http://hz.nwbrower.top/gtiwugwajm.html

PHP:  exit(1);
来源：http://hz.smart0.xyz/gtsrntvisp.html

JS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtewyowwca.html

TS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gtmbvqrxkm.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtvaazimww.html

Go:   os.Exit(1)
来源：http://hz.fzhhl.top/gttpbrjssl.html

Ruby: exit 1
来源：http://hz.quarkkingdee.top/gtwtzcauhn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtiamlovcu.html

[M06] 向标准错误输出
来源：http://hz.hysaishi.cn/gtfpdroark.html

Py:   print("err", file=sys.stderr)
来源：http://hz.52xcode.cn/gtbuswemsg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.kuanghao11.cn/gtcuzkisnn.html

JS:   console.error("err")
来源：http://hz.jinyuanbaomall.cn/gtdavwuvhx.html

TS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtkyqojaqg.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gtwconuiro.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtsrmzsxch.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtiujdqeuc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtjgbgrnev.html

[M07] 判断是否为主入口
来源：http://hz.316326.xyz/gtolgqmshk.html

Py:   if __name__ == "__main__":
来源：http://hz.hongshengwenyu.top/gtynzttffe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangdashe.top/gtdbsdwsws.html

JS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtnhyxdpox.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gteinjibfc.html

Java: public static void main(String[] args)
来源：http://hz.aizwys.cn/gtdjumjejf.html

Go:   func main()
来源：http://hz.xylfe.cn/gtlrsemnyx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtqirdxqte.html

C#:   static void Main(string[] args)
来源：http://hz.ybcxt.top/gtdtvyghii.html


<!-- 参考信息 -->