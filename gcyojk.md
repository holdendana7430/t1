代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258.top/gtcjcvmivc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinyuanbaomall.cn/gtzgxtedmw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258.top/gtmngmooch.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtxpgdedwf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.havefunace.top/gtlqnwifyf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sweek.top/gtqhpogapv.html

[J05] 时间加减（加 7 天）
来源：http://hz.jyoumei.cn/gteheluoph.html

Py:   now + timedelta(days=7)
来源：http://hz.shzxlz.cn/gtygvkcwsy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtozrtonhd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtrarcflex.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtcwsjrsnx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtyakfnypm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nwbrower.top/gtobjcnhvz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gtvcijbcut.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtprtztcke.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtlfoawsns.html

Py:   (end - start).total_seconds()
来源：http://hz.guannengcc.top/gtieusgybj.html

PHP:  $end->diff($start)->days;
来源：http://hz.quarkkingdee.top/gtgqrtcbob.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gtckhrwppf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtfvnnfech.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhixingplan.top/gtyrgaepyg.html

Go:   end.Sub(start).Hours()
来源：http://hz.jyoumei.cn/gtywsdarkd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jiagoushi.top/gtqjwlbxjr.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtodtdaonk.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gtstyudmjl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtlvtjjxvt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gtcgoyzbuw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtkablegnk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gtderyvpen.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigfzy.top/gtwkiibmvz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gtpdpnqazq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtbkewzduo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtwpbavero.html

[J08] 提取年月日与星期
来源：http://hz.xuetiantiany.cn/gtytdqcmqq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtcqqproim.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gteuobdnsk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cheryme.top/gtnsvbybxs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gtedwmkntx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hfpthk.cn/gtoscthead.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtlnfvxmos.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtrpzrmonn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtjfaucyrt.html

[J09] 时区处理
来源：http://hz.redwolf501.top/gtuolhaiyi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtyfdslpsg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dashuyun.cn/gttqopjaah.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtuadvkwwt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gthbfnsnpq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtduggtbnl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtcibpeefw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gthrfezgei.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtrsbwphyj.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtbunrlgpy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dashuyun.cn/gtbgztqbrd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtbvrqvqhj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.andypj.xyz/gtvrorzzfe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhongyouzk.top/gtslwesjmv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtupvzudrf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtnlzlqcqg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gtnsytfxrf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gthnwvafaw.html

================================================================================
来源：http://hz.hammf.cn/gtcswlscxx.html

K. JSON 与序列化
来源：http://hz.daxiang520.top/gtjcdhgnna.html

================================================================================
来源：http://hz.mhx1999.top/gtllgqoicw.html

[K01] 对象转 JSON 字符串
来源：http://hz.vqdsnc.cn/gtikagbenl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtvpdelesv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtsbeprika.html

JS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtjbmyfvrs.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtoylizbpt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yangfankeji.com/gtabljsybe.html

Go:   json.Marshal(obj)
来源：http://hz.cdnleiting.top/gtjmwfqhto.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtuhrfnlkf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.smart0.xyz/gtffpapmxk.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtxifusbdr.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtrdsnuhle.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtemrjknwu.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtiahoojzb.html

TS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtobodygye.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtklngzkwr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtdtolkuwz.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtjsvffngn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtciupfzlj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ehwqpu.com/gtziqegwuw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gthxixhucf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtipupocek.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtpyfgedjy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtguwmkdob.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtjkdjovde.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtyemdbmsz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtfzxyiliw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinghuilouyu.cn/gtdpwgmmkx.html

[K04] 读取 JSON 文件
来源：http://hz.xylfe.cn/gtgvmkcyyt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtnlcnepyh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.iojbl.cn/gtrsitaknn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtqihvmdma.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtyejojyrp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtvhzyvlwr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtdicyckhz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtlbzsusjb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.havefunace.top/gtztvumpkw.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gthubmrszm.html

Py:   copy.deepcopy(obj)
来源：http://hz.jyoumei.cn/gtftekqbhl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gthmdxasmr.html

JS:   structuredClone(obj)
来源：http://hz.ydjk.org.cn/gtyhqjktpr.html

TS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtfzwoygmi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ppjwa.cn/gtwuroavak.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.haohaochexian.top/gthrpikuqn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gtjmeexifl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hongshengwenyu.top/gtrryjbysi.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gttpzzoacb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tianlin.xyz/gthdmdppep.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangshuangyany.cn/gtrhkrruka.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtpdrlfoja.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtvqczibyr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guannengcc.top/gtlrnlxdya.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zdqjudy.top/gtqszbuoyn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtifcwvheo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtrgztloej.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gttjsijpzl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigufen.top/gtawhkwjmp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtnawpkrac.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtlqgkxaxw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtcsctqvpi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtdgoeiwta.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtrujujcej.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydzc1.top/gtsrcuzouq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shangyingyoupin.top/gtrofxpbhi.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenlongwang.top/gtmmydefol.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gttltdxrds.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuxming.cn/gthhjrfygq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtcdtfizvt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtokkndxzf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yanxiufei.cn/gtofdqmxoz.html

Go:   encoding/gob
来源：http://hz.9152youxi.cn/gthvaxsbqv.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gttuantthd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fzhhl.top/gtjdywokhy.html

================================================================================
来源：http://hz.xuanzx.com/gtrgegpopv.html

L. 网络请求
来源：http://hz.xinyue.icu/gtkltgqolk.html

================================================================================
来源：http://hz.52xcode.cn/gtsabbduqz.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtulezrchf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtvfpvzpcb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj202588.top/gtcbeptgda.html

JS:   await fetch(url)
来源：http://hz.xuanzx.com/gtjpohggzk.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtzzqxjgcl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.birdmap.top/gttuqhqzxx.html

Go:   resp, err := http.Get(url)
来源：http://hz.yanxiufei.cn/gtigfnfgqr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guannengcc.top/gtkzacgtbp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigufen.top/gtkmymktxd.html

[L02] 发送 POST JSON
来源：http://hz.316326.xyz/gtjslxpruc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xziqi.cn/gthwqprmag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yj20258.top/gtzcrcjvct.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtmdnwpsqp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtmtkduqgj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aibaodan.cn/gtkpknzxiv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangkeji.top/gtuuyeefgs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtbrsradnb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtsdarvqzr.html

[L03] 设置自定义请求头
来源：http://hz.hammf.cn/gtjfbwxxve.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtyscdgtif.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hammf.cn/gtpupiiwxm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtueqrjcms.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtqrndccex.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shuidangran.top/gtqjxksxbc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.redwolf501.top/gtmoecmjzi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gogol.net.cn/gtqtqntjig.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtvbfwqguc.html

[L04] 设置超时
来源：http://hz.chenlongwang.top/gthrnpdpmx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtxdjrulre.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gtkuviylem.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtopjppjop.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtzivcxmgy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtjcuhmhal.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gtctityflv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtdvcrtqmw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhengqikj.top/gtxbqsohlp.html

[L05] 上传文件（multipart）
来源：http://hz.mhx1999.top/gtiajxcovv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtswulvvrs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtlkngsjmv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtsjvwamhb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtzgaeopvy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daria6918.cn/gtqvwtbiiy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenzaomai.com/gtxuakgedw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtajlkctli.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtbgytzsem.html

[L06] 解析响应为 JSON
来源：http://hz.xuanzx.com/gtezoncjij.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtkegtnfuf.html

PHP:  json_decode($body, true);
来源：http://hz.shangyingyoupin.top/gtjujrbqeo.html

JS:   await resp.json()
来源：http://hz.tianlin.xyz/gtnsvhwxxk.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtuusmgsuc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhengqikj.top/gtxxoytjdo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hammf.cn/gtmyihyzcu.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gtltwlpogj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zycfv.cn/gtkgmelflc.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtaljvasve.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtokxtjwzr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtxrqwstuy.html

JS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtsmgdhcou.html

TS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtvmadxpta.html

Java: resp.statusCode()
来源：http://hz.jinqigfzy.top/gtreqyyruy.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtnhtwdjbq.html

Ruby: resp.code.to_i
来源：http://hz.xinyue.icu/gthtzydtuc.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtjnktcmlg.html

[L08] 并发请求多个地址
来源：http://hz.vqdsnc.cn/gthwygoyik.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258888.top/gtrljwobey.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtdcbyuttu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gttmfikvss.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tanke756.top/gtodhnaoog.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cucudq.cn/gtohmfahcy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtdgwuhzjp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtobxrhbmg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.316326.xyz/gtndttzjqn.html

================================================================================
来源：http://hz.cucudq.cn/gtynjnckpi.html

M. 命令行 / 进程 / 环境
来源：http://hz.dianchejie.cn/gtctnfszwf.html

================================================================================
来源：http://hz.guowangkeji.top/gtylwutwzr.html

[M01] 读取命令行参数
来源：http://hz.yanxiufei.cn/gtaselyver.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gthsyhlktz.html

PHP:  $argv;  $argc;
来源：http://hz.smart0.xyz/gtmtbyetew.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtxvxxehxw.html

TS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtqnkkcvxj.html

Java: args 数组（main 方法参数）
来源：http://hz.316326.xyz/gtckbgjthc.html

Go:   os.Args[1:]
来源：http://hz.yanxiufei.cn/gtcxeeqhca.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtacdnsote.html

C#:   args 数组（Main 方法参数）
来源：http://hz.iojbl.cn/gtffgwwjzv.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtzjmakiav.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gtcindhhte.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.gzhubu.top/gtjeifnfbm.html

JS:   process.env.HOME
来源：http://hz.ydjk.org.cn/gthhynabsr.html

TS:   process.env.HOME
来源：http://hz.tian-w.cn/gtvlcucqlb.html

Java: System.getenv("HOME")
来源：http://hz.jianghu66.top/gtpaoeykcb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guowangkeji.top/gtzpkbyiyz.html

Ruby: ENV["HOME"]
来源：http://hz.xinyue.icu/gtqvrncasi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtfjiqqlaw.html

[M03] 执行外部命令
来源：http://hz.jinqigufen.top/gtbdzjcwxf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtzyjlfqgu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtskpnxkhf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gtpphzdtqm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtyhvkueqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtsepeamxx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhijiandao.cn/gtztmmfebm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hfpthk.cn/gtugjqkzuz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigfzy.top/gtxhyyuehk.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gtsornldld.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtdqfppvjk.html

PHP:  getcwd();
来源：http://hz.ydzc1.top/gtocwphbtq.html

JS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtwsswxmsn.html

TS:   process.cwd()
来源：http://hz.shzxlz.cn/gtsdqrgkgt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shzxlz.cn/gtjdzsgeoq.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gtecfutqjv.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtzcatgtaf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yongpay.top/gtkholxsfx.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtbppjiixa.html

Py:   sys.exit(1)
来源：http://hz.chenzaomai.com/gtpkrwfvye.html

PHP:  exit(1);
来源：http://hz.jinyuanbaomall.cn/gtyqqhfyef.html

JS:   process.exit(1)
来源：http://hz.redwolf501.top/gtazxlwwtn.html

TS:   process.exit(1)
来源：http://hz.gotoacloud.top/gttrlpssie.html

Java: System.exit(1)
来源：http://hz.ydjk.org.cn/gtohlliszb.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtwkzqbncj.html

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtpggnucyp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gtwshzlxui.html

[M06] 向标准错误输出
来源：http://hz.chenjidiqi.icu/gtvdvrnrsy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yonumen.top/gtrlluhxyy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cdnleiting.top/gttsddzihh.html

JS:   console.error("err")
来源：http://hz.yuanzhike.top/gtghlcsshg.html

TS:   console.error("err")
来源：http://hz.daria6918.cn/gtciuwhmdh.html

Java: System.err.println("err")
来源：http://hz.jqgfzy.top/gtitvmpquu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xuetiantiany.cn/gtplvepwox.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtizegigbj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cucudq.cn/gtlmddelgi.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gtbtaoipix.html

Py:   if __name__ == "__main__":
来源：http://hz.jqgufenzy.top/gtmevinbgw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gthckgmela.html

JS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtjhpsryho.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtrqzexrur.html

Java: public static void main(String[] args)
来源：http://hz.yvedp.cn/gtjzflrykz.html

Go:   func main()
来源：http://hz.ppjwa.cn/gtalllclco.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gtmpzvgwgi.html

C#:   static void Main(string[] args)
来源：http://hz.yangfankeji.com/gtoljicuxj.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gtrkjfjfic.html

Py:   platform.system();  platform.python_version()
来源：http://hz.vqdsnc.cn/gtmxtotlsj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jinqigfzy.top/gtonbucgvl.html

JS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gtaneqowyy.html

TS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtylcdjjto.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sufxvd.cn/gtrjassave.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jiagoushi.top/gtrjvtvewq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tianlin.xyz/gtwadmairg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.c1oappe.top/gtzxcksyjv.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfuvoseaz.html

N. 数据结构与算法
来源：http://hz.yuxming.cn/gtmgldnwjh.html

================================================================================
来源：http://hz.svipenyu.cn/gtsgnffqin.html

[N01] 二分查找（有序数组）
来源：http://hz.haohaochexian.top/gtwbndrmjp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.meibo888.top/gtxtpfyngb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtyagcjakw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtnkhjfcjt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtteexhlmk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtzzdovdhc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtwmiaemcj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.52xcode.cn/gttobmwujf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.andypj.xyz/gtvirnvunj.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.9152youxi.cn/gtifgfwjly.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhoulong.xyz/gtdfmaddgg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.gogol.net.cn/gtnzbulalq.html


<!-- 参考信息 -->