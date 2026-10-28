代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gaohongyu789.top/gtdbyobmib.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.birdmap.top/gtojqtawgv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtcudyvbds.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nwbrower.top/gtmdfvibqv.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gtsufzyhhj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinyuanbaomall.cn/gtjiwrehmf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtduexppjc.html

JS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtoogszrxt.html

TS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtverddngf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cashguo.top/gtrwljvpkl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cqqwz.cn/gtdxtgwxyg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtruxpzegv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhengqikj.top/gtddyacsul.html

[J04] 时间戳与日期互转
来源：http://hz.ydjk.org.cn/gtruulqiuw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtqtclhqym.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yongpay.top/gthuxdaspe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtmjoljlah.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangshuangyany.cn/gtodpzmhei.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtgcessjpb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fengsongda.top/gtiqvevyhp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pengpengdd.cyou/gtmwvltdlc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gtwtovstta.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtcnzwjrzs.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtqrgictzi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhaomingkeji.xyz/gtjqmjkjln.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtxlixnbuy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtrdbnluja.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtzxrizxdw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtaqiyiqym.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtdnpeouzz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shuidangran.top/gtopgqltug.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtbyzvldsc.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtsoxjhxkt.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gtuemfmnlp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtyghehlti.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtjgdfjrea.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtupkyflye.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangdashe.top/gthupxthqo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtpjnuuesd.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtcauhxmjw.html

[J07] 比较两个日期
来源：http://hz.cashguo.top/gtvxyysdcl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtpsyomcfj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtbeewtyog.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtuuynxlqd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtbpoxybbe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangkeji.top/gtylbnuwls.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj202588.top/gttmcaphdx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtinvahcfj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtwfcpvpfs.html

[J08] 提取年月日与星期
来源：http://hz.pycfn.com/gtscdevssh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtsnqsnkyt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yangfankeji.com/gtfmjzjscz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtnsfelvyw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinghuilouyu.cn/gtfvcqhvmk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtwkpjvqkm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtxoscpxmm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ywan-chungtsiang.top/gthkpsdtsv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dashuyun.cn/gtdffdsavy.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtnedyntff.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hongshengwenyu.top/gtpkxmzjmy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtprjksxed.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtfiwqeeol.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtapcfptoc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.0kj1m.cn/gtjlloxwky.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ivvv.top/gtuozmsiky.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gtccryofmc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gttfhwpefd.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtkonihual.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtuyexltky.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gtauxqbvxy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtityigtgy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangtech.top/gthmtxzzgs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hysaishi.cn/gtohahgjss.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtledgbtwo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtevbgtshq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtkzgmeexf.html

================================================================================
来源：http://hz.andypj.xyz/gtqkeitvmn.html

K. JSON 与序列化
来源：http://hz.ivvv.top/gtdmuhuucm.html

================================================================================
来源：http://hz.chenlongwang.top/gtkkzhcvyc.html

[K01] 对象转 JSON 字符串
来源：http://hz.bjfxy.top/gtzavpixiw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtqphcorxc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtkjbtikgq.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtoefdoizv.html

TS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtxxjvzzmu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtigsbckwf.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtbjkniupv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtnobmfpzh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtymxqcfrh.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtuyhojklv.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtxdtvhato.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.9152youxi.cn/gtpoivjgle.html

JS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtzwnoxtct.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtvyxmngva.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydjk.org.cn/gtdpablqlu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtpxkhfggh.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtgzisdjjs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cashguo.top/gtilltbckq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtfwutvvxc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtssjskjct.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenlongwang.top/gtuurvijkg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtzfxwaeox.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtpwfovkab.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cucudq.cn/gtryomlrcs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gthgqiokwi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yueranfly.top/gtyhnwhhhq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtdrkqfzni.html

[K04] 读取 JSON 文件
来源：http://hz.gaohongyu789.top/gtzkxftsej.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtjduswxab.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.dashuyun.cn/gtzlhotncq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.birdmap.top/gtmvijjygi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtfxkqrcay.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtmcbcwjmv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gogol.net.cn/gtdqdkawmy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xinyue.icu/gtyfobgpws.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.mhx1999.top/gtyqsdmnib.html

[K05] 深拷贝对象
来源：http://hz.hongshengwenyu.top/gtvvibhjhl.html

Py:   copy.deepcopy(obj)
来源：http://hz.redwolf501.top/gtgfnggfhk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtjfefgpkx.html

JS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtapvpqzvp.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtpmqqgupk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtneidbtge.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.mhx1999.top/gtqyrfcjfh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hnqzz.top/gtyaupksxv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hongshengwenyu.top/gtdakncnwi.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtsdcppebz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtwxyassuc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtkkrdfsrt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtshzwpaoj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtmlujhavr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtfyhfchwy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gogol.net.cn/gtksewxqou.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangdashe.top/gtfjphgfmv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtjtejdgsp.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtpidnbmrx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhoulong.xyz/gtkukxmqir.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yonumen.top/gtimimqnne.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtgkqnlndb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtmjdjuton.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtmewphkuw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jiagoushi.top/gtcqwdlsgt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtlnmkrlki.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tianlin.xyz/gtsymqpmyt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ppjwa.cn/gtbmldlrmf.html

Py:   pickle.dumps(obj)
来源：http://hz.fengsongda.top/gtaegbihfa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tianlin.xyz/gtnawbkxph.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sysykeji.top/gttlutticj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gttbvgtumr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.9152youxi.cn/gtevaoupwg.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtrquouxeg.html

Ruby: Marshal.dump(obj)
来源：http://hz.smart0.xyz/gtwynnmfuq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigfzy.top/gtmrncimpi.html

================================================================================
来源：http://hz.c1oappe.top/gtgefbgbdh.html

L. 网络请求
来源：http://hz.xylfe.cn/gtatvhcfcd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbbpyrfgz.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtudgsgyyc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gthspcafyd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dashuyun.cn/gtvotzkcln.html

JS:   await fetch(url)
来源：http://hz.nwbrower.top/gtsrzbaczz.html

TS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtnenoegds.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pycfn.com/gtclijcnsl.html

Go:   resp, err := http.Get(url)
来源：http://hz.hongshengwenyu.top/gtnqojkdgu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtywtnbjdl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yongpay.top/gtzvjkftlz.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtxbmnyiww.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258888.top/gtvkwzorgn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangtech.top/gtypduehwp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtxwxvvmkl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtjwarmzxw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydjk.org.cn/gtvsrqnxki.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhixingplan.top/gtkpkhtvrq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtpekxdzji.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pengpengdd.cyou/gtbujmdwlz.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gtxaombxqk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtarzntfur.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guannengcc.top/gtpejcwyea.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtdjelonfj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtwbwdrhtj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtwytwqjog.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtlglizisx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guowangkeji.top/gtawgbpoau.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guannengcc.top/gtnkhbkzkq.html

[L04] 设置超时
来源：http://hz.sxryk.cn/gtgkeijjbj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtmybvrnqa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.mhx1999.top/gtavearean.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtpgpwuwdo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtyqjyqqpj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtshljiwdj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gtfgjltity.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtycbnzeyn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ywan-chungtsiang.top/gtbfffizqb.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtdtfnrbgy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtvzalhadi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtqdlriyqj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtvmvihlvh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtcfoxzujr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gtuebfoevq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtyfalajdi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtvtoagvyb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cashguo.top/gtxqjmedih.html

[L06] 解析响应为 JSON
来源：http://hz.pengpengdd.cyou/gtpiiaakkv.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gtokyrgmre.html

PHP:  json_decode($body, true);
来源：http://hz.smart0.xyz/gtsvlkpqvj.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtzuoxyyfo.html

TS:   await resp.json()
来源：http://hz.sufxvd.cn/gthvctcmvd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtkcovokqe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gtxwkhftsn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtliuoogjd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtddnneprm.html

[L07] 处理 HTTP 状态码
来源：http://hz.snrcjt.cn/gtynmgnmsr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtmicnmxtg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtrrwbmere.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtgmxryxxe.html

TS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtfkfjbwpg.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gtcuablikq.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtddasykyn.html

Ruby: resp.code.to_i
来源：http://hz.mhx1999.top/gtyaqdbiew.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtwnjulxsh.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtfwhoroej.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtfpowrldx.html

PHP:  curl_multi_init() 系列
来源：http://hz.svipenyu.cn/gtghmpirgs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtumnmfyou.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtafjfchek.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gotoacloud.top/gtnmyrxbvh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtqsdwdvhy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangkeji.top/gtuskklbxw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gtztvxwrpw.html

================================================================================
来源：http://hz.shzxlz.cn/gtkjeznsfm.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtxchejncg.html

================================================================================
来源：http://hz.pengpengdd.cyou/gteimjrthp.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtkghrwmen.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gtglqvofpy.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtoarljhrm.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtoaljztrd.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtasvzzcfd.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtutywewdm.html

Go:   os.Args[1:]
来源：http://hz.nanxuanxn.top/gtwrheihid.html

Ruby: ARGV
来源：http://hz.hongshengwenyu.top/gthuxlymhn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtdwmwarpc.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gtfrcrwkzb.html

Py:   os.environ.get("HOME")
来源：http://hz.svipenyu.cn/gtafywtpjt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jyoumei.cn/gtkrhnmlck.html

JS:   process.env.HOME
来源：http://hz.yj20258.top/gtwdnbvkbm.html

TS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtjnkrfzlt.html

Java: System.getenv("HOME")
来源：http://hz.ppjwa.cn/gtxxxcwvpw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtrdvbgmqc.html

Ruby: ENV["HOME"]
来源：http://hz.snrcjt.cn/gtkhkrpxml.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gteceyasii.html

[M03] 执行外部命令
来源：http://hz.xinyue.icu/gtndxuvngr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.wangshuangyany.cn/gtwrlwbsoj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fzhhl.top/gtxzkuxcwm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtjlbwplhy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtxkrapubz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj202588.top/gtobvxtuxc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gotoacloud.top/gtzlelfghp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ppjwa.cn/gtxohatboc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hongshengwenyu.top/gtazblkaum.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gtktuydgai.html

Py:   os.getcwd()
来源：http://hz.ydjk.org.cn/gtklqehafr.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtleqsbybe.html

JS:   process.cwd()
来源：http://hz.jyoumei.cn/gtslctqayj.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtooynxgqh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shzxlz.cn/gtmrdlhzdj.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtfyccxtfe.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtyrliskyo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtrztegibo.html

[M05] 设置退出码
来源：http://hz.guannengcc.top/gtahznmzyn.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtfrwmjpxq.html

PHP:  exit(1);
来源：http://hz.ydzc1.top/gthqbasjte.html

JS:   process.exit(1)
来源：http://hz.sweek.top/gthtcmkkme.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gtwzztyjkn.html

Java: System.exit(1)
来源：http://hz.xinyue.icu/gtfktzpfls.html

Go:   os.Exit(1)
来源：http://hz.yongpay.top/gtytrvnvvv.html

Ruby: exit 1
来源：http://hz.xuanzx.com/gtezukhcjn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtrvdresog.html

[M06] 向标准错误输出
来源：http://hz.nanxuanxn.top/gtiihiidwz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.meibo888.top/gtvvxbjjwj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yueranfly.top/gtixthgkkj.html

JS:   console.error("err")
来源：http://hz.wangdashe.top/gtfvkeufzu.html

TS:   console.error("err")
来源：http://hz.daxiang520.top/gtlzjasyjx.html

Java: System.err.println("err")
来源：http://hz.snrcjt.cn/gthbnsxsbt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gtzzxcaljt.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtscywypfw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gzhubu.top/gtegsxsrlc.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtctjilgrl.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtczsmqxgo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gotoacloud.top/gtwzhbyzte.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtwnyibwms.html

TS:   require.main === module
来源：http://hz.cdnleiting.top/gtkonwieij.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gtgrqgfecv.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gtejmhrclu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shuidangran.top/gtbdyokzaf.html

C#:   static void Main(string[] args)
来源：http://hz.zhoulong.xyz/gtsisgdfuv.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtdnfsaxxn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtktpgxhki.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtagpueyod.html

JS:   process.platform;  process.version
来源：http://hz.gotoacloud.top/gtpjvwofsy.html

TS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtpsvxrgqp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gtzolauyxh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guannengcc.top/gtlbqrmggr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hammf.cn/gtsxiidtjh.html


<!-- 参考信息 -->