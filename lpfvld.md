代发 wailian999

Go:   time.Now()
来源：http://hz.yj202588.top/gtojjqyqhx.html

Ruby: Time.now
来源：http://hz.shuidangran.top/gtwmrhjcaa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtxhmhzrds.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtbecmqcmr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtamlohjvx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gttlmfiyeg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xinyue.icu/gtijeuvvgx.html

TS:   d.toISOString()
来源：http://hz.cdnleiting.top/gtxhcqnzsj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.andypj.xyz/gtuqusavqa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ydzc1.top/gtsklfggkk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gthzfjnbzu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jyoumei.cn/gtiotqeric.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtemoybuyz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtccktnyer.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xinyue.icu/gtllozcggq.html

JS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtzwzhfmdr.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtvflsvsjh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtooqkertr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtqvwebhit.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtqmvkiykl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtwqtpxrkc.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtkdzrvxln.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tanke756.top/gtrzbuunnu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtkmgqmvxn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xinyue.icu/gtuubkldlr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daria6918.cn/gtnbwmasly.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtatmvmwzu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gthvoeflfs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtwqrovana.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtffhrzvsa.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gtpzxxbiin.html

Py:   now + timedelta(days=7)
来源：http://hz.smart0.xyz/gtsuhoptjn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zycfv.cn/gtembmqebq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtbwatdqwh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtihxtjmks.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ppjwa.cn/gtezrqdbgn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dianchejie.cn/gttnwfxkpc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258.top/gttftpaeng.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtfvlppaal.html

[J06] 计算两时间之差
来源：http://hz.zhixingplan.top/gtifpgcwjs.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtrmsoyeil.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuanzx.com/gtdnfgoykt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtundlyezn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gotoacloud.top/gtwjshlyyb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtnupkvxgn.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtxnmsrsvw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtrzsvlkgz.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtacmifjdq.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtdsokwvke.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtepepscbc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtyovpshck.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtgbfdexee.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtmkprowys.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtohpstyer.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhiwuduotai.top/gtuyfmagqj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtcgbxccfi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtpabinegr.html

[J08] 提取年月日与星期
来源：http://hz.cqqwz.cn/gtgzwjuesd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtsgamjwgm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtnrqqdvis.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtkavveufb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tanke756.top/gtfnnumxnb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtjkodsbjb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangshuangyany.cn/gteojqbylj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangkeji.top/gtmairvkfh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtfnsqiuxs.html

[J09] 时区处理
来源：http://hz.cqqwz.cn/gtdibxfouz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtsjdaybvf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jlsjyb.cn/gtzedudrdv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtzngfciym.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtkfjftctc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258.top/gtikuqsduy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ppjwa.cn/gtrvafllfq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sweek.top/gtwmiludwx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtnynylegq.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtjtjeecfd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guowangkeji.top/gtmhlymyzy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtuquabyap.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gttwcvrsyg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gtiblqfbqm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.iojbl.cn/gtmijvsxiy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aibaodan.cn/gtavnniryg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtwyzwpczf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.quarkkingdee.top/gtnvdjvxuq.html

================================================================================
来源：http://hz.zycfv.cn/gtnmiqvewx.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtmixenwnx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtrlhmjhph.html

[K01] 对象转 JSON 字符串
来源：http://hz.jianghu66.top/gtjsowzpst.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtqbnowidw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtwkzehbrb.html

JS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gttzqqdkei.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtduxvslgk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtocxciobv.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtkiiydhyg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtxkacnuoc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.9152youxi.cn/gtgmpqdgty.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtrdaprjts.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtrivuxpnh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtrchwchlt.html

JS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtbbogdluh.html

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtksijubaz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtwcbtpevf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtvtiztden.html

Ruby: JSON.parse(s)
来源：http://hz.sweek.top/gtevpbyrrx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gtfivaabtq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtjodcbpaj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtqhtgptmt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtuxplmrto.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtrkwdmffa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtpkjbspfx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.haohaochexian.top/gtpzlxlnjp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj202588.top/gtuhbnsntj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnxiangtu.top/gthfzwrqzc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtimamcjgy.html

[K04] 读取 JSON 文件
来源：http://hz.jinghuilouyu.cn/gtjeoezsdn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dianchejie.cn/gtqyrjcmds.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtraggazfm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtdbekawsv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtseyndehx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ybcxt.top/gtulrnljbb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtszssycbg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.havefunace.top/gtyysqfekl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cdnleiting.top/gtzmahfhwq.html

[K05] 深拷贝对象
来源：http://hz.xinyue.icu/gtxkhgpezs.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gtnzmcbbol.html

PHP:  unserialize(serialize($obj));
来源：http://hz.redwolf501.top/gtsytqmkwv.html

JS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtfssqxrta.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtomlxivmo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shuidangran.top/gtqjaykgqs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.316326.xyz/gteiwbngnm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtytgoilna.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtauiydpln.html

[K06] 解析 URL 查询串
来源：http://hz.aizwys.cn/gtrkrlnenn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtzkybwhcj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ivvv.top/gtumdskhfx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gteaabylvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtixnnzhom.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtcyautzry.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtdyemjzzr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hysaishi.cn/gtkbzqmnbd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.316326.xyz/gtfwmcqlfa.html

[K07] 进制转换
来源：http://hz.aibaodan.cn/gtcqbajxua.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gogol.net.cn/gtrvtgojpq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtwphfewik.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtnnitakeu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtvuynoqvb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtilpxakcw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinyuanbaomall.cn/gtqcwiioxk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtjkhvjhtx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtccxwvomx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtaakpqxhu.html

Py:   pickle.dumps(obj)
来源：http://hz.cucudq.cn/gtsraryxjb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pycfn.com/gtcyidpsws.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtsfnzsyyh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtcdqmazip.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhaomingkeji.xyz/gtipvvbmpw.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtpadasvki.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtmbhraeva.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtbnhviall.html

================================================================================
来源：http://hz.yangfankeji.com/gtahfvqjcq.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtebiylkzf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkcpblrhs.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gttqvhxbbr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtzizzqwlj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gtbieedpiv.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtbriwzfja.html

TS:   await fetch(url)
来源：http://hz.guannengcc.top/gtuadyzilo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtttvwthhf.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtygeiuzap.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtzmkinxcg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jiagoushi.top/gtwkfxtwqx.html

[L02] 发送 POST JSON
来源：http://hz.hysaishi.cn/gtlzprksqt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gtorzfvbir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hammf.cn/gtmvmolhxg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gttihomiig.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtgjzofilr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yvedp.cn/gtwchhbtvb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fengsongda.top/gtqwdjmnrm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtvyzoovvx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gttzsrobiw.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gthpdkxhvg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shuidangran.top/gtoljlhxhr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sysykeji.top/gtfzjiphtk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtnnlfgnpp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gthfbcberl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jinyuanbaomall.cn/gtnswlarkx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtjbsrrcoy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jianghu66.top/gtwifskecz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.meibo888.top/gtritonkqd.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gtfrgqikgj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtyhvxodoc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtvyjibnum.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtatbibukh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.iojbl.cn/gtchqhvldz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.snrcjt.cn/gtmsycpgro.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinghuilouyu.cn/gtqjmlsvsq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtvdmitbhw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258.top/gtfhfctasl.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gtsevofeea.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guowangkeji.top/gtxkyavppj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shangyingyoupin.top/gtnygveqkr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtotklpdga.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtpdbkzyjr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtdblvrqbh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gtjxhpooti.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtghdzslvt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtdnbfvhqd.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtbeqnccgq.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gtsthypois.html

PHP:  json_decode($body, true);
来源：http://hz.aibaodan.cn/gtlmdmjdsm.html

JS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtmreiljrk.html

TS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtzpupcsyh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.c1oappe.top/gtnclqwjns.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhongyouzk.top/gtclfwnhsg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fzhhl.top/gtemtyaady.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtbejpxiuq.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtmnjkigzb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtznrbeush.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gthwetbjrc.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtgxzclgas.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtphrhkizo.html

Java: resp.statusCode()
来源：http://hz.316326.xyz/gtambutldp.html

Go:   resp.StatusCode
来源：http://hz.sxryk.cn/gtrsbdpniu.html

Ruby: resp.code.to_i
来源：http://hz.tanke756.top/gtpeijlzxm.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gtfjywfcqh.html

[L08] 并发请求多个地址
来源：http://hz.yvedp.cn/gtoyxhaaqi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinyuanbaomall.cn/gtesifkuun.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtohzypvac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtxyuqzrcl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtvworyafq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenzaomai.com/gtynyauzyd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydzc1.top/gthjxawtdk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ehwqpu.com/gtbiblyplc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtbrgfxbny.html

================================================================================
来源：http://hz.jyoumei.cn/gtcvprtncl.html

M. 命令行 / 进程 / 环境
来源：http://hz.yj20258888.top/gtdooqkkkn.html

================================================================================
来源：http://hz.xziqi.cn/gttaccudia.html

[M01] 读取命令行参数
来源：http://hz.nanxuanxn.top/gtdoivpvch.html

Py:   sys.argv[1:]
来源：http://hz.yj20258.top/gtiryczyec.html

PHP:  $argv;  $argc;
来源：http://hz.yongpay.top/gtihcghsfo.html

JS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtsefyjxkz.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtbzamvcuh.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtedhqqhzw.html

Go:   os.Args[1:]
来源：http://hz.zhixingplan.top/gtajnrehqr.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtxfooeujs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.meibo888.top/gtccdniwfe.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtojwalqoq.html

Py:   os.environ.get("HOME")
来源：http://hz.smart0.xyz/gtklanodzi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtppxylfxp.html

JS:   process.env.HOME
来源：http://hz.gzhubu.top/gtvuysokzf.html

TS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtajfbsqys.html

Java: System.getenv("HOME")
来源：http://hz.sysykeji.top/gtbxudnvjc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxinkj.top/gtdepxcapi.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtpzieowla.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sxryk.cn/gtltizdkuv.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gthyqgqdpo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tanke756.top/gtalnzwoll.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jqgfzy.top/gtyuducfky.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtucgotngu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtsfnumqwb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gtqmclbfes.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.aizwys.cn/gtqurfusud.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtchrqdnde.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenlongwang.top/gttrpzcbmy.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtsnglnrfx.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtwaetairr.html

PHP:  getcwd();
来源：http://hz.zhiwuduotai.top/gtsekkgjnr.html

JS:   process.cwd()
来源：http://hz.yuxming.cn/gtcqhyvwok.html

TS:   process.cwd()
来源：http://hz.yuxming.cn/gtcpvkwqvv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhixingplan.top/gtlkedygsl.html

Go:   os.Getwd()
来源：http://hz.jqgfzy.top/gtydrqutek.html

Ruby: Dir.pwd
来源：http://hz.tian-w.cn/gtnyjznznj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guowangkeji.top/gtmghrylco.html

[M05] 设置退出码
来源：http://hz.yj202588.top/gtmocembtm.html

Py:   sys.exit(1)
来源：http://hz.pycfn.com/gtzbphwjru.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gtvbwbmmvg.html

JS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtevmaizix.html

TS:   process.exit(1)
来源：http://hz.bjfxy.top/gtzobprzqz.html

Java: System.exit(1)
来源：http://hz.52xcode.cn/gtuzfsyngc.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtdbryztlk.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtjchkwjhd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sufxvd.cn/gttcyqazuv.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtoivyweck.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxuanxn.top/gtaucrdicx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cqqwz.cn/gtarjojquh.html

JS:   console.error("err")
来源：http://hz.yj20258.top/gtdgoqwzdc.html

TS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtprvlfqvm.html

Java: System.err.println("err")
来源：http://hz.jlsjyb.cn/gtqhfhbuhc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.fzhhl.top/gtpbxrdvnj.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtujatoyew.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydjk.org.cn/gtvudbcbbf.html

[M07] 判断是否为主入口
来源：http://hz.yj202588.top/gtqasgmlsj.html

Py:   if __name__ == "__main__":
来源：http://hz.cheryme.top/gtbafzneng.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgfzy.top/gtyyvfxmky.html

JS:   require.main === module
来源：http://hz.52xcode.cn/gteoiepgka.html

TS:   require.main === module
来源：http://hz.gaohongyu789.top/gthyhseqak.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtveizdbzo.html

Go:   func main()
来源：http://hz.yongpay.top/gtqquwxvcx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtyvrskpyw.html

C#:   static void Main(string[] args)
来源：http://hz.chenlongwang.top/gtkxqdixur.html


<!-- 参考信息 -->