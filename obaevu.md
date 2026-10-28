代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtszjbwiwk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gtijvtreti.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtsakizyeu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtcwlwtzso.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhiwuduotai.top/gtecohxjau.html

[J04] 时间戳与日期互转
来源：http://hz.kuanghao11.cn/gtgfwdqhba.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtfsmvgmav.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xylfe.cn/gtzatbplku.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtenmxltqp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtdqqevihd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.mhx1999.top/gtvxhgkslf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.svipenyu.cn/gtumkjzrdv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtvwzzvkix.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj202588.top/gtuvubyqpl.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtfvfbokcg.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gtmfivkskf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dianchejie.cn/gtmqmmeokp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtninlmldg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gturgimvrd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtimxztxyv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtyhejchpf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.smart0.xyz/gtexhpzfhk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtzgzyyiel.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtuawxpyzk.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtjxorfdml.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhongyouzk.top/gtivvboyks.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtsxoqtish.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gotoacloud.top/gtpyjjiitf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtgwjvnwny.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gthrxtfoka.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtaeisnseg.html

C#:   (end - start).TotalSeconds
来源：http://hz.guannengcc.top/gtxjxaiead.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtvrekavue.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtrrpjtbbb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtdmodfjst.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtqavjgznx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtxjacusyv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtfszlkpfj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ywan-chungtsiang.top/gtyyalqade.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtrouuscbt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtrqnkltsy.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtjuqpqpbw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gthsansuwc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yanxiufei.cn/gtfoyuczce.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtpjtrfewj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.andypj.xyz/gtzjruphwz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tianlin.xyz/gtjamtsdak.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtgohdmleq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtyfsqquml.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtzssandtp.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtkzplugjp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtkiivknad.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gthouscuso.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtakclsrhg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtcuratgtp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtpxmmkelh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gtlbihehgp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gttryrfgmo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhongyouzk.top/gttojkmtzt.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtnvxhergu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shzxlz.cn/gtoydphioh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gtzehehdvb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtdkcrimld.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtxmiwdlzf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.quarkkingdee.top/gtwnemyetf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtdaugpmqj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.0kj1m.cn/gtwlngtifw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtdyykdxny.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtloethwlx.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gthkganwal.html

================================================================================
来源：http://hz.c1oappe.top/gtbtikrsso.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangshuangyany.cn/gtupzesgym.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtbopljfmg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtbdqkklsl.html

JS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtuwtbegbn.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtqvvwbtyw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cucudq.cn/gttyudtdnq.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtxcxpywza.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnqzz.top/gtjjggjfia.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gogol.net.cn/gtszbncxdz.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtbskwlzsz.html

Py:   json.loads(s)
来源：http://hz.tanke756.top/gttntgxzpk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gtpvjcnzqw.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtqrznjlzg.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtptxwejuj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtlbvgmugd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtgtizxyav.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtsvovyrdg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtcbbgdtcl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtfjlgogzh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtokepoaht.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtviwpftdj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtyifimqji.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtmrvvwopp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gteotpczik.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hammf.cn/gtycfsanrh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtebgzvlbu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtbxxfhaqx.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gtouwkdyvz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hammf.cn/gtcajtiofw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhongyouzk.top/gtaxadxxqo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtvncgwvih.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtxqspyvug.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtksmfzvlx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtlphrnxyz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.c1oappe.top/gtursfdznp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.svipenyu.cn/gtawdlhion.html

[K05] 深拷贝对象
来源：http://hz.xuanzx.com/gtkaxxfgxj.html

Py:   copy.deepcopy(obj)
来源：http://hz.mhx1999.top/gtuocqewql.html

PHP:  unserialize(serialize($obj));
来源：http://hz.svipenyu.cn/gtzfsfqmzo.html

JS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtblmhfslt.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtfrmnwhjs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtdpfrmeni.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtqsndwsrg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtcytyzodw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtufswhogc.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtfmscgtdn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtldgkwpnh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gteqkhaxfn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtdinzxelh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtmemwyqat.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtbldkrczm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtlwyjenuo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtbpxiquag.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtvdzxwhrs.html

[K07] 进制转换
来源：http://hz.jqgfzy.top/gtmjdsjmgf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtctnqwqkq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zycfv.cn/gtbtestwny.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtsrkcypuc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gtpkdztaoq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtlcfmfyun.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtrbuuvvdz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yanxiufei.cn/gtlxllqegi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.mhx1999.top/gtszdsedhp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuanzx.com/gtmydyhaxc.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtjfhwyvob.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daxiang520.top/gtxdnaefok.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtvuvbbpfd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtnopiqfff.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gtlkcjmtrx.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtmryymyut.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtqpmsbmfo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtiwdzuqtv.html

================================================================================
来源：http://hz.c1oappe.top/gtntkicehz.html

L. 网络请求
来源：http://hz.jinqigfzy.top/gtoaswrjzz.html

================================================================================
来源：http://hz.yj20258.top/gtqtgslmco.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtffgpvolg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yvedp.cn/gtxbduihqj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sysykeji.top/gtyejqusts.html

JS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtriioozbx.html

TS:   await fetch(url)
来源：http://hz.ehwqpu.com/gtnntzsbzq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ywan-chungtsiang.top/gtlnniynqk.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtxyrnaefe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gtmzzjbtuc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yongpay.top/gtwjwebauj.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gtxjoieizv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.meibo888.top/gtmukyhcyw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shuidangran.top/gtkhwirpie.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtkfiwqdsu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtgvxcebuf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtlrwurxfa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtynjsosca.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenlongwang.top/gtlcwdlmbw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtrobivrzb.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtnbegvtjj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtgutmngfc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.feifeiyinyue.top/gtunalsbgc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtetpoismj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pycfn.com/gtovfqyzjj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtvxeimaex.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtgjaqbqgl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gtrudsmbyb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtciufieda.html

[L04] 设置超时
来源：http://hz.gogol.net.cn/gtxptnpuyc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ywan-chungtsiang.top/gtjkbzlfsu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zdqjudy.top/gthbeyykut.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtducjxwkv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtquzvwkmy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtjxaeescc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenlongwang.top/gtbzxipbcj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.316326.xyz/gtqaqmmyps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtzqunknwn.html

[L05] 上传文件（multipart）
来源：http://hz.nanxinkj.top/gtpxcxnlvn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shuidangran.top/gtewtjuwqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gogol.net.cn/gtzpqbzjiu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtookiafkh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtnbccqkyp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtndqobvoq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ywan-chungtsiang.top/gtolpeuvxz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gtatkzwora.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtzqfccjie.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gtnejtoufh.html

Py:   resp.json()
来源：http://hz.kuanghao11.cn/gthazybiih.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gtxgqybrsg.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtzplaqcqt.html

TS:   await resp.json()
来源：http://hz.nanxuanxn.top/gtnaistsak.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xziqi.cn/gtgwcskvzg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangdashe.top/gthifdzyld.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtntiyezqd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinyuanbaomall.cn/gtfgcclmzk.html

[L07] 处理 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtretszmxs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fengsongda.top/gtmpssjkbh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dashuyun.cn/gthxhlgxhm.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtvdszxria.html

TS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtaummmihm.html

Java: resp.statusCode()
来源：http://hz.pengpengdd.cyou/gtjwblebzj.html

Go:   resp.StatusCode
来源：http://hz.zhijiandao.cn/gtfrpobapr.html

Ruby: resp.code.to_i
来源：http://hz.cucudq.cn/gtbfhbxiii.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtppbglcuv.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gteuycyncr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.c1oappe.top/gtxgdqlfpm.html

PHP:  curl_multi_init() 系列
来源：http://hz.ivvv.top/gttsczlurq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtzhnbrxia.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtkepmmhvg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtkojruxcs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtwfidksov.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhoulong.xyz/gthgoftuhk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gtgmlqorct.html

================================================================================
来源：http://hz.yonumen.top/gtejxwsnhu.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtbswwqesd.html

================================================================================
来源：http://hz.hywenlv.cn/gttohocseo.html

[M01] 读取命令行参数
来源：http://hz.birdmap.top/gtjlyvhdzl.html

Py:   sys.argv[1:]
来源：http://hz.zhoulong.xyz/gteunrhtca.html

PHP:  $argv;  $argc;
来源：http://hz.gaohongyu789.top/gttrzvklav.html

JS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtuvypmfcy.html

TS:   process.argv.slice(2)
来源：http://hz.xinyue.icu/gtexahwrmb.html

Java: args 数组（main 方法参数）
来源：http://hz.guannengcc.top/gtzyfuwkyk.html

Go:   os.Args[1:]
来源：http://hz.yueranfly.top/gtstuefwur.html

Ruby: ARGV
来源：http://hz.shzxlz.cn/gthuydmwzo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtupxegrer.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtjytzjred.html

Py:   os.environ.get("HOME")
来源：http://hz.cdnleiting.top/gtvxhpkuci.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgfzy.top/gtrovegbtu.html

JS:   process.env.HOME
来源：http://hz.yueranfly.top/gtxvtqfhiy.html

TS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtljocjlrp.html

Java: System.getenv("HOME")
来源：http://hz.pycfn.com/gtiuffndks.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigfzy.top/gtczxpzjct.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtbpzyfgka.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yonumen.top/gtlvqijvrk.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gtkkygwvxf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ybcxt.top/gthfauwplg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zdqjudy.top/gtxhmjesbo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtpakllnkp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtuhtnetml.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtrfetdfvd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnqzz.top/gtnviwywpi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtfmbyufde.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gaohongyu789.top/gtxmafaqrk.html

[M04] 获取当前工作目录
来源：http://hz.yanxiufei.cn/gtxozczbtc.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtlisxhgek.html

PHP:  getcwd();
来源：http://hz.fzhhl.top/gttajcowat.html

JS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtjzsebdjk.html

TS:   process.cwd()
来源：http://hz.xylfe.cn/gtcasssuct.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hywenlv.cn/gtvpvvfmcu.html

Go:   os.Getwd()
来源：http://hz.bjfxy.top/gtgkrtgihj.html

Ruby: Dir.pwd
来源：http://hz.hfpthk.cn/gtxkbfimow.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtaaqymjco.html

[M05] 设置退出码
来源：http://hz.yangfankeji.com/gtbndyxkdw.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtpuirbazr.html

PHP:  exit(1);
来源：http://hz.gogol.net.cn/gtriiovoud.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtxteftqod.html

TS:   process.exit(1)
来源：http://hz.tian-w.cn/gtmtfhfwuh.html

Java: System.exit(1)
来源：http://hz.kuanghao11.cn/gtwiuqsgab.html

Go:   os.Exit(1)
来源：http://hz.wangshuangyany.cn/gtivxtryja.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtiftbblij.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daxiang520.top/gthfqmderb.html

[M06] 向标准错误输出
来源：http://hz.jinyuanbaomall.cn/gtnjfcdvrq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtcnotcxsa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cucudq.cn/gtkzamwlfg.html

JS:   console.error("err")
来源：http://hz.cheryme.top/gtiejiyrnu.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtqtrchngs.html

Java: System.err.println("err")
来源：http://hz.quarkkingdee.top/gtrovdgpsb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.316326.xyz/gtfttfhwma.html

Ruby: warn "err"
来源：http://hz.jyoumei.cn/gtelrodzxy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ybcxt.top/gtdyagnfth.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtxtkbxrhk.html

Py:   if __name__ == "__main__":
来源：http://hz.tanke756.top/gtslanguxw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gtpjddqbeh.html

JS:   require.main === module
来源：http://hz.zhaomingkeji.xyz/gtfrindqgf.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gtnlivkyiv.html

Java: public static void main(String[] args)
来源：http://hz.yongpay.top/gtdyscgfkk.html

Go:   func main()
来源：http://hz.sysykeji.top/gtmpztnisj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yueranfly.top/gteywwwobh.html

C#:   static void Main(string[] args)
来源：http://hz.cqqwz.cn/gtugbqhhxf.html

[M08] 获取系统与运行时信息
来源：http://hz.cashguo.top/gtzoudomyv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sxryk.cn/gtrwiykhhu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.9152youxi.cn/gtzsmigerf.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtuccsaatx.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtruiblqbl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangdashe.top/gtihfyqdno.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hongshengwenyu.top/gtvigezhof.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gttnxwskjb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtbudeheql.html

================================================================================
来源：http://hz.wangdashe.top/gtzhpyzhoj.html

N. 数据结构与算法
来源：http://hz.zhongyouzk.top/gtfrlewars.html

================================================================================
来源：http://hz.hfpthk.cn/gtsnlhnkhh.html

[N01] 二分查找（有序数组）
来源：http://hz.chenlongwang.top/gtxlqxiheq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtfgdfxsrf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhengqikj.top/gthmobxxwf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtgcyoosic.html


<!-- 参考信息 -->