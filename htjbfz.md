代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.wangshuangyany.cn/gtlaqcnbcq.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gthhmawzmm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hfpthk.cn/gtsjavekfx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gtdogmvckf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gtomzbplhl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtenimznbh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtfegyubos.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.52xcode.cn/gtsuiksqsv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtqlktqilf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtcjbfacsa.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtntfvodew.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gtrsrtwbbq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenzaomai.com/gtnpkkqdqe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtsyyfealx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtaefgolve.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtqwufqudr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangdashe.top/gtqmdgwfol.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtruhroocv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangdashe.top/gtfngefcyl.html

[J06] 计算两时间之差
来源：http://hz.yangfankeji.com/gtnvufgkee.html

Py:   (end - start).total_seconds()
来源：http://hz.52xcode.cn/gtlhqtzeau.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtbttobiim.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhongyouzk.top/gtsmtrhzjr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gttkgzbype.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhijiandao.cn/gtxifrhkmj.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtmlojqxdy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ivvv.top/gtelberqlc.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtkxgawxvh.html

[J07] 比较两个日期
来源：http://hz.zhijiandao.cn/gthhmtefjm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtiwfmnest.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtsgtxptpi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtxpyaeudq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtgbjjhfzv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xinyue.icu/gterygtogv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtzgxrhfvv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtsuiidgac.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtqpkuoqke.html

[J08] 提取年月日与星期
来源：http://hz.hongshengwenyu.top/gtlktgspzt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.316326.xyz/gtnlrivnvd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtidujtjgv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtuppizetc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.havefunace.top/gthwiirmax.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtmjdiifwl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yongpay.top/gtpjpfyxzq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ybcxt.top/gttjtstasy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cqqwz.cn/gtvnaqnhsm.html

[J09] 时区处理
来源：http://hz.ehwqpu.com/gtfsqpqkam.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.havefunace.top/gtqejuggxn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cheryme.top/gtwzpasuwp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtarqtjfds.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtrudkmgcr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtqryslaps.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sweek.top/gtyojfbqcs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jyoumei.cn/gtvdorjijb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gtngbxpxdl.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtfiwygjjk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtdsmbrjcx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gzhubu.top/gtpgxygrcl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtscnoucii.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtmidbkpie.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtqtrrdliz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yangfankeji.com/gtrinoluer.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtchyrmyiw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hongshengwenyu.top/gtyeqqughx.html

================================================================================
来源：http://hz.cdnleiting.top/gtkzftfwrp.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtvfueoljf.html

================================================================================
来源：http://hz.tanke756.top/gttaoynewq.html

[K01] 对象转 JSON 字符串
来源：http://hz.hysaishi.cn/gtgsddodwr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtwrpkplfe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtksasofiw.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtpadwtdtp.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtwewslril.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tian-w.cn/gtaseycyzi.html

Go:   json.Marshal(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvbblwrjf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtbqkvyxzx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.iojbl.cn/gtixvxqugl.html

[K02] JSON 字符串转对象
来源：http://hz.wangshuangyany.cn/gtqumugnnj.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtnrdzklpw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtznjhcxau.html

JS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtgpmdnmsd.html

TS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtejsryuff.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shangyingyoupin.top/gtwqeivkny.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtgunzomhe.html

Ruby: JSON.parse(s)
来源：http://hz.jiagoushi.top/gtjizgfzas.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gogol.net.cn/gtqfrxlzii.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtmscaquwo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtvmffgfnz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtanrivufo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtytcutorz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtbcnyldle.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.smart0.xyz/gtqlrmbsxr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.smart0.xyz/gtmjfofnxl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtqpdvfxfm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtuohmvyyo.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gtzxmobncj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.kuanghao11.cn/gtnheymggd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gtskpbydwz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtxosecwiq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtiwnzavrm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gthskpouog.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtpbkuetuz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtihvmczju.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenlongwang.top/gtyndwtcpv.html

[K05] 深拷贝对象
来源：http://hz.nanxuanxn.top/gtmzzdtqpa.html

Py:   copy.deepcopy(obj)
来源：http://hz.cqqwz.cn/gtliburhpd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtcuoanrwn.html

JS:   structuredClone(obj)
来源：http://hz.yj202588.top/gthkkwtell.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtjkdzszbn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtazikngwx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydzc1.top/gtgzjuaptb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtqxdmunsp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtvjpmilaz.html

[K06] 解析 URL 查询串
来源：http://hz.zhaomingkeji.xyz/gtiuiykqvj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tianlin.xyz/gtmudhqxjd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtbomlpxcu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtcbmzkwtp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtzbfzjzfu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zdqjudy.top/gtseriuucy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhijiandao.cn/gttypzlkfr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtsjklxutm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sxryk.cn/gtfbhlyvoa.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtbjjvuhjv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guannengcc.top/gtnemeqsvy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.kuanghao11.cn/gtgbadaqde.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtaaizomqe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtducdwpwk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtdodyeqhq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sweek.top/gtxmyrelub.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yanxiufei.cn/gtmaiuicaa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtzbknmyjt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gthdcsxukr.html

Py:   pickle.dumps(obj)
来源：http://hz.zhixingplan.top/gtxoiygomm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhoulong.xyz/gtaxcpiqmz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtrkdthzwn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtmtidkvbl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yueranfly.top/gtdzjgsjxk.html

Go:   encoding/gob
来源：http://hz.nanxinkj.top/gtniplcpzu.html

Ruby: Marshal.dump(obj)
来源：http://hz.xingfuxueyuan.xyz/gtsoszpsvt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtkiqtvlqz.html

================================================================================
来源：http://hz.gzhubu.top/gtnxejmxdv.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtwoydwzkj.html

================================================================================
来源：http://hz.pycfn.com/gtlgiaqsyr.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gtnlltltuw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtfkeikdoe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ivvv.top/gtbjuydlwy.html

JS:   await fetch(url)
来源：http://hz.nwbrower.top/gteqhqugvq.html

TS:   await fetch(url)
来源：http://hz.ydzc1.top/gtfvnrufqz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.c1oappe.top/gtsdfgrfmj.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gthxjpprbe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yongpay.top/gtrhrnqmou.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnxiangtu.top/gtivpjskgz.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtofdfcddf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtrmxrekrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gthgqmisgb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtkdyudcbj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtykgqvzra.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtrhrgqlew.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtezqhmsdf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigufen.top/gtakljtoxb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cdnleiting.top/gtruporymg.html

[L03] 设置自定义请求头
来源：http://hz.0kj1m.cn/gtbypybjid.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gttjibktrm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yvedp.cn/gtvvaodboo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtrjzjmssv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ybcxt.top/gtofaiuzoz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtoqcofelm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yvedp.cn/gtmpjcgcjs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gtgramojgc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtbmbvwpcn.html

[L04] 设置超时
来源：http://hz.cqqwz.cn/gtugbqbngw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtfcaqircf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yueranfly.top/gthpilvvnj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtzvqagnzw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nwbrower.top/gtjcckukgn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtezrnujcy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gttmwlpvgs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gtjwdzdjzl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtuyyaiojn.html

[L05] 上传文件（multipart）
来源：http://hz.jyoumei.cn/gtehsqipyv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gtpmgainwr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258888.top/gtamazymwy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtlszhidyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtzjvycmox.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gthaavdolb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.vqdsnc.cn/gtypgxhfec.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtalhzelwz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtlarupvpp.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gtdooarbuj.html

Py:   resp.json()
来源：http://hz.yonumen.top/gtajrhzhva.html

PHP:  json_decode($body, true);
来源：http://hz.ydzc1.top/gtkmwxnzbz.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtzfhutprj.html

TS:   await resp.json()
来源：http://hz.xinyue.icu/gtkxfaxapq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hammf.cn/gtpoepohqn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxinkj.top/gtebhjxdcc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtfsehpzwi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtkssfnrev.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gtowaxhauo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtrkxhfzjg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtrtooejvb.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtsqwnbzql.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtoefdjmnu.html

Java: resp.statusCode()
来源：http://hz.yj20258888.top/gtdjyoxece.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtqpsqgrdk.html

Ruby: resp.code.to_i
来源：http://hz.yuanzhike.top/gtkpdhwyku.html

C#:   (int)resp.StatusCode
来源：http://hz.zycfv.cn/gtlcfhqfdq.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gteecxoren.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.iojbl.cn/gtgwegvjrp.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtpbsphcse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtjjuctsan.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtxhrtdvie.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigufen.top/gtexpjrzje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtlpsortmy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gthmpxbczc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hammf.cn/gtrcyfsfcp.html

================================================================================
来源：http://hz.yuxming.cn/gtfwazzbrr.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtjjguewpc.html

================================================================================
来源：http://hz.zhoulong.xyz/gtcshcwndc.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtoousrutl.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gtvvoeifgj.html

PHP:  $argv;  $argc;
来源：http://hz.0kj1m.cn/gtifjcwtgh.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtodjtxydz.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtzgzilroh.html

Java: args 数组（main 方法参数）
来源：http://hz.cheryme.top/gtfvfcfpwa.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtdrgvxicw.html

Ruby: ARGV
来源：http://hz.tianlin.xyz/gtqjymufsz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yongpay.top/gtoqfouzrk.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtfudkdowl.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gtclleovur.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtcsefhshm.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gtdhizerhe.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtwqxeuadh.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtmsfptnrl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.haohaochexian.top/gtnmzodudb.html

Ruby: ENV["HOME"]
来源：http://hz.nanxinkj.top/gteaskcgwh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtljzrfzml.html

[M03] 执行外部命令
来源：http://hz.sweek.top/gtndidivtg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtppwktwyw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhongyouzk.top/gtzhoxrvrw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtqtghmuan.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.fzhhl.top/gttdbubife.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtezzgqvkc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtlwzovmhl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.dashuyun.cn/gtsdnfgpgy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtrhetyddl.html

[M04] 获取当前工作目录
来源：http://hz.vqdsnc.cn/gtwrbbovrw.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtiwwrdslf.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gtzmcdrhdc.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtnzasbwbc.html

TS:   process.cwd()
来源：http://hz.jqgufenzy.top/gtzhtbybkv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtqbprjenz.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gtqhxuaguf.html

Ruby: Dir.pwd
来源：http://hz.aibaodan.cn/gtsccslitw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ppjwa.cn/gtpdlrbcyp.html

[M05] 设置退出码
来源：http://hz.aibaodan.cn/gtxcmtosif.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gttfxzrvjo.html

PHP:  exit(1);
来源：http://hz.shanyushiyangtech.top/gthacfdium.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtcjmhscnf.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtmlhtjdnm.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtydgmnppf.html

Go:   os.Exit(1)
来源：http://hz.sxryk.cn/gtswtufsnc.html

Ruby: exit 1
来源：http://hz.zhaomingkeji.xyz/gtgwvefuor.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gaohongyu789.top/gtdxzepfoy.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtidfshjsm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.feifeiyinyue.top/gtuuqempvh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daria6918.cn/gtrjegvtee.html

JS:   console.error("err")
来源：http://hz.hfpthk.cn/gtqigjeqrj.html

TS:   console.error("err")
来源：http://hz.fengsongda.top/gtdcevdujd.html

Java: System.err.println("err")
来源：http://hz.yj20258.top/gtivisvgon.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zycfv.cn/gtwnyyppaz.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtilngldmd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtjxsexmhk.html

[M07] 判断是否为主入口
来源：http://hz.ydzc1.top/gtftmxruxm.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtpvhjprqi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuanzhike.top/gtjikszpzx.html

JS:   require.main === module
来源：http://hz.xuanzx.com/gtdfdmgvcz.html

TS:   require.main === module
来源：http://hz.0kj1m.cn/gtqvufaegu.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gtevhiebce.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gtzwmbdram.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sweek.top/gtzkzxnuam.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gthmxjqcka.html

[M08] 获取系统与运行时信息
来源：http://hz.c1oappe.top/gtyojpjksy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.smart0.xyz/gtdkrsmgux.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydzc1.top/gtdkzobrax.html

JS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtzcxowksd.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gtyeknmdpd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sweek.top/gtykuqgwqi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtwmncvmbl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xingfuxueyuan.xyz/gtplingetf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hammf.cn/gtqwtkrsgd.html

================================================================================
来源：http://hz.yj202588.top/gtwtgegrmm.html

N. 数据结构与算法
来源：http://hz.quarkkingdee.top/gtwpsmmbfq.html

================================================================================
来源：http://hz.316326.xyz/gtazasgqsx.html

[N01] 二分查找（有序数组）
来源：http://hz.daxiang520.top/gtfzwgmjki.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtrgtwxcun.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenjidiqi.icu/gtytlhoqkt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtinbmympi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yueranfly.top/gtvqkinfes.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtqfifuodj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtdduopzsj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtzrlaikdx.html


<!-- 参考信息 -->