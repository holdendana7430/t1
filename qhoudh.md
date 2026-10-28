代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtlgdgemhq.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtmsrvsvut.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtehkojlax.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtjvcsgmzg.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gtfsgzpvkb.html

Ruby: Time.now
来源：http://hz.wangshuangyany.cn/gthdolmfze.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtsyvmipfn.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gtkyjphgnt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtmlltxhju.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cucudq.cn/gthkfpoqcm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gttxdknaju.html

TS:   d.toISOString()
来源：http://hz.havefunace.top/gtfupmqana.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtfetucxgp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtqxdbvqcp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtmussebsy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangtech.top/gtvqbowvph.html

[J03] 字符串解析为日期
来源：http://hz.guowangkeji.top/gthcjnkwrt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.quarkkingdee.top/gtwpdagmro.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtjdnqmzem.html

JS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtglbqkqxe.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtuabxrrph.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtvemacahd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fengsongda.top/gtsoutcbuc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtujaxjloa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.haohaochexian.top/gtaloijrpw.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtwzdbtkgz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtylwawooh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gtwqiukigy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtsdyknscg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.meibo888.top/gthvozrkvj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtiuyinetb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.havefunace.top/gtsrifqnjm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtjfgxydqw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.svipenyu.cn/gtepknxgzh.html

[J05] 时间加减（加 7 天）
来源：http://hz.ivvv.top/gtixbyiloh.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtpkyefwxg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gtcfsejqlr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtgyxlwddi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtcrgddrej.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtqlokljvw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtywoxlsdt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxinkj.top/gtwdgqgcsy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shuidangran.top/gtxlfgcijt.html

[J06] 计算两时间之差
来源：http://hz.gaohongyu789.top/gtjhkdalyw.html

Py:   (end - start).total_seconds()
来源：http://hz.chenjidiqi.icu/gtkhaxxryy.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtqbxishar.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtnvjulauk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gthvphhlvk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtgsquagap.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigufen.top/gtgagdfkzj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gteelotkew.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtacvplziu.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtcvqqamgt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtaqnzbacs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtobonvqlf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtaidmltvq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtueujrbfz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gogol.net.cn/gtrghscyec.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tian-w.cn/gtcesxnkhd.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtbbgpcygg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtpfzmgvgj.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtzseqsvfb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cheryme.top/gtoyjzysoi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hnqzz.top/gtnkdammge.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gtqqwejeiy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtrhmhbnad.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guowangkeji.top/gtlhnkskor.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtysptaaat.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xziqi.cn/gtznylqgvj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtmjaszyeh.html

[J09] 时区处理
来源：http://hz.nanxinkj.top/gtsfaywtxh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtdtoexuzk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sysykeji.top/gtoteounes.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtjrnilcho.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtlwnvksjz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtbnshrqhs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jlsjyb.cn/gtgplufkqr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gtlzaqobgy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tanke756.top/gtwvzmwtak.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtlhumpini.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cqqwz.cn/gtdwnetxzn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.c1oappe.top/gtenlummxl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ybcxt.top/gtzcefbivm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtbsrpgqxv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gtvzddmdme.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgufenzy.top/gtzslsyevv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtauwfsqvm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gttxcriekj.html

================================================================================
来源：http://hz.ivvv.top/gtxzwgiqok.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtpdjzrrvm.html

================================================================================
来源：http://hz.snrcjt.cn/gtmqjsfwzu.html

[K01] 对象转 JSON 字符串
来源：http://hz.sufxvd.cn/gtcihiwpqb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtxbtakats.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtummlitqi.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtcumfczdk.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtnzrqnqdz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtvstvaksb.html

Go:   json.Marshal(obj)
来源：http://hz.9152youxi.cn/gtualuimas.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtojeafwoi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtkewujtra.html

[K02] JSON 字符串转对象
来源：http://hz.jyoumei.cn/gtzgzifkcj.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtwdfrmjlg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gttwutrigp.html

JS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtzciieyhv.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtimliffkq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ywan-chungtsiang.top/gtyjlrwjch.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtdhpatcko.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtpovxomkw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gtnysiyvxg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtetdmmdts.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gthvalpagw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtahzizini.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtxdbtdfxy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtyilslfbj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenzaomai.com/gtnxczcctp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pengpengdd.cyou/gtofulvdmv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtizhtrxhd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gteybtlwlz.html

[K04] 读取 JSON 文件
来源：http://hz.sysykeji.top/gtgqtnygxp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.9152youxi.cn/gtiwskvilw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtjhmuplxw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtrvjmikxt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtwzjbwrtr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtxuajlqoq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtvnjzcxix.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtxbhddrcz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtmyqxsisy.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtynrswusb.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtjlczgdbv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnqzz.top/gtsfvqyxnp.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtqfkbanqm.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtqazrzngn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dianchejie.cn/gttmtmdmkx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gthmtdxubs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtuyceqpfw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenzaomai.com/gtlugrrbzh.html

[K06] 解析 URL 查询串
来源：http://hz.sufxvd.cn/gtaipiwhkp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gttklhcdtt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtdgqhlqrq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtyfxwgcmt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtetscnaxx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tian-w.cn/gtufbfccsb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gtemnbqwcf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtmnizuewf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.redwolf501.top/gtwsssjihx.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gttmijcmmb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jlsjyb.cn/gtqwqnsmuk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gttsokmras.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtxoiypqml.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtybvedpvn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtxwjilllv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtsaqidtrk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigufen.top/gtaylfapjv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sweek.top/gtqfzefxwi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtiqeqjgym.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtxgvaajyy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtospdzjmh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtkklgvefn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtkmjfioko.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtqtxljjwh.html

Go:   encoding/gob
来源：http://hz.hnxiangtu.top/gtodwbabqv.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtxuwxogfk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtuhehnpta.html

================================================================================
来源：http://hz.redwolf501.top/gtvagurcqh.html

L. 网络请求
来源：http://hz.tanke756.top/gtokaissss.html

================================================================================
来源：http://hz.gogol.net.cn/gtqtuctaye.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtgcempynn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtajtvzfgh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtrpwgtwts.html

JS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtzjenevjz.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtblkydfqv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.andypj.xyz/gtfkhcxwuf.html

Go:   resp, err := http.Get(url)
来源：http://hz.hywenlv.cn/gtqjdlulwj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pengpengdd.cyou/gtwzklirdf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtkzcihflz.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtzhrybxsg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dashuyun.cn/gtumcekrgr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgufenzy.top/gtbnmdcwrd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtznsspxoe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtheifybiy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtiggqrctc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtlbafmzzc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shzxlz.cn/gtzoiyxqyv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aibaodan.cn/gtrdeuhtdl.html

[L03] 设置自定义请求头
来源：http://hz.jinyuanbaomall.cn/gtdahjdsjl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtqrlshbtb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sweek.top/gtdlvjbwaj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtxtknwars.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtrgzpiuyh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinqigufen.top/gtxtoucmdk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ivvv.top/gtdswrvtzq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aibaodan.cn/gtbpoilpqq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gthslipcbo.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtieiyalud.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aibaodan.cn/gtppxgdyxw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinyuanbaomall.cn/gtjqaixpag.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtnucyhxhy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shzxlz.cn/gtfdxduyul.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gtkmekihjt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhiwuduotai.top/gthhdpiopo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtrparpkse.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guowangkeji.top/gtedtwyhjg.html

[L05] 上传文件（multipart）
来源：http://hz.xingfuxueyuan.xyz/gtrzzykakb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gogol.net.cn/gtspcrrins.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.quarkkingdee.top/gtnpoljlby.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtyeenqfhb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtadoalemo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhongyouzk.top/gtdziafcrn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenjidiqi.icu/gtvhllgydu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aibaodan.cn/gtlrvjlgfn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtldmqgjga.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtyfoavjpe.html

Py:   resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtueswkvhi.html

PHP:  json_decode($body, true);
来源：http://hz.xingfuxueyuan.xyz/gthjnadngt.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtutffrrge.html

TS:   await resp.json()
来源：http://hz.fzhhl.top/gtivayzdim.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.smart0.xyz/gtsuiischt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtcilvlhfc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shangyingyoupin.top/gtvbbhlyrl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ybcxt.top/gtnhjnmcmy.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtevjsageh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cucudq.cn/gtwfghpuaz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258.top/gtrqsxqtyd.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gthlantwha.html

TS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtceqjhcfp.html

Java: resp.statusCode()
来源：http://hz.smart0.xyz/gtddpftrga.html

Go:   resp.StatusCode
来源：http://hz.zhengqikj.top/gtyfsqfqiy.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtdnmqwgck.html

C#:   (int)resp.StatusCode
来源：http://hz.zhengqikj.top/gthkjumbqu.html

[L08] 并发请求多个地址
来源：http://hz.zhaomingkeji.xyz/gtkpdmoxiv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtowlbzvqe.html

PHP:  curl_multi_init() 系列
来源：http://hz.shangyingyoupin.top/gtqfofjgwo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtvqbxdaaw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtldpdqoco.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nwbrower.top/gteaeqyorr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.birdmap.top/gtcpjnvdxc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtpdagqoub.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.andypj.xyz/gtzsnnyqzb.html

================================================================================
来源：http://hz.fengsongda.top/gtlyxzkczu.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtctiwpmzf.html

================================================================================
来源：http://hz.hfpthk.cn/gtgezdmxbt.html

[M01] 读取命令行参数
来源：http://hz.hongshengwenyu.top/gtooewefns.html

Py:   sys.argv[1:]
来源：http://hz.guowangkeji.top/gtlbwyowgf.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtndinblyt.html

JS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtyzcytmvc.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtfaxfktve.html

Java: args 数组（main 方法参数）
来源：http://hz.c1oappe.top/gtdidhtmwm.html

Go:   os.Args[1:]
来源：http://hz.svipenyu.cn/gtxcrqqdkp.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtkdedvyst.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yanxiufei.cn/gtzeqesenk.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtimbfjxtj.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtheulyxdt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.dianchejie.cn/gtmfrxorvw.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gtpfekumuf.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtbzluzkns.html

Java: System.getenv("HOME")
来源：http://hz.52xcode.cn/gtvgelbpep.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxinkj.top/gtniejsrve.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtettbvpjv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.redwolf501.top/gtwmxprlbr.html

[M03] 执行外部命令
来源：http://hz.fzhhl.top/gtyxehltcz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xylfe.cn/gtvdazibbe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhaomingkeji.xyz/gtyjgcueop.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtfjvvtzla.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtneasonej.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gttazoyxxk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtijmgkoec.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.kuanghao11.cn/gtpdahxhsu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hongshengwenyu.top/gtlozjkyzm.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gthpxiijyo.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtfbmykskm.html

PHP:  getcwd();
来源：http://hz.jqgfzy.top/gtsupsyxjp.html

JS:   process.cwd()
来源：http://hz.ivvv.top/gtaidxyape.html

TS:   process.cwd()
来源：http://hz.zhongyouzk.top/gtihmckzlz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtcktxvywf.html

Go:   os.Getwd()
来源：http://hz.quarkkingdee.top/gtvwvogksu.html

Ruby: Dir.pwd
来源：http://hz.yanxiufei.cn/gtwtyecbws.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nwbrower.top/gtaffhbrtl.html

[M05] 设置退出码
来源：http://hz.guowangkeji.top/gtyivhyhba.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtbzwzbugi.html

PHP:  exit(1);
来源：http://hz.iojbl.cn/gteoxsnaje.html

JS:   process.exit(1)
来源：http://hz.dianchejie.cn/gterdueujz.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtsucoouwz.html

Java: System.exit(1)
来源：http://hz.dianchejie.cn/gtdlmenmyw.html

Go:   os.Exit(1)
来源：http://hz.hfpthk.cn/gtfggnunkp.html

Ruby: exit 1
来源：http://hz.zhaomingkeji.xyz/gtphnmoeuj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xziqi.cn/gtwfiktdba.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gtkposwgvv.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtcfwoqozz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtfjljrnmx.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtgtdzeaav.html

TS:   console.error("err")
来源：http://hz.dashuyun.cn/gtfaqvgwmp.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtiobwvxzh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ybcxt.top/gtmqqhcugt.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtjtkykqeu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.birdmap.top/gtkjcffzhn.html

[M07] 判断是否为主入口
来源：http://hz.316326.xyz/gttmuwedxe.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gtozqsyyzi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zdqjudy.top/gtjtnplsbr.html

JS:   require.main === module
来源：http://hz.haohaochexian.top/gtzxdnbrek.html

TS:   require.main === module
来源：http://hz.aibaodan.cn/gtifregleb.html


<!-- 参考信息 -->