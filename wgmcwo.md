代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnqzz.top/gtzsaxvaha.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.quarkkingdee.top/gthkucxrsd.html

[J05] 时间加减（加 7 天）
来源：http://hz.sufxvd.cn/gtwsptooel.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtcparpfof.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gthvnqfpzd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtnrhvvgvg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtovirscbv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gttkaxuhxi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtyiuxdphu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtnnxfhlrl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtzxqxsyzj.html

[J06] 计算两时间之差
来源：http://hz.yj202588.top/gtubinnbab.html

Py:   (end - start).total_seconds()
来源：http://hz.zhiwuduotai.top/gtlryjttsj.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtbxhyzoxx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtencusksf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.smart0.xyz/gtpawaoctm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtarteemjz.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuetiantiany.cn/gtibywzzia.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sweek.top/gtyelozdim.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhiwuduotai.top/gtfeghssoj.html

[J07] 比较两个日期
来源：http://hz.hammf.cn/gtiivahvqn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtxksyvwml.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtkihtvzou.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtzblidngw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtjgoejuns.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydjk.org.cn/gttmpqjzgz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aizwys.cn/gtktuvmxbe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtioyndgwa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gthkgstjgk.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtkthdcjgv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtciavfjqc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangkeji.top/gtzvoalexd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xylfe.cn/gtbsrvtljq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtmwroopcz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gthgzalivh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuxming.cn/gtdeqhmwek.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhixingplan.top/gtwfyzbcln.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gtxpgthhvo.html

[J09] 时区处理
来源：http://hz.wangshuangyany.cn/gtmldvebnk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xinyue.icu/gtbdfhlgqh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtizwonmdc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtzfvhkpph.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gthkxbwqlw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtcghjkici.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhaomingkeji.xyz/gtcymnkkjr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gtyyaqubjf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yongpay.top/gtaaxnhath.html

[J10] 取今天 / 本月第一天
来源：http://hz.aizwys.cn/gtfdwhrmcz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtjuiaqxvv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtjznusxpo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtidzwsflf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xinyue.icu/gtqaduovaf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhixingplan.top/gtwuuduzvy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtbeedgytv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.smart0.xyz/gtfwbverwk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gtrpzbgxjd.html

================================================================================
来源：http://hz.jyoumei.cn/gteyqkxvzt.html

K. JSON 与序列化
来源：http://hz.sysykeji.top/gtxzwojzrc.html

================================================================================
来源：http://hz.hysaishi.cn/gtntvwngjb.html

[K01] 对象转 JSON 字符串
来源：http://hz.gogol.net.cn/gtjemybedo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtxtmfuhcc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtywsudizo.html

JS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtiiexhurg.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtdvqgkkys.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gtrkjeznvt.html

Go:   json.Marshal(obj)
来源：http://hz.aizwys.cn/gtsavwwurq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ehwqpu.com/gtgvgjhqyo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtkvlgmhog.html

[K02] JSON 字符串转对象
来源：http://hz.feifeiyinyue.top/gtgsfsvniy.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtcehkueua.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigfzy.top/gtzzxbfugi.html

JS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtmhblvbca.html

TS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtvqneqgil.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhaomingkeji.xyz/gtdaohlpkj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtflilfwoy.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gteqzeoypi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtefopjjxh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhaomingkeji.xyz/gtcnwqhoir.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtkwtnyfbz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtcfaktdyc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtfcueswnq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtivtgfmar.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtgpbtxril.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtplzgdxnh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenzaomai.com/gtyzaxhqxq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.kuanghao11.cn/gtedlybiyg.html

[K04] 读取 JSON 文件
来源：http://hz.shanyushiyangtech.top/gtamescmsd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gtuwbsofvq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxinkj.top/gtknqluuas.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtbvoovnhd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtkzdbxxyd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dashuyun.cn/gtfdehrdjp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtdfcecepw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtkbozyzds.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtgatkiiqv.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gtwhcuyanr.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtcnusydlj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtkrmxsrim.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtplzaplfj.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtgdxmzngl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xingfuxueyuan.xyz/gtjrrbfrct.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.52xcode.cn/gtzwlvhtkb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtjwxoffcp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtoqdfiryq.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtsjliuiip.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtdgaeueuw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cqqwz.cn/gtbzntezfz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtvyngkihl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtworputfb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtlqwhbctv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtyynwuaae.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gtiioeykhe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtcurtfwou.html

[K07] 进制转换
来源：http://hz.jqgufenzy.top/gtljhnusnj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gtwvecxnta.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xziqi.cn/gtasoqdwyb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yongpay.top/gtpiqgunuk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtuqmtwpdf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtdddkqhlw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtzpdvtocj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hywenlv.cn/gtxghkacqn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtytxpqjgk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guowangkeji.top/gtbobuhvnd.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtfbplchzg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.mhx1999.top/gtukoyubih.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtcyieyujq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtfgnedczl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtimriqqyn.html

Go:   encoding/gob
来源：http://hz.guowangkeji.top/gtadxlbzfr.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gtwwisnnvb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hysaishi.cn/gtndscxode.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsqscbtji.html

L. 网络请求
来源：http://hz.yuxming.cn/gtcprixfqs.html

================================================================================
来源：http://hz.daxiang520.top/gtpzhjitzj.html

[L01] 发送 GET 请求
来源：http://hz.zhiwuduotai.top/gtwhhyrnpy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtelnsjlnq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtgmcppwgx.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtkjirbmyb.html

TS:   await fetch(url)
来源：http://hz.daria6918.cn/gtqgxoiuzw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtnbsskwse.html

Go:   resp, err := http.Get(url)
来源：http://hz.hywenlv.cn/gtnzitlgrf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.tanke756.top/gtsttgxbvs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jlsjyb.cn/gthatrmbmz.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gthdhaoqxl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuanzhike.top/gtwkbfmsdj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgufenzy.top/gtoytgtged.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtjougyayt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.52xcode.cn/gtbpjlhhmo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tianlin.xyz/gtqznumrpo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtnwyfykzy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtuxjafozs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gtsjalkbst.html

[L03] 设置自定义请求头
来源：http://hz.jqgufenzy.top/gtewmnxlaj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jiagoushi.top/gtizqawtuy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.mhx1999.top/gtokzprepu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtnylbpssl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtlxpxjnop.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenzaomai.com/gttylhraaz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gthmgikuzh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ydjk.org.cn/gtcofwofzn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtjlrwpajq.html

[L04] 设置超时
来源：http://hz.yj202588.top/gtvgdchuce.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtgjekaire.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gtrxlbnflq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtpbpsugye.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtfadsetkr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.mhx1999.top/gtinelrxoa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtaxcttnlh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guowangkeji.top/gtzgqbsgka.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigufen.top/gtxdasvnod.html

[L05] 上传文件（multipart）
来源：http://hz.xziqi.cn/gtfjyuubpo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cucudq.cn/gtgwyxhfbg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtefubxstt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtogpwixor.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtweypsxmg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhijiandao.cn/gthoyzajgw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.bjfxy.top/gtlrrfkqrf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtvgkptjeg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.haohaochexian.top/gtdxmmitxr.html

[L06] 解析响应为 JSON
来源：http://hz.smart0.xyz/gtrtweykgl.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gtezxhauca.html

PHP:  json_decode($body, true);
来源：http://hz.feifeiyinyue.top/gtbmwmrouj.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gtvcrwyish.html

TS:   await resp.json()
来源：http://hz.hnqzz.top/gteugxzhpt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenjidiqi.icu/gtnbgtbypk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtvqzfvdxd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtzkqljnep.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinyuanbaomall.cn/gtbmgwwctq.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuxming.cn/gthddntbhy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dashuyun.cn/gtlfxxiigx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yongpay.top/gtqwlrlfxd.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtcquyffzg.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtmnqjfynu.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gtcvzydhpo.html

Go:   resp.StatusCode
来源：http://hz.fengsongda.top/gtdtbrswvz.html

Ruby: resp.code.to_i
来源：http://hz.52xcode.cn/gtaebdacdd.html

C#:   (int)resp.StatusCode
来源：http://hz.yueranfly.top/gtftwarkch.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gtwprhtyon.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtkwterzhk.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gttaqkkslt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pycfn.com/gtmnfvchga.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtjzscrezs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtcofukoea.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gtsoidnjvw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gthiyfroiz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nwbrower.top/gtldodhtnd.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtoeufhslq.html

M. 命令行 / 进程 / 环境
来源：http://hz.shzxlz.cn/gtpjnnceve.html

================================================================================
来源：http://hz.shuidangran.top/gtewcfguzn.html

[M01] 读取命令行参数
来源：http://hz.daxiang520.top/gtetpgqfze.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtvtaghrgt.html

PHP:  $argv;  $argc;
来源：http://hz.ydjk.org.cn/gthncrckwn.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtvmeluitq.html

TS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtvauwwcwu.html

Java: args 数组（main 方法参数）
来源：http://hz.yanxiufei.cn/gtwgweajtw.html

Go:   os.Args[1:]
来源：http://hz.quarkkingdee.top/gtutaaowle.html

Ruby: ARGV
来源：http://hz.cqqwz.cn/gtetgjtjuj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtnygqkrgz.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtnrbzyalj.html

Py:   os.environ.get("HOME")
来源：http://hz.ydjk.org.cn/gtwzwgcgef.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtzvrqwyff.html

JS:   process.env.HOME
来源：http://hz.sxryk.cn/gtxpathwmq.html

TS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtjummpimk.html

Java: System.getenv("HOME")
来源：http://hz.ehwqpu.com/gtflxsamok.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtjloqeptr.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtprpgarfp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtgqpdnmil.html

[M03] 执行外部命令
来源：http://hz.hammf.cn/gtsslmnqrq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cdnleiting.top/gtybpjagjr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gtbnodalcy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtdjbkibpw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtaberpkrw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pengpengdd.cyou/gtjilcznpw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtiksfpbik.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtfxueflwc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gotoacloud.top/gtumqqjapd.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtaqrxxgvn.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtjpczhqyh.html

PHP:  getcwd();
来源：http://hz.zdqjudy.top/gtdpmjefft.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtwixsgdvv.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtgrigiwxi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigfzy.top/gtzgysytfq.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gtjcfbskoz.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gtcqusupoc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgufenzy.top/gtonqzjwjt.html

[M05] 设置退出码
来源：http://hz.yongpay.top/gtznzmynoc.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gtvzxtjnuu.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtwziwdkpj.html

JS:   process.exit(1)
来源：http://hz.tanke756.top/gtmcrrcnkb.html

TS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtrynzfjyj.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtvjspioel.html

Go:   os.Exit(1)
来源：http://hz.gaohongyu789.top/gtawjhpurj.html

Ruby: exit 1
来源：http://hz.0kj1m.cn/gticqgusdp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cqqwz.cn/gtmjqyglcu.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtzwyitaqk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gttutflgca.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sxryk.cn/gtaekfuybx.html

JS:   console.error("err")
来源：http://hz.xuanzx.com/gtbhjxqsjj.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtehirfdkn.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gtnadzcfze.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxinkj.top/gtisnunqpn.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtxolvyawv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gzhubu.top/gtbztuuqbn.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtagpsxjlv.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtsdikvtsl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gtjbtytyrd.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtviwqgvfo.html

TS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtqwfbmjzv.html

Java: public static void main(String[] args)
来源：http://hz.jinqigfzy.top/gtrbpvnttw.html

Go:   func main()
来源：http://hz.c1oappe.top/gtpqdurisb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtuhwgxynk.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtizepojzw.html

[M08] 获取系统与运行时信息
来源：http://hz.ydjk.org.cn/gtmffbxjjn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtjqcxzpzg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhoulong.xyz/gtekenjvdk.html

JS:   process.platform;  process.version
来源：http://hz.guowangkeji.top/gtfaujwkwv.html

TS:   process.platform;  process.version
来源：http://hz.yongpay.top/gtkuqpwuoy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fengsongda.top/gtnttjmeyz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gtwdohcohk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtezatwafc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.jyoumei.cn/gtxhhnbexk.html

================================================================================
来源：http://hz.iojbl.cn/gtkdadzcus.html

N. 数据结构与算法
来源：http://hz.jinyuanbaomall.cn/gtewvlxtox.html

================================================================================
来源：http://hz.hywenlv.cn/gtjktrbaty.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtvxqyyhpv.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtzfydhyrr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnxiangtu.top/gtvuitacrx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gthhdgofjh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtquifocgo.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtijhmlixd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.mhx1999.top/gtukgkdlqi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtbettmfoq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sysykeji.top/gtsqarrbsg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtoohlauef.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nwbrower.top/gtpsdkewac.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aibaodan.cn/gtfodyhovm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtydczctmc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yvedp.cn/gtdmdaainq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yvedp.cn/gtapkczzhm.html

Go:   slices.Sort(arr)
来源：http://hz.iojbl.cn/gtcmrknvpx.html


<!-- 参考信息 -->