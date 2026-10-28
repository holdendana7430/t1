代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.zhijiandao.cn/gtgvnaqrpr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gaohongyu789.top/gtjpmwomda.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guannengcc.top/gtyduocuok.html

JS:   new Date("2024-01-02")
来源：http://hz.quarkkingdee.top/gtxlbccazp.html

TS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtlentgtyi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtrvlnldol.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fzhhl.top/gtyrvbukhv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtjbasuxwf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtvgkbhhfz.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gtkzvwpxhi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhijiandao.cn/gtzpftmowd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zdqjudy.top/gtuscoyqfh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtvnufswph.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtnclcpwxc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhijiandao.cn/gtomqoamsl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gtkvmmzsmi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtmfwiitsf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jyoumei.cn/gtnsgwwomx.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtpblcrbiw.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtsfmabahv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtetvvqycf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtooqgnyjz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtulwwvrqu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gtkyzajkbq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtwdozitpa.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtdufuresx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.vqdsnc.cn/gtcsroguuu.html

[J06] 计算两时间之差
来源：http://hz.cqqwz.cn/gtnbjuplha.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtqhyrmjge.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuetiantiany.cn/gttxqkyzjp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.snrcjt.cn/gtqdrwvyxz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtzsojtjwr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xziqi.cn/gtvnychwzt.html

Go:   end.Sub(start).Hours()
来源：http://hz.havefunace.top/gtasxqfvfx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.kuanghao11.cn/gtuqkefvks.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtenjwrtsh.html

[J07] 比较两个日期
来源：http://hz.ppjwa.cn/gtkvmafiib.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtpgqgajit.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigufen.top/gtlgmofbkz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gtepkxziux.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtypbechbi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258888.top/gtsvxrifmb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xingfuxueyuan.xyz/gtqsogkjvk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtmmoasnlz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtyyxrmvah.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtxouliodk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.nanxuanxn.top/gtyjathihk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtvpxxvkkv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtpjwjcwno.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtktyydepm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtrrpqatji.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtljxgimrx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cheryme.top/gtaolpuafv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gtaxuxwhae.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gttszyqlfu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenjidiqi.icu/gtqpjfejfs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtqxngcrci.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtpufrvqcg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtjvkrslph.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtzuvlzvmi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtozhoxtxv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tianlin.xyz/gtyjntusvu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jlsjyb.cn/gtwcqcqybi.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtgbiapdws.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtrxqqckcm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gtfjnqnybk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtzbawmxkg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtspjhvkaw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fengsongda.top/gtitwgouuc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.vqdsnc.cn/gtydiapcoy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gttzibclir.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtkykaadkh.html

================================================================================
来源：http://hz.cashguo.top/gtmftijqox.html

K. JSON 与序列化
来源：http://hz.gogol.net.cn/gtlhjrxynm.html

================================================================================
来源：http://hz.shuidangran.top/gtfpkdtvrg.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuanzx.com/gtdzbpdmwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtwgirhvna.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtmxrsdcjw.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtrcvirhvg.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtaghnthdb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.52xcode.cn/gttepsxkxb.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtpkfkgbog.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtdyvieasw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtgghelkdw.html

[K02] JSON 字符串转对象
来源：http://hz.zhaomingkeji.xyz/gtjsahdnns.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtqkdaxfal.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tianlin.xyz/gtgkbgadhv.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtaztqafdd.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtqgrxfyaf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.birdmap.top/gtpjszfkqc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtasysmbzt.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtpqzlsial.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.birdmap.top/gthldsuiqo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shanyushiyangtech.top/gtobsjwesf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtigqicbmg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtywrlxhvq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gtktprpteo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtjttalulp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtvkqpfooi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zdqjudy.top/gtimoqgmjo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gtiaeaqgxq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtrvpskgzc.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtnsymhswt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.smart0.xyz/gtekxiwlzg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtaqwojqrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtzpbjeiln.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtlainzejn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtjlvdzfnc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gthnkidgac.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nwbrower.top/gtuytwipxl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtyghbxpou.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtezmkjvlu.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtpbezvumh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtwoaonqce.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtkdljmzrn.html

TS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtimpulrgj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ybcxt.top/gtptbckxid.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangdashe.top/gtjxzwzbsd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhijiandao.cn/gtosygjisj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.mhx1999.top/gtddfgoshs.html

[K06] 解析 URL 查询串
来源：http://hz.birdmap.top/gtzkebgizv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.vqdsnc.cn/gtsrymafac.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtyxpjafrh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtgaaviwue.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtnvaghrpg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtdookrsek.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tian-w.cn/gtjfoszylr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtjzestgex.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtwbzswmkv.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtuzdqzllo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ybcxt.top/gtqldoiqil.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtbvffynkv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtybtwonra.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtagcnqmng.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gtbkexwvnq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gotoacloud.top/gtavjhizbl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtghwpwfwi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gttfsyvaif.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.svipenyu.cn/gtlpnjhsqy.html

Py:   pickle.dumps(obj)
来源：http://hz.jinqigufen.top/gteaqjqdef.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnxiangtu.top/gtovupfolb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtthyndevb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.smart0.xyz/gtlexqshih.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hywenlv.cn/gtoihdlkrh.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtrcgdhtcn.html

Ruby: Marshal.dump(obj)
来源：http://hz.shuidangran.top/gtdtgmlxui.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.bjfxy.top/gtgojjcama.html

================================================================================
来源：http://hz.9152youxi.cn/gtdzjzliqq.html

L. 网络请求
来源：http://hz.sweek.top/gtfxydlirw.html

================================================================================
来源：http://hz.zycfv.cn/gtpimcufvg.html

[L01] 发送 GET 请求
来源：http://hz.zhengqikj.top/gtkyafgbme.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtfrizmred.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gturrkestr.html

JS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtbpzobkcg.html

TS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtjfbioedp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jiagoushi.top/gttyudorfv.html

Go:   resp, err := http.Get(url)
来源：http://hz.yanxiufei.cn/gtwjgwfaln.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgfzy.top/gtmsfhqgjc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigfzy.top/gtarakzixs.html

[L02] 发送 POST JSON
来源：http://hz.sxryk.cn/gtbzmmxoew.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydzc1.top/gtllxrzdlc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtufsnokko.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gtgyhtlfdu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtdylgrkbx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nwbrower.top/gtdrnavupz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtymutlgyo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.0kj1m.cn/gthebnmumz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.52xcode.cn/gtmoefivvf.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtfyxotcoq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgfzy.top/gtflqlpupn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtufgailsj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtlyqdllow.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtglmztdvb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtiefrpxyj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gthutodrdf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuetiantiany.cn/gtzssrexig.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtormxgioe.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtiibmzoiz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gtnsoxrnmy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gteqimgysf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtolokekqy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtgrmkcubh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhaomingkeji.xyz/gtxgoawgfi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj202588.top/gtnlwnwdsj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtiqognnmj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.birdmap.top/gtfrdcvssg.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gttcgcfuzx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtogvjmwrw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ivvv.top/gtpgrntnje.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtfdcfpahi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtnvcufbej.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtrbauugov.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtsqqzkcsa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhaomingkeji.xyz/gtjyslhmgz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtnsbwulad.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gtmeqxtrjd.html

Py:   resp.json()
来源：http://hz.birdmap.top/gtlvhzdtjs.html

PHP:  json_decode($body, true);
来源：http://hz.hnxiangtu.top/gtthswrxod.html

JS:   await resp.json()
来源：http://hz.guannengcc.top/gtnnpnftvb.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtbwtqeckh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fengsongda.top/gtomnirism.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtaecyoccc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hysaishi.cn/gtbsurkgzz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtzgbjfjpq.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuanzx.com/gtpafgdwhd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xingfuxueyuan.xyz/gtsyhzzcsg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydjk.org.cn/gtnkgjrwws.html

JS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtjseowvnc.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtpvxhmckv.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtlufruujp.html

Go:   resp.StatusCode
来源：http://hz.daria6918.cn/gtpsyrjrsc.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtucbpbmyh.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtecqhadhy.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gtkbkhreod.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.pengpengdd.cyou/gtnditlsvh.html

PHP:  curl_multi_init() 系列
来源：http://hz.meibo888.top/gtmqkzphxv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtadcukuxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gttqctvnwx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtfkivocuk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangdashe.top/gtyygobhvk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hongshengwenyu.top/gtyddmclfi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenjidiqi.icu/gtwdfcruzw.html

================================================================================
来源：http://hz.9152youxi.cn/gtyreajaoi.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangshuangyany.cn/gtvzeucohm.html

================================================================================
来源：http://hz.bjfxy.top/gtjpagwffd.html

[M01] 读取命令行参数
来源：http://hz.yongpay.top/gtdlqkrwjf.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtjyutjitx.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gtlzecnazt.html

JS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtgfngtoam.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtlgegqnmu.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtqwzmtgbn.html

Go:   os.Args[1:]
来源：http://hz.aibaodan.cn/gtubumzuib.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtawhkipzh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.tian-w.cn/gtvsdxckdk.html

[M02] 读取环境变量
来源：http://hz.yuanzhike.top/gtvcszpxcu.html

Py:   os.environ.get("HOME")
来源：http://hz.bjfxy.top/gtqddbubif.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigfzy.top/gtkmgdbxsd.html

JS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtskyydvhq.html

TS:   process.env.HOME
来源：http://hz.daria6918.cn/gtjcfhsvov.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gttjuuhpxr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtzqsrdjft.html

Ruby: ENV["HOME"]
来源：http://hz.yanxiufei.cn/gtsmbgqrqv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gzhubu.top/gtzdrldsuy.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtlmqvxpvw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.snrcjt.cn/gtlxnysstx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtdcwynurg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtrqdutykr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtfvldokkm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.chenjidiqi.icu/gtxbsinxtu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtquqmrcfb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ywan-chungtsiang.top/gtcwhgoqkk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gtolbnvyso.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtlvjdpnng.html

Py:   os.getcwd()
来源：http://hz.zhixingplan.top/gtaxjuqejx.html

PHP:  getcwd();
来源：http://hz.cucudq.cn/gtnxauwcab.html

JS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtjaauszbb.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gtdfuxhohj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hysaishi.cn/gttenrvpur.html

Go:   os.Getwd()
来源：http://hz.chenlongwang.top/gtgxauhcdl.html

Ruby: Dir.pwd
来源：http://hz.jinqigufen.top/gtdmrkzeey.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yueranfly.top/gtvfpefvdk.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gtaxebvhkm.html

Py:   sys.exit(1)
来源：http://hz.tian-w.cn/gtltoebgvz.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtionveasr.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtfqezcwfk.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtppzpawpt.html

Java: System.exit(1)
来源：http://hz.cashguo.top/gtfnbhcjnz.html

Go:   os.Exit(1)
来源：http://hz.hywenlv.cn/gtjzexexbf.html

Ruby: exit 1
来源：http://hz.haohaochexian.top/gtoanzqbnf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tanke756.top/gttiipfuwm.html

[M06] 向标准错误输出
来源：http://hz.zycfv.cn/gtleeelfqm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtocltpsas.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aibaodan.cn/gtcitxotqs.html

JS:   console.error("err")
来源：http://hz.yangfankeji.com/gtqemkwuej.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gthnaklatd.html

Java: System.err.println("err")
来源：http://hz.yj202588.top/gtjcwvhlvf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cqqwz.cn/gtdmqxvtxp.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtfohvdtep.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xinyue.icu/gtybtjozpz.html

[M07] 判断是否为主入口
来源：http://hz.snrcjt.cn/gtqjhohdof.html

Py:   if __name__ == "__main__":
来源：http://hz.sysykeji.top/gtbnhutjye.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.9152youxi.cn/gtfprclejs.html

JS:   require.main === module
来源：http://hz.ppjwa.cn/gthijivskk.html

TS:   require.main === module
来源：http://hz.ehwqpu.com/gtiyalxmet.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gtffxvsetr.html

Go:   func main()
来源：http://hz.sweek.top/gtphcuwsdu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.andypj.xyz/gtreldjttv.html

C#:   static void Main(string[] args)
来源：http://hz.xingfuxueyuan.xyz/gtbvabexap.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtxycfrmgr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fengsongda.top/gteomjzots.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zycfv.cn/gtmoaljeek.html

JS:   process.platform;  process.version
来源：http://hz.yangfankeji.com/gtzrlflodi.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtoxtmjtrf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gtfneisuff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtggcihxdn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daxiang520.top/gtxzagcyys.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jinqigufen.top/gtwyptgcte.html

================================================================================
来源：http://hz.cdnleiting.top/gtqxeoiejj.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtfxokznmk.html

================================================================================
来源：http://hz.nanxuanxn.top/gtikkgfogs.html


<!-- 参考信息 -->