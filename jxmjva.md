代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtnybvlnht.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtghyoutsr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtgkgolzek.html

TS:   d.toISOString()
来源：http://hz.yvedp.cn/gtdljdyhgw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.meibo888.top/gtjgnamvhj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hammf.cn/gtjpdkfqeb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gtvejvcbsa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gteftzgueu.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtlaosvgue.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtvdlzzbmn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gzhubu.top/gtpfdqpirm.html

JS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtcstchyke.html

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtkstmuvdi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj202588.top/gtmlrpqggw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtpsfhhtlj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtivweflud.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dianchejie.cn/gtdtfdpvbg.html

[J04] 时间戳与日期互转
来源：http://hz.yueranfly.top/gttiprzbdd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtqlhxxovi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtwpopinfz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gtujehuroy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.vqdsnc.cn/gtjeqjvask.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinyuanbaomall.cn/gtxysfgcri.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtqeyrbidr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fengsongda.top/gtuoxztdai.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhixingplan.top/gttbjubwze.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gteqkimfwk.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigufen.top/gtugsmjvsm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtwgaqfacq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtbwarpdeq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtpyzovwxk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sweek.top/gtnhyobpwg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nwbrower.top/gtnxbgvdbg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtwzjsyoit.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtsowixadm.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gtazyhefjg.html

Py:   (end - start).total_seconds()
来源：http://hz.ydzc1.top/gtqhkoizvx.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtqfegobvl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sweek.top/gtxwgsxzkr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cqqwz.cn/gtdpqylpnp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xinyue.icu/gtswtfabzk.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtzbchuvso.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zdqjudy.top/gtgdezusdc.html

C#:   (end - start).TotalSeconds
来源：http://hz.gzhubu.top/gtqqlngjeh.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtlyqblqkp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtmzaatskv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnxiangtu.top/gtcjojpsid.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtmitttghq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtgqetqrsu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtkrvglsfw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gthnypcqil.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtzgihxnaf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtfyqpsqra.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gtdtlvdmfq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yanxiufei.cn/gtffojcfmz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtkkoznsfi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtsxmnurvz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gterjfghme.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gtedfgznty.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtdtillatu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ehwqpu.com/gtjidiphvb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jyoumei.cn/gtfubpudue.html

[J09] 时区处理
来源：http://hz.shzxlz.cn/gtpyelkwys.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtyyonvrrp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtymwyjcft.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtahbucwyg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtgwpbvyho.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtfmrujdjs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ppjwa.cn/gtgwrswrys.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.9152youxi.cn/gtzeklwkdr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tanke756.top/gtozujnthw.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtsowavmgh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jlsjyb.cn/gtgfvqtvro.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtjbxexmjp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.9152youxi.cn/gtxfsoucfr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtyhzpshyk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtdhjmdyke.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtyodtpbjp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtqdzkbvlg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtthhagegh.html

================================================================================
来源：http://hz.xylfe.cn/gtgpppeaxk.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtajjtvuha.html

================================================================================
来源：http://hz.shuidangran.top/gtdsueskvp.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtxssbvhvb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtrongohma.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtrhyloyis.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtvmlgufnr.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtzmzkexvt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pengpengdd.cyou/gtgpqjbpdd.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtdiznuidn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhengqikj.top/gtzlnmdrwf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtksqwysjw.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigufen.top/gtbcozdyzs.html

Py:   json.loads(s)
来源：http://hz.gzhubu.top/gtulzvzdac.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yvedp.cn/gtxpmyethj.html

JS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtxmkjudwi.html

TS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtzsbeswzg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtncjcrtsd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtmuxsdmap.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtkymmdmnb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtgtkyxzwb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sufxvd.cn/gtwifvllja.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtxxapcmzd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtkbolqsbm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtrrmnjaxr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtrfintjjb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtlzzdpzuu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gtmleqskdv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtblwiipmt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gtcrgysubc.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtcgebanmc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yvedp.cn/gtspwibiic.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtkmjwubph.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtnvqtzpby.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gthlkrzrdg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtdwtajhbx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtihaifuwi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cashguo.top/gtsaicfetu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtscaouesm.html

[K05] 深拷贝对象
来源：http://hz.hnqzz.top/gtqcpqzrlx.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuxming.cn/gthjjblbzj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtkprcahmn.html

JS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtpnuxezhp.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtqwrpwyyy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuxming.cn/gtjmhvspdc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guowangkeji.top/gtrompqymj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.bjfxy.top/gtsfiktqsj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtlszsyqiw.html

[K06] 解析 URL 查询串
来源：http://hz.9152youxi.cn/gtkzpdixcr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhoulong.xyz/gtojcfygxp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.smart0.xyz/gtwgqcvrqb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtmzycocnj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtqlaquwxi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pycfn.com/gtftpfpxfu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtocisrmjg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtsprlgtuc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtkbgvqzmd.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtybftxywl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtjgecgqep.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gttmnlfzdp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shuidangran.top/gthwkdugvi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtmyumuulz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtwzisdqij.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.andypj.xyz/gtkgkowvgo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gtnbzjsokp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.0kj1m.cn/gtjqcrcnkl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtdlyqifpo.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgfzy.top/gtbrbyfcdm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gthcaaebaw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtmedohvlj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtyadrogty.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cucudq.cn/gtnyoikeac.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gtrghdoaks.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtvsevxolr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtqyqcmuzm.html

================================================================================
来源：http://hz.bjfxy.top/gtypdsxxca.html

L. 网络请求
来源：http://hz.jianghu66.top/gtmfrvxsav.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtawnaidmm.html

[L01] 发送 GET 请求
来源：http://hz.xziqi.cn/gtiivxnvtc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xingfuxueyuan.xyz/gtvycrhkfo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhengqikj.top/gtdahltdiv.html

JS:   await fetch(url)
来源：http://hz.xinyue.icu/gtrmlwajus.html

TS:   await fetch(url)
来源：http://hz.birdmap.top/gtjdirjzks.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xziqi.cn/gtvqafdimv.html

Go:   resp, err := http.Get(url)
来源：http://hz.sxryk.cn/gtrwgvmskj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtffqylshn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tanke756.top/gtxeyrrqfu.html

[L02] 发送 POST JSON
来源：http://hz.xinyue.icu/gtlnqsguax.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtrvitkbxt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gttccfvnee.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtaqcqjxbn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtcojgibyr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtlzqgtqou.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtkbbagzpo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cqqwz.cn/gttftvnlhn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gtdirbdlpt.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gthjoollhf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gteogbxget.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gtsqwqlhrr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtfzjvfykf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtwhsgplmm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dashuyun.cn/gtakqldaaf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtnenxqubx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuanzx.com/gtgopcgpeu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gthrefuvkq.html

[L04] 设置超时
来源：http://hz.gogol.net.cn/gtzzspfhep.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jiagoushi.top/gtrkwbjkqv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gtxakyordo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtbgjqnuwa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtytlqbesa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtxttsdlek.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.birdmap.top/gtcggwsywt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinghuilouyu.cn/gtcwjysdpp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gtirbrydzv.html

[L05] 上传文件（multipart）
来源：http://hz.zhoulong.xyz/gtoveribzr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gtunhzqjux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenlongwang.top/gtxxhuzvkc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtoneyriim.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtzvlsxurv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guannengcc.top/gtddmrkhdp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtlwicltel.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.9152youxi.cn/gtugvxyixg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dashuyun.cn/gtozusntob.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtfypnmolf.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtirskkhbz.html

PHP:  json_decode($body, true);
来源：http://hz.cucudq.cn/gtmtsizlqs.html

JS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtrfnmbglj.html

TS:   await resp.json()
来源：http://hz.yuxming.cn/gtaeblitzt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gttjtfqwqc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gteemwpluy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtflepkxai.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gttxrfgpku.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtvlfrjrwh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.vqdsnc.cn/gtvrfqijds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gotoacloud.top/gtffpnxcxl.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtnrijfleh.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtwqmwtjyi.html

Java: resp.statusCode()
来源：http://hz.yuanzhike.top/gtfrazgxgz.html

Go:   resp.StatusCode
来源：http://hz.dianchejie.cn/gtjsmpnhyc.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtrzzaqyas.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gthvnvkewu.html

[L08] 并发请求多个地址
来源：http://hz.cucudq.cn/gtryivejip.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtwhwxplge.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtzdwesrtz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtlqyyrwyh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtctrirykm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtymalbsoh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhengqikj.top/gtkbdulfgl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gtiajpquib.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gtnvfduhbh.html

================================================================================
来源：http://hz.yanxiufei.cn/gtuhvvouzl.html

M. 命令行 / 进程 / 环境
来源：http://hz.zdqjudy.top/gtvirnjifl.html

================================================================================
来源：http://hz.ehwqpu.com/gtqrdpaslo.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtqekkvfjs.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtdpdimhml.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtymilzfnv.html

JS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtshsotvgd.html

TS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtfpeyqlzp.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtylbnmfjh.html

Go:   os.Args[1:]
来源：http://hz.gogol.net.cn/gtuybpwpqn.html

Ruby: ARGV
来源：http://hz.xingfuxueyuan.xyz/gtqdhdtuyb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gtuscsjbmd.html

[M02] 读取环境变量
来源：http://hz.daria6918.cn/gtzjmyitle.html

Py:   os.environ.get("HOME")
来源：http://hz.cqqwz.cn/gtrlyieijh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.c1oappe.top/gtkyzqgizw.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtqpimsudq.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtrwdsrahq.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gttujcznxk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtxqwapikb.html

Ruby: ENV["HOME"]
来源：http://hz.meibo888.top/gtxdcbtgge.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xylfe.cn/gttnjxuymx.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtyecxpinp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgfzy.top/gtmlbfgdod.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhiwuduotai.top/gtmaouijhi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtjwpnndxa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtytqrgrcf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yangfankeji.com/gtijgukhku.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nwbrower.top/gteprhlbgs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtzipgewpe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sysykeji.top/gtqhuifshj.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtfoxmpfgc.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gthkhfgpxo.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gtvmiuhjow.html

JS:   process.cwd()
来源：http://hz.yuxming.cn/gtmilntzkj.html

TS:   process.cwd()
来源：http://hz.smart0.xyz/gtkxzjrerb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydzc1.top/gtyiilstsv.html

Go:   os.Getwd()
来源：http://hz.cheryme.top/gtwkeeoslr.html

Ruby: Dir.pwd
来源：http://hz.jinyuanbaomall.cn/gtqzmvqbzl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydzc1.top/gtnttpqwvu.html

[M05] 设置退出码
来源：http://hz.316326.xyz/gteznqmsdq.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtlswnjsya.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtxpizzwii.html

JS:   process.exit(1)
来源：http://hz.iojbl.cn/gtejbbmmaa.html

TS:   process.exit(1)
来源：http://hz.sweek.top/gtofliekqc.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtcuzqnhnl.html

Go:   os.Exit(1)
来源：http://hz.aizwys.cn/gtyjbynwdr.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtmwlxhlgi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuanzhike.top/gtgqzaivut.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gtumxaivns.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yj20258.top/gtnkldrner.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cdnleiting.top/gtgsuyidrc.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtkcwrccvd.html

TS:   console.error("err")
来源：http://hz.sweek.top/gtcocpjujb.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtlrlfrsxa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.feifeiyinyue.top/gtawhqhwwl.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtyejbowfv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtwuozwksn.html

[M07] 判断是否为主入口
来源：http://hz.xylfe.cn/gtixhbyvmb.html

Py:   if __name__ == "__main__":
来源：http://hz.ehwqpu.com/gtrydshsxo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yueranfly.top/gtkwntccrp.html

JS:   require.main === module
来源：http://hz.gaohongyu789.top/gtkemrfyrh.html

TS:   require.main === module
来源：http://hz.sysykeji.top/gtgivzfldi.html

Java: public static void main(String[] args)
来源：http://hz.pycfn.com/gtwzipfdzr.html

Go:   func main()
来源：http://hz.gotoacloud.top/gtszoozfiu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yangfankeji.com/gteaklgdhs.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gtzqgqnqth.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtorqghata.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtvfjketlq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fengsongda.top/gtkyljsnxm.html

JS:   process.platform;  process.version
来源：http://hz.zycfv.cn/gtjdokzwdd.html


<!-- 参考信息 -->