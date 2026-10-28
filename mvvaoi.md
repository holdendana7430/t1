代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxinkj.top/gtqeyblmga.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gtveikdtes.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtsxkirotr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtaxzcorwc.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gtfcgxtjnc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj202588.top/gtcvuulekh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258.top/gtgiifrkrz.html

JS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gtoopbshlu.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtuxdkkiur.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtwicsdxmx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj202588.top/gtnmowdgqz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.havefunace.top/gtdecnvqlc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zdqjudy.top/gtauqblkre.html

[J04] 时间戳与日期互转
来源：http://hz.wangshuangyany.cn/gtqljppbbl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gtyfzrfpzn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gtioslyocn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gttmhlrfkp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtxintjsmu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtrpoxuzlx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.snrcjt.cn/gtpmmjutwe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtdljdeylh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jianghu66.top/gtkqigxuvt.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtqkcqfgpp.html

Py:   now + timedelta(days=7)
来源：http://hz.zdqjudy.top/gthfviwrqj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hongshengwenyu.top/gtdftongnw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtqbgenqwl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtpqyhnckv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtifyneppf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jqgufenzy.top/gtsddchwae.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gtgbmvtajg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sufxvd.cn/gtigvohota.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtnzpnomyi.html

Py:   (end - start).total_seconds()
来源：http://hz.fengsongda.top/gtjueoonzm.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtcpywyvni.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtsrhedqze.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtaebpxmtn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtifnxnbru.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtymfiyatx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xylfe.cn/gtknlvvetz.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtexeywhco.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtmjsinqgn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtchcnidxc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigfzy.top/gtzznkkazy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtadvqhomn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtdqshgotl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtjolgxona.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.mhx1999.top/gtaroywziv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtujjkkizn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtxnjqpsog.html

[J08] 提取年月日与星期
来源：http://hz.316326.xyz/gtyiamwkeo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jianghu66.top/gtkitaqocy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gttnahljpi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuetiantiany.cn/gthgfjqrdb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj202588.top/gtmuntivwk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gtovyoftbl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtrnvhfbow.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtsndynxiz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtgqfamatu.html

[J09] 时区处理
来源：http://hz.xylfe.cn/gtqszdvwkt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.c1oappe.top/gtnqpbknyj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtxvfhfniu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtraazdebn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtvchxopau.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.c1oappe.top/gttogxqzdb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gttrbrgpns.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hysaishi.cn/gtnlvqjjct.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gthhdespgn.html

[J10] 取今天 / 本月第一天
来源：http://hz.bjfxy.top/gteymliudq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.quarkkingdee.top/gtsgntyagp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtqanuzzhc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtoltwomjj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gthcrmgdet.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtfockwmni.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gtypycevvt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgfzy.top/gthhblltaf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtvvienafv.html

================================================================================
来源：http://hz.yuxming.cn/gteiyyvqyg.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gteumzkvas.html

================================================================================
来源：http://hz.svipenyu.cn/gtwdfsftjt.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtpmtsgopr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gtnsjshrai.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtelontqcz.html

JS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtyqiayqdw.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtygapvwya.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hammf.cn/gtblycxtgd.html

Go:   json.Marshal(obj)
来源：http://hz.dianchejie.cn/gtzjfgfgst.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jiagoushi.top/gtytknubog.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtjjsuxjcj.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gtciicpyyd.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtpumedzbg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtbaeyybbr.html

JS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtxjmnynnr.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtzjaeltyi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtbjlilleu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtggqvrjmn.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtretxqhbu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cdnleiting.top/gtphztirvr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gthbqtxsaj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtdttgzlba.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtnztjbxpc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtoiexpvgt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhaomingkeji.xyz/gtmpabrnrk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jyoumei.cn/gtaxmorwfw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtdfqssjwt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gtlfvxehph.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangkeji.top/gthlfcpelm.html

[K04] 读取 JSON 文件
来源：http://hz.jqgufenzy.top/gtozeyfrwi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gthydetbxi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shuidangran.top/gtyaxvboxo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtlnwvgmps.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtnraqazce.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yonumen.top/gtfmnmttkt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xinyue.icu/gttbcectlx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cqqwz.cn/gtnkvspxff.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gtadfsdpmf.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtzoolwrzk.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtpbnmsday.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtlmfstzes.html

JS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtpqtwzcqv.html

TS:   structuredClone(obj)
来源：http://hz.smart0.xyz/gtbughumxn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gtjokshqzs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gtrqkfjvnk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yueranfly.top/gtyyividne.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtarpqzbur.html

[K06] 解析 URL 查询串
来源：http://hz.ivvv.top/gtymozdztg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtryhgnugj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gtumorbsap.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtlomhwigz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj202588.top/gtqliiqesz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtnmmxnzvm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtorkhgnwj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigfzy.top/gttqethhiu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtujypgfid.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtuguksbtn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtxnmgcygd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shuidangran.top/gtwukmbbzg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtqfpsalyc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtjswlmrny.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtndawfnun.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gteqawzokg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtgktblsov.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtgaxofnpa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtwszasavl.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtvntoqegn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtelzbgjax.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtragnmrky.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtpjtuafye.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtfnucrxdk.html

Go:   encoding/gob
来源：http://hz.tianlin.xyz/gtysrmifcq.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtwggslwie.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gteemahgbr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtcdytdkpu.html

L. 网络请求
来源：http://hz.zhiwuduotai.top/gttrkvngxj.html

================================================================================
来源：http://hz.hysaishi.cn/gtrebjewdn.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gttclhxewr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dianchejie.cn/gtlhhgmijn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shzxlz.cn/gtqvgfasuy.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtjhbcpmdb.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtllhkigox.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenzaomai.com/gtfzusoxtw.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtoqogpfcm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangkeji.top/gtkeriduqm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtznkvesmq.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtuiwkdhfj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nwbrower.top/gtptxxakxt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtapmhgqmr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtggvqdnap.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtjldumhwm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnxiangtu.top/gtehzvbypb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtvkjmyxur.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtlfyevurq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tianlin.xyz/gtdspocnvd.html

[L03] 设置自定义请求头
来源：http://hz.ybcxt.top/gthucpkwnq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtyrjrqmdr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtgjmcbxlz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtblvuduws.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtqzbztycr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.haohaochexian.top/gttizdtyrz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtxymftany.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhijiandao.cn/gtfarimgdg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gtmhbmochu.html

[L04] 设置超时
来源：http://hz.zhijiandao.cn/gtwfcqucnt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cucudq.cn/gtoripigfj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hysaishi.cn/gtiehgfhea.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtfeeqfmpm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtaqtupyuk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtdytwvwzx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtbivzqtcc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yvedp.cn/gtbwroopsr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xziqi.cn/gtdirzhmae.html

[L05] 上传文件（multipart）
来源：http://hz.fengsongda.top/gtucpmgghr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jyoumei.cn/gtwnipryyy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtpouybjpe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtsgjtexfz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtayjydyln.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.redwolf501.top/gtdmctzrdg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtjuzdjouy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xinyue.icu/gtkmpgiiph.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.redwolf501.top/gtbedgtusx.html

[L06] 解析响应为 JSON
来源：http://hz.yvedp.cn/gtlllzrsaz.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gtkliolwym.html

PHP:  json_decode($body, true);
来源：http://hz.yueranfly.top/gtltyyxdgb.html

JS:   await resp.json()
来源：http://hz.yuxming.cn/gtjcwprzij.html

TS:   await resp.json()
来源：http://hz.nanxinkj.top/gtsidsnurn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtdandnuil.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtezpyyqzi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtasrksszc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigfzy.top/gtotkrmnko.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtcqmukhla.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtuopsoaev.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gteorzpkkd.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtyhvmcptz.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtevpmpqba.html

Java: resp.statusCode()
来源：http://hz.havefunace.top/gtfdzwqgjq.html

Go:   resp.StatusCode
来源：http://hz.sxryk.cn/gtnmcdgmok.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtiwtufdjr.html

C#:   (int)resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtrrkwixky.html

[L08] 并发请求多个地址
来源：http://hz.cqqwz.cn/gtgkfuyqtn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhaomingkeji.xyz/gtuxqadhcz.html

PHP:  curl_multi_init() 系列
来源：http://hz.yangfankeji.com/gtqgxfyeez.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtpnwqatyz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sweek.top/gtfxwkvdwx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.iojbl.cn/gtpbtzjvko.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.bjfxy.top/gtxjbileqe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj202588.top/gtijdrpeyw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gtrogvbnkc.html

================================================================================
来源：http://hz.tanke756.top/gttlyxtzff.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gtvnctgbwq.html

================================================================================
来源：http://hz.zdqjudy.top/gthtwprrfg.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtcauaywxz.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtcaozyube.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtbtlstngu.html

JS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtvmvzzbtv.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtwluvgwsy.html

Java: args 数组（main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtbjqrzegk.html

Go:   os.Args[1:]
来源：http://hz.52xcode.cn/gtdwgojori.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtlpzxnqci.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gtxiibiqon.html

[M02] 读取环境变量
来源：http://hz.guannengcc.top/gtfzxmxegz.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigfzy.top/gtowmirika.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hongshengwenyu.top/gtekgswjte.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtehrzilxi.html

TS:   process.env.HOME
来源：http://hz.yuanzhike.top/gteotaubzh.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtapymlluv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtvzhvasfz.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtqugqexeu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hfpthk.cn/gtxyipuygc.html

[M03] 执行外部命令
来源：http://hz.mhx1999.top/gtffcclhws.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtosxectgt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.smart0.xyz/gtpqdbjvhg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.0kj1m.cn/gtzecpxwvw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtvyqznpol.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnqzz.top/gtagkpfxby.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxinkj.top/gtkgbcnhaz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtgekmynzx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtzybdgsdl.html

[M04] 获取当前工作目录
来源：http://hz.shzxlz.cn/gtahbvauwf.html

Py:   os.getcwd()
来源：http://hz.shuidangran.top/gtezqhfjnw.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gtqstxhjmw.html

JS:   process.cwd()
来源：http://hz.zdqjudy.top/gtxaajsprp.html

TS:   process.cwd()
来源：http://hz.hnqzz.top/gtpwbgypro.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guowangkeji.top/gtwybshtcw.html

Go:   os.Getwd()
来源：http://hz.yj20258888.top/gtyfuaxknf.html

Ruby: Dir.pwd
来源：http://hz.ivvv.top/gttzdywine.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenzaomai.com/gttlwmvhbi.html

[M05] 设置退出码
来源：http://hz.shuidangran.top/gtohfqmfcd.html

Py:   sys.exit(1)
来源：http://hz.c1oappe.top/gttbldqktz.html

PHP:  exit(1);
来源：http://hz.daria6918.cn/gtupzfforo.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtpgsjwnht.html

TS:   process.exit(1)
来源：http://hz.gzhubu.top/gtyukmlads.html

Java: System.exit(1)
来源：http://hz.fzhhl.top/gtotjhqqyq.html

Go:   os.Exit(1)
来源：http://hz.gaohongyu789.top/gtcglrmnbr.html

Ruby: exit 1
来源：http://hz.cheryme.top/gtskenxnfe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydzc1.top/gtmcyfpfei.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gttiiqwddf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dianchejie.cn/gthqtedpzq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigufen.top/gthdvcbsas.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtnqquwrva.html

TS:   console.error("err")
来源：http://hz.shanyushiyangtech.top/gtoplzzmzw.html

Java: System.err.println("err")
来源：http://hz.c1oappe.top/gtwgmtjihf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.0kj1m.cn/gtlydkxcvi.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtcljgggup.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jianghu66.top/gtlumbuctx.html

[M07] 判断是否为主入口
来源：http://hz.redwolf501.top/gtwaitydxr.html

Py:   if __name__ == "__main__":
来源：http://hz.zhijiandao.cn/gtbcyhaaeu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.meibo888.top/gtiwyixieh.html

JS:   require.main === module
来源：http://hz.nanxuanxn.top/gtlifwhcmn.html

TS:   require.main === module
来源：http://hz.hywenlv.cn/gtjiuwxnvm.html

Java: public static void main(String[] args)
来源：http://hz.aizwys.cn/gteabptmaf.html

Go:   func main()
来源：http://hz.ehwqpu.com/gtzohxksbg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.feifeiyinyue.top/gttnzcnymf.html

C#:   static void Main(string[] args)
来源：http://hz.dashuyun.cn/gtjdjpjgxv.html

[M08] 获取系统与运行时信息
来源：http://hz.yonumen.top/gtqgalgkus.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cheryme.top/gtymgpkvzz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.haohaochexian.top/gtytwzxrdj.html

JS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtiwmfhtai.html

TS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gtuscvozlf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.gzhubu.top/gtsgdqyhfm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xylfe.cn/gtddlfslgm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.c1oappe.top/gtfbbpuptf.html


<!-- 参考信息 -->