代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtvxebzvlb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gthjywswjp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtifkbhylj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhengqikj.top/gtwdczcubz.html

[J03] 字符串解析为日期
来源：http://hz.pengpengdd.cyou/gtkjymkcbp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xylfe.cn/gtqdzejtin.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydzc1.top/gtkqvqpiof.html

JS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtopbomgqr.html

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtosudiaoq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtdrernizi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.pengpengdd.cyou/gtuopjsgra.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtxdtafjvd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dianchejie.cn/gthvkrpsgi.html

[J04] 时间戳与日期互转
来源：http://hz.andypj.xyz/gtdwtrnzjr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.iojbl.cn/gtvbtmsaiq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtmbhpbtbq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhoulong.xyz/gthudcdvyj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guannengcc.top/gtowzggyfg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daxiang520.top/gtzwwrfkgu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuxming.cn/gtckmhqbaf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xinyue.icu/gtrcxahhtl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinghuilouyu.cn/gtghgkydyw.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtyuyguywk.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gtnbdgjkxl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.andypj.xyz/gtborbyaci.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtpomynqkk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtyjvrwajy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnqzz.top/gtqmjfogzm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yanxiufei.cn/gtytznfjoc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtvoqkyvfc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cashguo.top/gththzvmfi.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtzknddrmo.html

Py:   (end - start).total_seconds()
来源：http://hz.feifeiyinyue.top/gtkpebmkrr.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gtsvnupaeg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gotoacloud.top/gtfejrlbiq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtvrfdnbxp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.feifeiyinyue.top/gtwwgxutsl.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuanzx.com/gtxihzobyy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtewbzvrax.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtwmzgxhvh.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gtkjlplyzh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtrqprzawf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ppjwa.cn/gtkwkqpgxy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtoknkcmcq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gthlozphyk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtcrksvgeu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gtlzzyiwnb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtrnovgmli.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtryonxntq.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtlowmbmxk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xziqi.cn/gtxczcrghk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daxiang520.top/gtibvddwes.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gteexczwul.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zdqjudy.top/gtrbijcjfz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gtifydamin.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yanxiufei.cn/gtrfqwgshv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gtgdypayxl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtvtblljzf.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtwptvavjk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daria6918.cn/gtqyfvmyoy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtlpdlyffn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtjjfqqgve.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtbghgrpfe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtibdqaylm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cqqwz.cn/gtkpabjwtx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guowangkeji.top/gtbuqykihr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gtjhgdffnw.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxuanxn.top/gtjnlmgzut.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtsdtfbuow.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.svipenyu.cn/gtbghuxsdn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtxxdphzge.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtqhxuuozl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtpfoevjdz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtqgmlthgr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fengsongda.top/gtborhjutj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.316326.xyz/gtwfmxxqfm.html

================================================================================
来源：http://hz.0kj1m.cn/gtfvxoidhm.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtbnowgdwj.html

================================================================================
来源：http://hz.zdqjudy.top/gtmjkjfnvd.html

[K01] 对象转 JSON 字符串
来源：http://hz.nanxuanxn.top/gtmyfohuxl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtobiouvsb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtozbonfyb.html

JS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtokgdpjob.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtkcsiosbb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtrubmnpnr.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gteixhrrkj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtgoodnblf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtijvuetpg.html

[K02] JSON 字符串转对象
来源：http://hz.tanke756.top/gtmthpkkrx.html

Py:   json.loads(s)
来源：http://hz.yueranfly.top/gtldhfceic.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtoybjdocu.html

JS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtzapyvaov.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtfawflvhn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gtryxjtwer.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtwsgbebqk.html

Ruby: JSON.parse(s)
来源：http://hz.nanxinkj.top/gtvipzoelh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangshuangyany.cn/gtmihlfrov.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sufxvd.cn/gthaddqwoo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtitesixda.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258.top/gtbpvbabsb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtnrqkclxn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gaohongyu789.top/gtsbexgodz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtkowaxmjd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yangfankeji.com/gtdmwicgec.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtkdtpfdtb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtejoqtsmg.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtfczefpag.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtcrkdsgqs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yanxiufei.cn/gtqkbfdxim.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtkponkgpb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtyiiuhgjs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj202588.top/gtmcfvvlyi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtemxpyprs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.snrcjt.cn/gtmixonomd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtvkagievb.html

[K05] 深拷贝对象
来源：http://hz.wangshuangyany.cn/gtwhjohwvm.html

Py:   copy.deepcopy(obj)
来源：http://hz.fzhhl.top/gtrzzmwdrr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtqakjuszu.html

JS:   structuredClone(obj)
来源：http://hz.smart0.xyz/gtjudtocju.html

TS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtfbdnjrpy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cdnleiting.top/gtnzqqqanc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtuqbofwmb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gtliqegyhl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtkzszrfta.html

[K06] 解析 URL 查询串
来源：http://hz.redwolf501.top/gtdilrojdq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hnxiangtu.top/gtigzhcngl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtmghonwrn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtkbjgazhz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtpzxqexwo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dianchejie.cn/gtksdnhtlu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shuidangran.top/gtszvjblss.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtnwpcvjqz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tianlin.xyz/gtmynhvqqh.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtojrfwcdf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gtwpewraxx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gtaenylclt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtoizfrurd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtqcedyqjg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtxqkuryah.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.quarkkingdee.top/gthtwvwoqp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tanke756.top/gtawhnybza.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gtkgklirhp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zycfv.cn/gtottrmweg.html

Py:   pickle.dumps(obj)
来源：http://hz.zhiwuduotai.top/gtcgdegmoe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangtech.top/gtmsdphzsl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtdwnredkc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtuutydtpa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtvtrceani.html

Go:   encoding/gob
来源：http://hz.tanke756.top/gtmkvhmvsu.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj202588.top/gtglttjffu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhixingplan.top/gthgusiesn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtidjewhzl.html

L. 网络请求
来源：http://hz.gzhubu.top/gtgklutkhn.html

================================================================================
来源：http://hz.ydjk.org.cn/gtnvxsqvyk.html

[L01] 发送 GET 请求
来源：http://hz.chenzaomai.com/gtixjyfwxp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtjcnefmdz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxuanxn.top/gtzojpjipi.html

JS:   await fetch(url)
来源：http://hz.shuidangran.top/gtbyhixwzp.html

TS:   await fetch(url)
来源：http://hz.sweek.top/gtlotcpzbp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtpvekqigb.html

Go:   resp, err := http.Get(url)
来源：http://hz.yonumen.top/gtyjqifijd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shzxlz.cn/gtmxadtsus.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hfpthk.cn/gtsnqequrv.html

[L02] 发送 POST JSON
来源：http://hz.chenzaomai.com/gtsrruazwe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtayblevap.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtjfsjmnnj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtszfshvap.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtpqhyritw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtwsewmycx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yanxiufei.cn/gtlwtdmmwz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daxiang520.top/gtgsakskfo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gtartgzyok.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gtnlheejki.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtmpmgfgwm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtyppwfibu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtihghjeqp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtkkedjblk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtweltuyhu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtfpngzlnk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtxywzyrep.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sysykeji.top/gtyfivtuga.html

[L04] 设置超时
来源：http://hz.smart0.xyz/gtpbrxrzxz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangtech.top/gtcdfulozs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gtxivajsta.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtasqhntff.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtcwkjemfs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtpmcktkyd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.mhx1999.top/gtkdnuryqn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangtech.top/gtzvqtcdif.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gtynjcdkxf.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtcawtjhes.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gtvttczvbz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtsvwkucwj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtepaegsap.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtcusuvkja.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.c1oappe.top/gteoyjmfit.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.bjfxy.top/gtdkykqmfo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtywnsxgkl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtmtoiqwjq.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtutjzjngy.html

Py:   resp.json()
来源：http://hz.jiagoushi.top/gttnwnnpbl.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gtplazxxpr.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gtctersaml.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtxgzefrxp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtirgdqhka.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtlhzfbzdi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtdnbgaajr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtlpfflbrs.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtubsqmppi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.0kj1m.cn/gtbxlqrmdp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zycfv.cn/gtnbhsjgtl.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtxnfkpqok.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtlwoqgtsv.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtbphetnnt.html

Go:   resp.StatusCode
来源：http://hz.0kj1m.cn/gthmvcsmha.html

Ruby: resp.code.to_i
来源：http://hz.pycfn.com/gtevvuzmvv.html

C#:   (int)resp.StatusCode
来源：http://hz.cashguo.top/gtuegdmzxa.html

[L08] 并发请求多个地址
来源：http://hz.daxiang520.top/gtxnypnojf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cashguo.top/gtqbzbhscu.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhiwuduotai.top/gtfqgskpqe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtsoxvmxbu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtnjykneaq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gtiwlbatvo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.kuanghao11.cn/gtgtibjihn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhixingplan.top/gtwiebvyiq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenlongwang.top/gtvlcqdymm.html

================================================================================
来源：http://hz.cqqwz.cn/gteczqfsmj.html

M. 命令行 / 进程 / 环境
来源：http://hz.fengsongda.top/gtwyhbjnxj.html

================================================================================
来源：http://hz.jqgfzy.top/gtmfxmzxdl.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtfrrdtdvd.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtmdhnopev.html

PHP:  $argv;  $argc;
来源：http://hz.havefunace.top/gtoptxawvh.html

JS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtqwzueafh.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtdpauylzm.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtixsylqbz.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtbfiqnlhp.html

Ruby: ARGV
来源：http://hz.gogol.net.cn/gtpcnrrmhs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jianghu66.top/gtixwxwwzd.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtkmjwilpi.html

Py:   os.environ.get("HOME")
来源：http://hz.jinghuilouyu.cn/gtuwkiokpn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtborgdkkh.html

JS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtsfjfitjc.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtrgvnhodl.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtkppoutzx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtytsjysyf.html

Ruby: ENV["HOME"]
来源：http://hz.jinghuilouyu.cn/gtbkygxwzn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenzaomai.com/gtmhvchmqd.html

[M03] 执行外部命令
来源：http://hz.cheryme.top/gtawfozixe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hfpthk.cn/gtaviwfkti.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yueranfly.top/gtrcsudlog.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtqcpwgelc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtiduxoqwg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtclxyibvn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.kuanghao11.cn/gtpulumwkq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.havefunace.top/gtkwjjuutu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigufen.top/gtqgxolqsc.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gtxokvyrcy.html

Py:   os.getcwd()
来源：http://hz.xinyue.icu/gtqgkeoizm.html

PHP:  getcwd();
来源：http://hz.xziqi.cn/gtnwcvwycz.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtistmnfzj.html

TS:   process.cwd()
来源：http://hz.9152youxi.cn/gtpcjhateo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.kuanghao11.cn/gtqtijktxw.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gtvbljlxeo.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtpfihsdbh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gtcslzkdcn.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtycdrxgej.html

Py:   sys.exit(1)
来源：http://hz.9152youxi.cn/gtlbhaoyam.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtjykzfstb.html

JS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtesqlincl.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtrbpwpepj.html

Java: System.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtugygshui.html

Go:   os.Exit(1)
来源：http://hz.daxiang520.top/gthvrwderg.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gtnmabpaiz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtgqdzsdwv.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gthrqkmgvs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtrrhqhmls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenlongwang.top/gtmrksxrjf.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gttjukykqr.html

TS:   console.error("err")
来源：http://hz.fzhhl.top/gtgsvlrsfx.html

Java: System.err.println("err")
来源：http://hz.meibo888.top/gtyhnuvqac.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtlgbkpsoj.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gtasruhqqm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.kuanghao11.cn/gtypehfunr.html

[M07] 判断是否为主入口
来源：http://hz.sufxvd.cn/gtdvrbylia.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtpaelrsxy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangdashe.top/gtjcvyyvnn.html

JS:   require.main === module
来源：http://hz.snrcjt.cn/gterpsgcxm.html

TS:   require.main === module
来源：http://hz.ydzc1.top/gtpvzlivue.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtbvvethcp.html

Go:   func main()
来源：http://hz.tian-w.cn/gtqcfmlfyt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhaomingkeji.xyz/gtdcnlznkv.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtxmctirtn.html

[M08] 获取系统与运行时信息
来源：http://hz.guannengcc.top/gtglkzdsux.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gthtwajqve.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hfpthk.cn/gtnuthjmzo.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtwypgcgrc.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtfjenrxdg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.iojbl.cn/gtlcfutabj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtchenbmyh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.vqdsnc.cn/gtwpghyyir.html


<!-- 参考信息 -->