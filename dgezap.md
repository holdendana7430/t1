代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gtujtctpke.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtgaxidxgk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yanxiufei.cn/gtbtpeueio.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtvsajmesg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhixingplan.top/gtbtboxbav.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtlymgkhym.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yonumen.top/gtgkxtzngc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhiwuduotai.top/gtvajkgbxh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtmgeguoxy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtyrxizrmm.html

[J05] 时间加减（加 7 天）
来源：http://hz.ivvv.top/gtfslncgdn.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtkskxjyrh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hfpthk.cn/gtpgvnimuk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtgabcfkcn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtxivppqlk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yvedp.cn/gtzgfyesnq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gttvgoxplw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.316326.xyz/gtdswqdjzf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtnclzbkus.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtlmxfsaeh.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtetagyern.html

PHP:  $end->diff($start)->days;
来源：http://hz.pycfn.com/gtptbvvlmf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sweek.top/gtyrsrgcoj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtsxmtfkan.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shangyingyoupin.top/gtzgdqkdyv.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtfejbjntx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gthbwaxcna.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtebmwoivz.html

[J07] 比较两个日期
来源：http://hz.jinghuilouyu.cn/gtalytbqtc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtzkkspmof.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gotoacloud.top/gtounglrje.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtikbnxlec.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtosfkdxbj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtlrynwmxc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtrpmbwgaj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtjinfytot.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtahxbowxc.html

[J08] 提取年月日与星期
来源：http://hz.vqdsnc.cn/gtnizlsrxi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtkwryfipy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtxpkycnhh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gtosinwnay.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtnowgxcry.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtvtogirmc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tianlin.xyz/gtupfbzapw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hywenlv.cn/gtyrodwetb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgfzy.top/gtjjahrwuk.html

[J09] 时区处理
来源：http://hz.yvedp.cn/gtddrsiwsl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.9152youxi.cn/gtzbkmfoqu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtmisupwvq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gtwougkwmb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtxbybvsur.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gtwxshyuni.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gtafcinbau.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.0kj1m.cn/gtxqjbcvhj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigufen.top/gtdvnwinqr.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtodnnkjna.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daria6918.cn/gtmcsqupbt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtpmddccsi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtxfgbuhkr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aizwys.cn/gtansaytci.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258888.top/gtgjcxvczs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258888.top/gthkjiqhqq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gtsdtjvksj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sxryk.cn/gtfelktsfb.html

================================================================================
来源：http://hz.yongpay.top/gtrhjundsv.html

K. JSON 与序列化
来源：http://hz.xylfe.cn/gtlhnnexwf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtljhqoizd.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtkxzggbzz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gtttqlvxrs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xinyue.icu/gtliuzghky.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtxlcptcdj.html

TS:   JSON.stringify(obj)
来源：http://hz.sufxvd.cn/gtyyklergc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xingfuxueyuan.xyz/gtxkuixdfu.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtxrdweuov.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtnrugyziw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtprjgykec.html

[K02] JSON 字符串转对象
来源：http://hz.jqgfzy.top/gtaobluhws.html

Py:   json.loads(s)
来源：http://hz.yj20258.top/gtfmjyeidt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhongyouzk.top/gtvlcfekwu.html

JS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtexnkpxhb.html

TS:   JSON.parse(s)
来源：http://hz.yj20258.top/gtpgqeours.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtxuluinwr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuxming.cn/gtrqbyhepp.html

Ruby: JSON.parse(s)
来源：http://hz.andypj.xyz/gtjanqekri.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtzypzgbcp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtcctpzfxk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtneylsozk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtdaahrurt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtfnxrcngg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtbjsgtenv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gtdrblfkgf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gtaqmefafr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtxjnukecd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gotoacloud.top/gtfkhgbqsw.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtirwlwjui.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj202588.top/gtrumboalz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtitkeciyx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gtyeiohudy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtuvoummem.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.feifeiyinyue.top/gtlrjyozvr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtymcvxlxm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gthshxnhkp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gtkfnbqwvu.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtifhwqnrk.html

Py:   copy.deepcopy(obj)
来源：http://hz.ppjwa.cn/gtscvhzftm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gtxddsoqxm.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtcvaxlmsq.html

TS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtdxdjlrbd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gtymrmuhxl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtxyieoskx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dashuyun.cn/gtqycnvjjx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtubqdouwb.html

[K06] 解析 URL 查询串
来源：http://hz.ydzc1.top/gtrwisjszi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gttdxgbhfi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gtximxhpuq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtjvasrcux.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtjcwomyce.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtjigajlaq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tianlin.xyz/gtvkrhfjdv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtpfbuwrda.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtyoeahkci.html

[K07] 进制转换
来源：http://hz.yvedp.cn/gtscbdfjrt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sysykeji.top/gtlckybqfs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gthnxjhtlo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtyaivxcoz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtsxgujyfz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtdftbbicj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtyfajketz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuanzhike.top/gtlwgbqakr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnxiangtu.top/gtrlocmmes.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtozlkdpab.html

Py:   pickle.dumps(obj)
来源：http://hz.zhaomingkeji.xyz/gtwpzrkjbn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtxwvgpqvl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pycfn.com/gtkxmctlmu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtwhhmicyf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtbiruypvh.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtxtdlmhhm.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtujqxwrks.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gteiaabmdn.html

================================================================================
来源：http://hz.jiagoushi.top/gtfrjztvru.html

L. 网络请求
来源：http://hz.nanxinkj.top/gtzwftpuyr.html

================================================================================
来源：http://hz.chenlongwang.top/gtzqrnlnyo.html

[L01] 发送 GET 请求
来源：http://hz.haohaochexian.top/gtfomhpgdg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangshuangyany.cn/gttrrhxkqt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj202588.top/gtftlctlib.html

JS:   await fetch(url)
来源：http://hz.andypj.xyz/gtipkwtwgo.html

TS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtnelkurag.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gtdmxlkwoz.html

Go:   resp, err := http.Get(url)
来源：http://hz.yangfankeji.com/gtbpwetsvk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtilqmsidf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.haohaochexian.top/gtshpplfht.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtsjynflnt.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gthvbtddtj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtbxwdhuyi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtkyiwayyb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtvisceuma.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtpvztaquz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuxming.cn/gtjfjrtqic.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gtkmepfwhn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgfzy.top/gtwtptnuqb.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtztpugltw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtaeulmaib.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtzwwcfzds.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.52xcode.cn/gtduznakrw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtgeqikhed.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtvshwmomf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtwmbdhpvd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtcznycudn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.vqdsnc.cn/gtgebbgrdf.html

[L04] 设置超时
来源：http://hz.hongshengwenyu.top/gtmjfkijpj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hongshengwenyu.top/gtrmvqyacr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258.top/gtmkwkrfwz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtbfqydark.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtwmuzdozx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gzhubu.top/gtyfdzmnks.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gthmxvpavr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yueranfly.top/gtrniggooo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangshuangyany.cn/gtdmxciqzl.html

[L05] 上传文件（multipart）
来源：http://hz.wangdashe.top/gtdluchajn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtxdmyoleg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gogol.net.cn/gtdabhaoeu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtyemqnxut.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtljqbgmlf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.havefunace.top/gtfmarvifm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gtzptiwnlw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtujeoyhlr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtvxbgnvmn.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtelyhpfvn.html

Py:   resp.json()
来源：http://hz.gogol.net.cn/gtjfpgjwuq.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtwyhvdahx.html

JS:   await resp.json()
来源：http://hz.yuxming.cn/gtfvqgwfnn.html

TS:   await resp.json()
来源：http://hz.guannengcc.top/gtalrbqxle.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hammf.cn/gtmgcbiiwx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cucudq.cn/gtdvwufaow.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj20258.top/gtfqmnvaeq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gtpyumicxy.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtwerotjqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtugfwdsxt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hongshengwenyu.top/gtrlkaocmp.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtthcqvytq.html

TS:   resp.ok;  resp.status
来源：http://hz.fzhhl.top/gtzneljjpw.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangtech.top/gthupgwhwx.html

Go:   resp.StatusCode
来源：http://hz.kuanghao11.cn/gtpyxfxlhr.html

Ruby: resp.code.to_i
来源：http://hz.yonumen.top/gtrfmqdwty.html

C#:   (int)resp.StatusCode
来源：http://hz.vqdsnc.cn/gttmbqvyvo.html

[L08] 并发请求多个地址
来源：http://hz.chenzaomai.com/gtqiripaur.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jianghu66.top/gttevaiuzx.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtuzqjvkbj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtmypnxlgj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtdvrjhpyv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gaohongyu789.top/gtuszgjzdw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gturvdvbvq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ppjwa.cn/gtsiyzbomt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtsqllzwhm.html

================================================================================
来源：http://hz.xuanzx.com/gtqeigotea.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtprmejmoy.html

================================================================================
来源：http://hz.hnqzz.top/gtnzuulwgb.html

[M01] 读取命令行参数
来源：http://hz.fengsongda.top/gtuqeuuhof.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtwrtqdkaj.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtiykzutol.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtxejcswlo.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtiijqgxtc.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258888.top/gtdjsybbpi.html

Go:   os.Args[1:]
来源：http://hz.ehwqpu.com/gtsqobosvr.html

Ruby: ARGV
来源：http://hz.pycfn.com/gteqxmwflx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sxryk.cn/gtnjxqldwp.html

[M02] 读取环境变量
来源：http://hz.bjfxy.top/gtuwojpxdq.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtcfqhonte.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.0kj1m.cn/gtwppyoxsw.html

JS:   process.env.HOME
来源：http://hz.ybcxt.top/gtpkzsukyk.html

TS:   process.env.HOME
来源：http://hz.hnxiangtu.top/gtbldwazyk.html

Java: System.getenv("HOME")
来源：http://hz.sweek.top/gttnzxneby.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tian-w.cn/gtyujguitm.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gttqixiljf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuxming.cn/gtssmjurvk.html

[M03] 执行外部命令
来源：http://hz.hfpthk.cn/gtfxhhleag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cucudq.cn/gtxyhkyqra.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtcusazwks.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtkxylkkgl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtkynhqpsm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtlgacnmet.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yonumen.top/gtuukkwvwr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuetiantiany.cn/gthcmdyqsd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gtfgdjtfwb.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtsiwaquuj.html

Py:   os.getcwd()
来源：http://hz.birdmap.top/gtcbvfeoaf.html

PHP:  getcwd();
来源：http://hz.yj20258888.top/gtcqpsohcj.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtoryvefmw.html

TS:   process.cwd()
来源：http://hz.daria6918.cn/gtfikpcwtj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtqtfpgheq.html

Go:   os.Getwd()
来源：http://hz.bjfxy.top/gtluvcqfry.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gtiytgjjuy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xylfe.cn/gtcjcadzif.html

[M05] 设置退出码
来源：http://hz.pycfn.com/gtilyqwsib.html

Py:   sys.exit(1)
来源：http://hz.redwolf501.top/gtewzihpng.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtrzmhzovn.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gteonmmdlw.html

TS:   process.exit(1)
来源：http://hz.ivvv.top/gtwrycqmrh.html

Java: System.exit(1)
来源：http://hz.jinqigufen.top/gtzzyvsqpb.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtdtdvcuqc.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtolorgiwc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yanxiufei.cn/gtplgaveld.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gtqfftmonp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.9152youxi.cn/gtzntrokxi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtwumcjfog.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtvjbujwwm.html

TS:   console.error("err")
来源：http://hz.xylfe.cn/gtvazxzfer.html

Java: System.err.println("err")
来源：http://hz.hammf.cn/gtuhzoeavn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yvedp.cn/gtkcgacplz.html

Ruby: warn "err"
来源：http://hz.quarkkingdee.top/gtstuueixx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258.top/gtbdjvqklq.html

[M07] 判断是否为主入口
来源：http://hz.cqqwz.cn/gtnhbxrgmf.html

Py:   if __name__ == "__main__":
来源：http://hz.fengsongda.top/gthyvnhoom.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgufenzy.top/gtiqzegmmq.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gtylgtwsqf.html

TS:   require.main === module
来源：http://hz.xinyue.icu/gtrgvmkvad.html

Java: public static void main(String[] args)
来源：http://hz.xingfuxueyuan.xyz/gtvekwwbtp.html

Go:   func main()
来源：http://hz.aizwys.cn/gtlzzrrlph.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenzaomai.com/gtmnhbvxck.html

C#:   static void Main(string[] args)
来源：http://hz.gotoacloud.top/gtzbqhfqou.html

[M08] 获取系统与运行时信息
来源：http://hz.yanxiufei.cn/gthmphxdks.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxinkj.top/gtipzqqiqz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinyuanbaomall.cn/gtonkpiuxa.html

JS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtsxmrsorq.html

TS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtrqtsypim.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xingfuxueyuan.xyz/gtybmknjqt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.0kj1m.cn/gtitiezudm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daxiang520.top/gtmrsdqllt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtqwiiqyyh.html

================================================================================
来源：http://hz.sxryk.cn/gtfojrnclk.html

N. 数据结构与算法
来源：http://hz.daxiang520.top/gtsbynsqrk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpxouznog.html

[N01] 二分查找（有序数组）
来源：http://hz.svipenyu.cn/gtudzzkmxd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.guannengcc.top/gtshwfqifr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj202588.top/gtftimzoqv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtfhtyhixx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtbrywrnam.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.quarkkingdee.top/gtvqrgskzl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hywenlv.cn/gtwwgwfpdv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtnhktqbxj.html


<!-- 参考信息 -->