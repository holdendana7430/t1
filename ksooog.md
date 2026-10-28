代发 wailian999

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtgxrbenkt.html

Ruby: Time.now
来源：http://hz.quarkkingdee.top/gthmgvlkhw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guannengcc.top/gthxvehpzn.html

[J02] 格式化输出
来源：http://hz.zhijiandao.cn/gtdssldjiz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtmwwigmcm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gthptvwepo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtawqghevj.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtazmujkyr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxinkj.top/gtrkyrtydv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtcdrnkbyj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.kuanghao11.cn/gtfldgepgs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gttgdaqzmk.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtsoaoqylp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtjpufylms.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtmlqufsth.html

JS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gttbcudavl.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtrjijoccl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangdashe.top/gturjvwlne.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xziqi.cn/gtiisjeazn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtuvbenpmt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.feifeiyinyue.top/gtnoqjeqys.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtyoylvrkq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtnkntrnzy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtpijjrxgb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtjnwhucge.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hfpthk.cn/gtdrmjzpth.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guowangkeji.top/gtvclecgab.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtdfjqzfib.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgufenzy.top/gtvaomared.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtgaznhwuz.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtorhggeog.html

Py:   now + timedelta(days=7)
来源：http://hz.jyoumei.cn/gtkjeeoqsy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gtledujyqf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtujimscuk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtjvmfskju.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shangyingyoupin.top/gtcleimgws.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtgjfwpzqt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtfdrayyak.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtimmgrdij.html

[J06] 计算两时间之差
来源：http://hz.ppjwa.cn/gthzyguvpa.html

Py:   (end - start).total_seconds()
来源：http://hz.daxiang520.top/gtfkaxdyii.html

PHP:  $end->diff($start)->days;
来源：http://hz.svipenyu.cn/gtcclwaxuc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtrrvqkbvd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtjshfrspv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtzwfrgazu.html

Go:   end.Sub(start).Hours()
来源：http://hz.ivvv.top/gtxzaxfvya.html

Ruby: end - start                 # 返回秒数
来源：http://hz.quarkkingdee.top/gtibgwdznb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yueranfly.top/gtuhzjmjzl.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtrsahrxlu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtopecknpr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtrygxldyn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtkyfnjssz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtdrhenghe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gttkqaduti.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ybcxt.top/gtijsvmsco.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtxqexixjs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtraumynbl.html

[J08] 提取年月日与星期
来源：http://hz.jqgufenzy.top/gtcazygatk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yanxiufei.cn/gtaftlfbql.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aibaodan.cn/gtbaojcxmv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gthkcavljj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhengqikj.top/gtdnozgpbd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xziqi.cn/gthyjtgwtq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtboyppfhr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtcpftmspp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtyouajxir.html

[J09] 时区处理
来源：http://hz.sweek.top/gtadycseup.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtuznamyto.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtfpqznzne.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtkczgkuld.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gttltucfuq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtnlmqxrmc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.meibo888.top/gtmvcqyqhc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nwbrower.top/gtcgpelmuf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gtubvkrxca.html

[J10] 取今天 / 本月第一天
来源：http://hz.iojbl.cn/gtsigejars.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgfzy.top/gtvgwfpyyb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dashuyun.cn/gtvnbqzmgd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtytbdnwse.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gtzkfvgyqb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtpeowabaw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtkbcyrozz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhixingplan.top/gtktdaqvvh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtjtswacef.html

================================================================================
来源：http://hz.pycfn.com/gtwjmlnpes.html

K. JSON 与序列化
来源：http://hz.ydzc1.top/gtoamywoye.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvdsxdbaw.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtoilajuwc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtlhufwqqt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtpspsmfhp.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtgoqdmrbf.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtfnnyjyef.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtlqedhhlw.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gtmqdogvzl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gtucdccpnu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtsecpspmo.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtcdbxgpuh.html

Py:   json.loads(s)
来源：http://hz.gotoacloud.top/gtcnxkzuuq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangkeji.top/gtlmyeaogo.html

JS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtlcnspbgp.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gterntuybm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigufen.top/gtuaubijmf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtjnucjimz.html

Ruby: JSON.parse(s)
来源：http://hz.cheryme.top/gtqyagrmmo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtpblloxmh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.svipenyu.cn/gtietmcxfg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtjnunrdvh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtvjwbmzfg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtkdobgbzy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtbeaxgisn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guowangkeji.top/gtrzpcwrlq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yanxiufei.cn/gtrpwqovvz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gtyquzqetd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtwqsndpba.html

[K04] 读取 JSON 文件
来源：http://hz.ivvv.top/gtdawtyjmz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shuidangran.top/gtfqhcoqar.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtbbxrfvwj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtoygtphkv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtytasejaw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtffahhufd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtvefkxxsg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtdgrmfjhj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtorxqsqcz.html

[K05] 深拷贝对象
来源：http://hz.gaohongyu789.top/gtapljhtba.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gtnvwucpue.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtjnvxvknt.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtfezsyiaq.html

TS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtuecvgjet.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtrrryjmnp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtsqyxjass.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtcnyuftwu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj202588.top/gtldewuglr.html

[K06] 解析 URL 查询串
来源：http://hz.sysykeji.top/gtazlepsex.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cdnleiting.top/gtphrqzolf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtokksdzmx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gthbmjjanb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtnmfivhpi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtcndoruqz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cqqwz.cn/gtmkpcofkv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtcssxlfoi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xinyue.icu/gtkmjpdjct.html

[K07] 进制转换
来源：http://hz.zhaomingkeji.xyz/gtmspvutrt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gtyozgshfp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xziqi.cn/gtvbfodxmk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.meibo888.top/gtoqyzinbn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtxemvlbqj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtgmuctswd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangdashe.top/gtmipjpplz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gtmhctqixh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dianchejie.cn/gtqrpclqcc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hammf.cn/gtdbeuupwj.html

Py:   pickle.dumps(obj)
来源：http://hz.jianghu66.top/gtqlyflsnc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.havefunace.top/gtsamdavbh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtgxkkxlfc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtsehpqsrs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhongyouzk.top/gtysiqpedn.html

Go:   encoding/gob
来源：http://hz.shuidangran.top/gtefdowdoi.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinghuilouyu.cn/gtzocncabf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuxming.cn/gtrasqumzs.html

================================================================================
来源：http://hz.smart0.xyz/gtnztqfaez.html

L. 网络请求
来源：http://hz.zhengqikj.top/gtsmarbyhv.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgulmsxld.html

[L01] 发送 GET 请求
来源：http://hz.birdmap.top/gtxyvimyzn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtrijntcuo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj202588.top/gtfhbcbzre.html

JS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtvgficxgn.html

TS:   await fetch(url)
来源：http://hz.yongpay.top/gtgsszkldr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sufxvd.cn/gtyjjpnfbt.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtduypcejl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hywenlv.cn/gtyhlcckow.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gtpkvqsbcf.html

[L02] 发送 POST JSON
来源：http://hz.cheryme.top/gtqbqftuqh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtwazepuct.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.bjfxy.top/gtdxjdumfd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.316326.xyz/gtvjghhxlg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtewstvnqb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.9152youxi.cn/gtfdfqdgam.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gteqkeuart.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtkjyyamda.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aizwys.cn/gteruhtskg.html

[L03] 设置自定义请求头
来源：http://hz.hnqzz.top/gtbywbukty.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydzc1.top/gttnxvcrqv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhaomingkeji.xyz/gtzfumvcfz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtpmwxzxkq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtftfqzevh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hongshengwenyu.top/gtjjnhhmdc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gthrzhfald.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangshuangyany.cn/gtjtcgoyjh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.andypj.xyz/gtgvmwdfxk.html

[L04] 设置超时
来源：http://hz.ywan-chungtsiang.top/gtzxmsczdg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gtaaadgrrr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtivgmwpnh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtfbemtnab.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxinkj.top/gtrqtzpapi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tian-w.cn/gtinmtoscs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tianlin.xyz/gtotcstoid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yongpay.top/gtavkyhrcr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtgaiwuywr.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtdzashfis.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtrzqlkpyw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtixcirmhb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtwmppyhle.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtuaditsgt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gaohongyu789.top/gteldsawna.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fzhhl.top/gtwjsdburt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtpasgapjr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shuidangran.top/gtdblssizt.html

[L06] 解析响应为 JSON
来源：http://hz.haohaochexian.top/gtlplznkpn.html

Py:   resp.json()
来源：http://hz.hfpthk.cn/gteemrgdaj.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtitistxxq.html

JS:   await resp.json()
来源：http://hz.yj20258888.top/gttwufwydt.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gtkwqamrdm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangtech.top/gthixvgpgr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtfxesdezf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtmvarxffd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aibaodan.cn/gtbmotoexl.html

[L07] 处理 HTTP 状态码
来源：http://hz.xziqi.cn/gtczctydma.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ywan-chungtsiang.top/gtlotmmkad.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtvusqasdp.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtipvwastu.html

TS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtzfqtclpj.html

Java: resp.statusCode()
来源：http://hz.tanke756.top/gtlitpqndb.html

Go:   resp.StatusCode
来源：http://hz.iojbl.cn/gtoytjgsws.html

Ruby: resp.code.to_i
来源：http://hz.jqgfzy.top/gtoeljlwby.html

C#:   (int)resp.StatusCode
来源：http://hz.birdmap.top/gtvyholtqw.html

[L08] 并发请求多个地址
来源：http://hz.9152youxi.cn/gtkrdohpyh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtrhnyvmfi.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtmkffrcai.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cashguo.top/gtitzkjlww.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtrisvaeyn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtedukuvuv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jqgfzy.top/gtkgzqsyce.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtfdzvnllt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinghuilouyu.cn/gtbcqkcahm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtnlqzaedc.html

M. 命令行 / 进程 / 环境
来源：http://hz.vqdsnc.cn/gttgydciiz.html

================================================================================
来源：http://hz.haohaochexian.top/gtikskfveb.html

[M01] 读取命令行参数
来源：http://hz.feifeiyinyue.top/gtbdvramew.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtnmiyzxai.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtxuaiskkv.html

JS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gteczihitw.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtlfzdkyoq.html

Java: args 数组（main 方法参数）
来源：http://hz.cdnleiting.top/gtpelmpdwb.html

Go:   os.Args[1:]
来源：http://hz.pengpengdd.cyou/gtzoiaixqp.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtevbykklr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shzxlz.cn/gtxownwybc.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtufeovvsh.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxinkj.top/gtcvrlyokc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtedwpnrke.html

JS:   process.env.HOME
来源：http://hz.xziqi.cn/gtzowwlvya.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gthdpqeazv.html

Java: System.getenv("HOME")
来源：http://hz.jqgfzy.top/gtyxgqrpku.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtggbnwzgc.html

Ruby: ENV["HOME"]
来源：http://hz.pengpengdd.cyou/gtjicxylhk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pycfn.com/gtkgcbfbqi.html

[M03] 执行外部命令
来源：http://hz.snrcjt.cn/gtotnhzvog.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.andypj.xyz/gtxkiesgag.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.9152youxi.cn/gtcakzrfms.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtfmoddhtv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtjdcparxw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gtdsukrnln.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hammf.cn/gthrelakmd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gttlghaxmw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtjirtepfs.html

[M04] 获取当前工作目录
来源：http://hz.shuidangran.top/gtiqqzeczi.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtkjakknve.html

PHP:  getcwd();
来源：http://hz.sufxvd.cn/gtuxdgnmuw.html

JS:   process.cwd()
来源：http://hz.chenzaomai.com/gthwgdgnmt.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtumcfopeo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.andypj.xyz/gtadvlndmb.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtnnpmfsxe.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtsniiieyk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jlsjyb.cn/gtlemzvjgk.html

[M05] 设置退出码
来源：http://hz.chenzaomai.com/gtxcptgejf.html

Py:   sys.exit(1)
来源：http://hz.52xcode.cn/gthvgrylap.html

PHP:  exit(1);
来源：http://hz.birdmap.top/gtxrfzktyz.html

JS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtrkovfbya.html

TS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtibnoennp.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtjmyaicew.html

Go:   os.Exit(1)
来源：http://hz.cdnleiting.top/gtazgkycwq.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtflojgwgv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtyzjrzvpx.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gtoqdxxqne.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shangyingyoupin.top/gthrlkyegu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gtsmksfvbs.html

JS:   console.error("err")
来源：http://hz.yuanzhike.top/gtomfzkidi.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtgnehrkqh.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtzebatspx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gtoitxrspa.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtskzasqcz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtmlaprjpu.html

[M07] 判断是否为主入口
来源：http://hz.ywan-chungtsiang.top/gtuoeinfiu.html

Py:   if __name__ == "__main__":
来源：http://hz.sxryk.cn/gtfiptqwgx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jlsjyb.cn/gtotxorqog.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtrlwzixio.html

TS:   require.main === module
来源：http://hz.yonumen.top/gtkguxfylq.html

Java: public static void main(String[] args)
来源：http://hz.zhaomingkeji.xyz/gthebcuahy.html

Go:   func main()
来源：http://hz.feifeiyinyue.top/gtnehaeydj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fengsongda.top/gtldugoheh.html

C#:   static void Main(string[] args)
来源：http://hz.shangyingyoupin.top/gtkcrtkfan.html


<!-- 参考信息 -->