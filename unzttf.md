代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtvupyuuyt.html

JS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtxyoxyipn.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtdjyuszqs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtuxvpprcy.html

Go:   time.Now()
来源：http://hz.sufxvd.cn/gtzfunzhcz.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtsyqngyyd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtamckxsjk.html

[J02] 格式化输出
来源：http://hz.0kj1m.cn/gtnyldsaia.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtdfyooiyt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydjk.org.cn/gtwpzglyww.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtzsfrluxb.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gthdqysqmo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.feifeiyinyue.top/gtpgxbmxtw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ivvv.top/gtiswahunx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtmawkkrls.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxinkj.top/gtztfacldv.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtidyslbvy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gteliqutvx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtmodeboxv.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gttftyxizu.html

TS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtvfrkpicu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtihcvaqxh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtjduzvpyu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.meibo888.top/gtyplwkapn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.andypj.xyz/gtoctykrqk.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtuutyfzkt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtgcwpgwdr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ppjwa.cn/gteumgxobi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtjzhkbsvp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtxlypcjta.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.quarkkingdee.top/gtrrvrleex.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtbylizixh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtzjkeykrc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ehwqpu.com/gthqgehqap.html

[J05] 时间加减（加 7 天）
来源：http://hz.havefunace.top/gtellvhqeb.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtlgvutvid.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fengsongda.top/gtvaavyfbj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtitgujbpj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtukowlynl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nwbrower.top/gtctnzvpnf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtgcexltby.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtxnbvyhpw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtqarstihx.html

[J06] 计算两时间之差
来源：http://hz.yongpay.top/gtztvsynlh.html

Py:   (end - start).total_seconds()
来源：http://hz.andypj.xyz/gtjpbnrhrn.html

PHP:  $end->diff($start)->days;
来源：http://hz.sysykeji.top/gtmhguxcts.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtqdurgxti.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.smart0.xyz/gtvtaelxnr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangshuangyany.cn/gtfzwnvlsd.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gteeoalldu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtybsllexb.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtqhpnmlmj.html

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtesfxnwfv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtxvnqrytx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shzxlz.cn/gtvjsyflnx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gttrsgezbe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtgxhwoggx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtmwdrpkwt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtqbkxvbrc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtvclfadpn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtnywinycn.html

[J08] 提取年月日与星期
来源：http://hz.shzxlz.cn/gtuqcqvozp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhixingplan.top/gtdndrsqrc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtwwryoywg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ybcxt.top/gtjgibcjkv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtgwolozol.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtsicmjrko.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.snrcjt.cn/gtmlibntyf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtazgubszx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtgxqvyprz.html

[J09] 时区处理
来源：http://hz.yonumen.top/gtvpenqiak.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guannengcc.top/gtdukyaodj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtyfsvstfo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtyqhyeanr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtkrghgxox.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gthrmeacxz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtilpanfnu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtipigqapp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenlongwang.top/gtbdrfohdx.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtoenawajj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aibaodan.cn/gtudhzlfec.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuanzhike.top/gttojfntmk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gtrlveuajn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangshuangyany.cn/gtnwherzhc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.havefunace.top/gtfxrmzxzn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.daria6918.cn/gturnbtuki.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tian-w.cn/gtefklwgaa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgufenzy.top/gtyisbrlbj.html

================================================================================
来源：http://hz.yj20258888.top/gtlnvpjihs.html

K. JSON 与序列化
来源：http://hz.yanxiufei.cn/gtrritqklw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtuhaoredb.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtuvrzzeuk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.meibo888.top/gtqjdqhxdy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtinjldzcg.html

JS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtfpabnpjf.html

TS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtlbggfolp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gtkkonmpjl.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtnobnjmny.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtqbeqwaja.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cheryme.top/gtxxnoqkap.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtzawsexhk.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gthnsqnefz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nwbrower.top/gtycwxukti.html

JS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtwvvwhgpa.html

TS:   JSON.parse(s)
来源：http://hz.yj20258.top/gteskxfjaz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gtoltlttqg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtuhicbyob.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtodxcjyjj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenjidiqi.icu/gtyfkshkvf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtapbwwctj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtlhzijbar.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtewhqyxzf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtvxjuxmlm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtpeslttpc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yueranfly.top/gtegvajypv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtuhbbmgup.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ppjwa.cn/gtvbhcomsf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yvedp.cn/gtdthibyqq.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangtech.top/gttktnxgtk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gtqyyitmfz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtjlzkkkga.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtyyckacly.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtleqibggr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhengqikj.top/gttbcuxxco.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtbkqpfllp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtbsxoavpq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtwwyuimxi.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gtglculsfx.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhengqikj.top/gtwcvlbywb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aibaodan.cn/gthkaqmyxx.html

JS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtzrujlugs.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtufzrkmor.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxinkj.top/gtqxxeskhr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cashguo.top/gtichxcfvi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gthtknkzgl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtpkihqeei.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtqewqgvtb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtrgnwkqcb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgufenzy.top/gtuodnbflk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtztjcdhyk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtejfjzaxj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pengpengdd.cyou/gtjoogkavi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtpabiqsar.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtwbqyhend.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtyeikbmtk.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtmfgfpsqh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.aizwys.cn/gtcbfmapcx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtpoafmftb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtfqlqgjyd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtrzuorhsz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtlhvhwdmf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.smart0.xyz/gtstjdmcov.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.bjfxy.top/gtkfimbcar.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtzirjlhwz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cheryme.top/gtlifsmynk.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtuwwwlbxv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gttlzghwnu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtjqslqkad.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtvajafchs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dianchejie.cn/gtlhwshxlh.html

Go:   encoding/gob
来源：http://hz.xuetiantiany.cn/gtxvzwznhr.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtfdvfrmgu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtitazrksh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtuaitzwie.html

L. 网络请求
来源：http://hz.gzhubu.top/gtrubvkpgt.html

================================================================================
来源：http://hz.hfpthk.cn/gtuglqovto.html

[L01] 发送 GET 请求
来源：http://hz.jlsjyb.cn/gtskfegllr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guowangkeji.top/gtuvzfzstt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xingfuxueyuan.xyz/gtamydnpbr.html

JS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtprtjvksp.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtbdbsgdah.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guowangkeji.top/gtjepxzykm.html

Go:   resp, err := http.Get(url)
来源：http://hz.yonumen.top/gtrjiryqrs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gtruflikjw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtbbnntntt.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtebbiewcs.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gthfkontrm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtfmmlzaml.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtmjlzkojn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtfezmftoj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.andypj.xyz/gtstmucqcu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuxming.cn/gtnsavgpfw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pycfn.com/gthojenige.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgfzy.top/gtlmysptly.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtidakykgf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtpmoutomh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhixingplan.top/gtukksnhtk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtunljfuum.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtimhschtn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtuqtkhduv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtgefdcyfe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gtrerjcjjq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gthfebxagh.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtoumxyjfu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daxiang520.top/gtyfjqpaaq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtjyvgcdka.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtwtyubfmr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pengpengdd.cyou/gtijjscdzw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gthjhfhoxl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daxiang520.top/gtulfceiiz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.0kj1m.cn/gtxpbkluoi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jyoumei.cn/gtlcogdjuj.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtuyozdapc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtvkhrprsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jianghu66.top/gtbhayhgfs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtpeiokluy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtzbgrwvip.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sweek.top/gtultxbixg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtidcvrmzf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtubrhogse.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtbmvcwciz.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtrrahpdew.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtjqzdgkbv.html

PHP:  json_decode($body, true);
来源：http://hz.yuxming.cn/gtbnzxoixc.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtvcrghkak.html

TS:   await resp.json()
来源：http://hz.zycfv.cn/gtgsidikyb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sysykeji.top/gtlfzjglev.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinghuilouyu.cn/gtzihtcbry.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hfpthk.cn/gtbuvfnzaq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hongshengwenyu.top/gtuueeiipb.html

[L07] 处理 HTTP 状态码
来源：http://hz.mhx1999.top/gthdupuiwp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cashguo.top/gtvahpenlq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtmentrhcs.html

JS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gttihhrcdj.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtzcvhkkry.html

Java: resp.statusCode()
来源：http://hz.svipenyu.cn/gtdaucgwff.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtvcpqxqbm.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtjbcaiino.html

C#:   (int)resp.StatusCode
来源：http://hz.cdnleiting.top/gtedncsbfs.html

[L08] 并发请求多个地址
来源：http://hz.yanxiufei.cn/gtszgrtqnw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.nanxuanxn.top/gtfhiwfcqt.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtukeycbci.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtkydwshid.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtsfqpowyl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.fzhhl.top/gtfmkfwzsr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.dianchejie.cn/gtlbacbeun.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gtwnzyrocq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtxgknqvye.html

================================================================================
来源：http://hz.zhoulong.xyz/gtycpjgyjc.html

M. 命令行 / 进程 / 环境
来源：http://hz.gotoacloud.top/gthaltqies.html

================================================================================
来源：http://hz.jinqigufen.top/gtjrsimhuy.html

[M01] 读取命令行参数
来源：http://hz.sysykeji.top/gtxysoaqif.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangtech.top/gtkicpqszd.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtrbrsdlzc.html

JS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtvyfghamn.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtruqlxvjc.html

Java: args 数组（main 方法参数）
来源：http://hz.gaohongyu789.top/gtbvmzvsrs.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtbsqssypj.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gtwzthgvmf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtgjhhamug.html

[M02] 读取环境变量
来源：http://hz.tianlin.xyz/gtjbyhacmy.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtgiictybt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtbyjxqwxg.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtuucotkps.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtjdceqqxi.html

Java: System.getenv("HOME")
来源：http://hz.yj20258888.top/gtdzvlripe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gtbyhvpvmu.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtislodrnk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtwuyrkobm.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtdcrxaonq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtzvdzqpno.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtbdqhggrh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sysykeji.top/gtjdmqlwte.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtmvtgpybz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sufxvd.cn/gtlwlhbnew.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gtobxbpjus.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtgecbylgm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guannengcc.top/gtcwdwykcs.html

[M04] 获取当前工作目录
来源：http://hz.fzhhl.top/gtrracsygd.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangkeji.top/gtdfysepsi.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gtxxmotoon.html

JS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gthfnodcdv.html

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtlaycncxt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtizeypiun.html

Go:   os.Getwd()
来源：http://hz.haohaochexian.top/gtxjaxztbj.html

Ruby: Dir.pwd
来源：http://hz.andypj.xyz/gtllpmlfej.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuxming.cn/gtwhppvqlb.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gtmwnanamf.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtqzrtptkb.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtltwmhbpz.html

JS:   process.exit(1)
来源：http://hz.316326.xyz/gtxaoxukhv.html

TS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtpsgvqtdt.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtfhbethso.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gtrrhepdps.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtkpaicnfa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtjeiopevf.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtsmsabhiz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtpttqouwv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gthdtznvam.html

JS:   console.error("err")
来源：http://hz.fzhhl.top/gtcoprmczt.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gttmastlkn.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangkeji.top/gtzvxbbvvq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zdqjudy.top/gttabepemh.html

Ruby: warn "err"
来源：http://hz.jinqigfzy.top/gtuabicywg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yvedp.cn/gtaqljbfay.html

[M07] 判断是否为主入口
来源：http://hz.cqqwz.cn/gtqsbwukxa.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtfyastsrf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtnmvdzthi.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtihwxuyfm.html

TS:   require.main === module
来源：http://hz.hammf.cn/gtqdygocbi.html


<!-- 参考信息 -->