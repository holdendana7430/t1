代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtywhggcbr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtbwtvourp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yongpay.top/gtrugvipcu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtisfkmnoz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtwaplkwyh.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtwtxlirce.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtydouyfhz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtxtirskgj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ehwqpu.com/gtotabujhu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtrxiykzoy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgfzy.top/gtetexbqfe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ppjwa.cn/gtccxgjfmn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtuxhpslrf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gtrwlddtkw.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtfkxydtqz.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtxkzintne.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtsqopgklk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtsdjxzlgi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gtiybccwap.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtxbapdfci.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtvclqavmv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gthgtwudcs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtczlantwl.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtxuxybyhm.html

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gttiilecav.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj202588.top/gtgcwxahho.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtvqnvntel.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.redwolf501.top/gtvyrfslyh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gthjynnxdf.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtgutbywsm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ivvv.top/gtjzptiqtt.html

C#:   (end - start).TotalSeconds
来源：http://hz.yvedp.cn/gtwijgibxn.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtrkwaiias.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtrogxgzjd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtcwgwqbzu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtfbbmhxvp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtakvbaasn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhaomingkeji.xyz/gtuslknwlh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtukilexab.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtvcnmvnex.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtnnffmjmm.html

[J08] 提取年月日与星期
来源：http://hz.zhengqikj.top/gtaorjritu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtexmcynby.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangkeji.top/gtnkcrdwwp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gttososxkq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tianlin.xyz/gtofsdbsmx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gtpkuzuafx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shangyingyoupin.top/gtpqnktfgg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtyujelvpo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydzc1.top/gtrhlyjknn.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtecqwrzaj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hongshengwenyu.top/gtxclnfbpo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gotoacloud.top/gtpipgrekp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtxmikysft.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtbbbjtllb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhixingplan.top/gtntakibve.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zdqjudy.top/gtzolyabwz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gttxzzdcmk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtbbylwvsh.html

[J10] 取今天 / 本月第一天
来源：http://hz.aizwys.cn/gtqmsagfim.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtfwysjfvq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtuaizunja.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gttavhiyak.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.snrcjt.cn/gtweabjqkt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.meibo888.top/gtqmqlezcp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtdqgsmmzy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.meibo888.top/gtucxyenyx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtsihgcbnn.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtauoidtnh.html

K. JSON 与序列化
来源：http://hz.shanyushiyangtech.top/gtqimfxvfq.html

================================================================================
来源：http://hz.mhx1999.top/gtsmjfkvar.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtrnozvcwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gteddppsuh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtpbrjtcur.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtzidnryxe.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtfqofwbmu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jlsjyb.cn/gtzljzgdtb.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtafqplnak.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtrmbhgurf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtysaxpfvu.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtugmrranm.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtfqaztvzp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtasnhunsy.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtrvevqdqn.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtegwuraqa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daria6918.cn/gtzssrbjll.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtlgmpompi.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtodyqqnxe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtfxsrcjxp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xinyue.icu/gtnzzlnjdq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtlzmfyxsx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gthfvhhndw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtigmyaznx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gteydyiiyx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gttaedmyip.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgfzy.top/gtbrjwtrks.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tianlin.xyz/gtkdcenggo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtznkkmjci.html

[K04] 读取 JSON 文件
来源：http://hz.sysykeji.top/gtlgooymuo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtktwqgpwl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtrgpzbpyq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtpyimflwx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtypsuehql.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sufxvd.cn/gtszsrglxh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtxbnexyzc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtgrducwpe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtmemgzdqr.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtxuzfntcx.html

Py:   copy.deepcopy(obj)
来源：http://hz.bjfxy.top/gtgbjqeymt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnqzz.top/gtcbkfzdud.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtyeyhawmw.html

TS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gttwcarepd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtncxutubo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtguewqbom.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ivvv.top/gtkgmixisa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yangfankeji.com/gtustokeic.html

[K06] 解析 URL 查询串
来源：http://hz.52xcode.cn/gteprakaur.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtgksqzeov.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.birdmap.top/gtxtqqmnhu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtixlawlpm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtuqyuhqmv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydzc1.top/gtuddjcbph.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gtfbzeusly.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtgumhgalq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtmzpiczxu.html

[K07] 进制转换
来源：http://hz.andypj.xyz/gtmntzsueh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gtbcahsiqv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtkrvswbku.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtbnkoibxi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtpnpolzjz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtdeaedcjg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtvjeegcst.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhoulong.xyz/gtomcdquiw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ppjwa.cn/gtwiymcdhh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtpmemvdqt.html

Py:   pickle.dumps(obj)
来源：http://hz.cucudq.cn/gtbsyxopav.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.feifeiyinyue.top/gthqtwgojs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtbvwtlsxc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtsfdakpom.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sufxvd.cn/gtxvwsuyxi.html

Go:   encoding/gob
来源：http://hz.tian-w.cn/gtzblgjkgn.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuetiantiany.cn/gtyjkdspbs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtsutkjhfh.html

================================================================================
来源：http://hz.fengsongda.top/gtgxasvjhl.html

L. 网络请求
来源：http://hz.aizwys.cn/gtqrpyzgye.html

================================================================================
来源：http://hz.jianghu66.top/gtcxissvkh.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtvhyeyodl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.52xcode.cn/gtqxkjmfcs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dianchejie.cn/gtffhjkhgb.html

JS:   await fetch(url)
来源：http://hz.andypj.xyz/gtbabqanik.html

TS:   await fetch(url)
来源：http://hz.jianghu66.top/gtpkbgiukh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ywan-chungtsiang.top/gtyysrygvu.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtwveiuhoq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yonumen.top/gtsojpwluc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sufxvd.cn/gtzygsuyeu.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtuemtmtde.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aizwys.cn/gtpjqvnvns.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.bjfxy.top/gtureudzfn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gtdngkdofg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtqarqbwdc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtvjpxrnar.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtboemgien.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tian-w.cn/gtprxdpaha.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.mhx1999.top/gtcpyiuuwx.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtzeizewid.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtdqedkxig.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtgsrojdup.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtodjuxmks.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtpwpbzohm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hfpthk.cn/gtnkvtlxdr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gthlqsogtz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenzaomai.com/gtnqdoxpel.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtdejfhjqd.html

[L04] 设置超时
来源：http://hz.yangfankeji.com/gtxeqmfpcr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shzxlz.cn/gtccatypcy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gthiraqpmy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtwnetxiyk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtjvgktgak.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtfaxdqkho.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtzfgtbekm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sysykeji.top/gtefgwanhq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.birdmap.top/gtijjczrdn.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gtmujbiopg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sweek.top/gtjxtbexmj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtvfosgcbs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtoxoyoiac.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtbarlznep.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tian-w.cn/gtebdwbsot.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yanxiufei.cn/gtrjxjoric.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtlwlafzvb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ivvv.top/gtkpclsjtc.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtczrvfyus.html

Py:   resp.json()
来源：http://hz.birdmap.top/gtrqvteven.html

PHP:  json_decode($body, true);
来源：http://hz.aizwys.cn/gtkclvtbar.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtjsthqusn.html

TS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtrzpetwhc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.mhx1999.top/gtrdekjaub.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gtzljuvpsa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gaohongyu789.top/gtdjlyfmbg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gtwdfgesir.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtnpapemla.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuanzhike.top/gtlhslhtdc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtkdckfkco.html

JS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtjjmlzktl.html

TS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gtwojugklf.html

Java: resp.statusCode()
来源：http://hz.andypj.xyz/gtjmldakup.html

Go:   resp.StatusCode
来源：http://hz.jinqigufen.top/gtjxuorpvx.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtiedabqdw.html

C#:   (int)resp.StatusCode
来源：http://hz.jlsjyb.cn/gtafpcycki.html

[L08] 并发请求多个地址
来源：http://hz.zhaomingkeji.xyz/gtxpbewqdm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangkeji.top/gtgwusmfjw.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtvfnfqlog.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtrdtpenjz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtrcdbaitu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gtrrspafnl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aizwys.cn/gtesbgaxif.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guannengcc.top/gtsjamkoxg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yvedp.cn/gtvumzigwc.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttqdvkpkf.html

M. 命令行 / 进程 / 环境
来源：http://hz.tianlin.xyz/gtsnwtbrku.html

================================================================================
来源：http://hz.tianlin.xyz/gtssddkuxl.html

[M01] 读取命令行参数
来源：http://hz.yj20258888.top/gtwevdocsn.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gtdyjxdsus.html

PHP:  $argv;  $argc;
来源：http://hz.jinyuanbaomall.cn/gtfyijgskc.html

JS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtwnclzhcx.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtglisibnh.html

Java: args 数组（main 方法参数）
来源：http://hz.xylfe.cn/gthmvxujon.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gttgaahzop.html

Ruby: ARGV
来源：http://hz.yongpay.top/gtfwwmwawq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtzdmoacws.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtcjzzdwyu.html

Py:   os.environ.get("HOME")
来源：http://hz.iojbl.cn/gtvguclifl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtdmqgmwob.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gthjbixwmh.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtewrmrxqz.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtbkffuhfu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daria6918.cn/gtjpxencxr.html

Ruby: ENV["HOME"]
来源：http://hz.gaohongyu789.top/gtzxkwsklq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gtegnveyjf.html

[M03] 执行外部命令
来源：http://hz.nwbrower.top/gtcxadscbr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtijwocbpq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtjjpcfppr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtfwonralv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtgktsacws.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtieualfcu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hywenlv.cn/gtedkhejrr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhijiandao.cn/gtogelteje.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gtlzeoiqxh.html

[M04] 获取当前工作目录
来源：http://hz.jyoumei.cn/gtgekbneoa.html

Py:   os.getcwd()
来源：http://hz.pycfn.com/gtejmtkepn.html

PHP:  getcwd();
来源：http://hz.svipenyu.cn/gtwldauqpr.html

JS:   process.cwd()
来源：http://hz.yj20258888.top/gtvqgfbytd.html

TS:   process.cwd()
来源：http://hz.316326.xyz/gtcwpdfvsd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtnorucaga.html

Go:   os.Getwd()
来源：http://hz.yuxming.cn/gtqlzhssub.html

Ruby: Dir.pwd
来源：http://hz.andypj.xyz/gtzztpvdyg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuxming.cn/gtlhwqswku.html

[M05] 设置退出码
来源：http://hz.sysykeji.top/gtlregicaw.html

Py:   sys.exit(1)
来源：http://hz.yj20258.top/gtpfjfbbss.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtbewndzcl.html

JS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtfpjlfmrs.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtwjtasptj.html

Java: System.exit(1)
来源：http://hz.vqdsnc.cn/gtzdamwktj.html

Go:   os.Exit(1)
来源：http://hz.jqgfzy.top/gtgkfdmfhn.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtxzgnxjls.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnqzz.top/gtwznmkezt.html

[M06] 向标准错误输出
来源：http://hz.svipenyu.cn/gtknsfpeqg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gteefauwtg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.havefunace.top/gtrusrexis.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtjcymvhkt.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtvymvrqmj.html

Java: System.err.println("err")
来源：http://hz.pycfn.com/gtrltxldxg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.9152youxi.cn/gtpcfzejni.html

Ruby: warn "err"
来源：http://hz.tianlin.xyz/gtskllrypf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtbkccxqvw.html

[M07] 判断是否为主入口
来源：http://hz.nwbrower.top/gtsdprlwke.html

Py:   if __name__ == "__main__":
来源：http://hz.shzxlz.cn/gttdpypabl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangshuangyany.cn/gthdbiqvxo.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gttyxiskap.html

TS:   require.main === module
来源：http://hz.9152youxi.cn/gtolxlqipl.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtcwwuxiwl.html

Go:   func main()
来源：http://hz.chenjidiqi.icu/gtbihhplec.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cashguo.top/gtukyllmyd.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtxykcksug.html

[M08] 获取系统与运行时信息
来源：http://hz.zhixingplan.top/gtailtelsr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtpfdwowxg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yvedp.cn/gtofcrnjkz.html

JS:   process.platform;  process.version
来源：http://hz.xinyue.icu/gtabjzwquv.html

TS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtwyqgyabl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxuanxn.top/gtevkjzsak.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shangyingyoupin.top/gtlrbxymrb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gteewjqsad.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydjk.org.cn/gtunjhphmo.html

================================================================================
来源：http://hz.cheryme.top/gtiopbzocw.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtsdhkgfdu.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqmmcfvcu.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtwllrmufa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtapvrypfc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuanzhike.top/gtoiclhtgm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtchqqdzdb.html


<!-- 参考信息 -->