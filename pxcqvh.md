代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gteutvlela.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jianghu66.top/gtscngrgmp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtkzllgrnm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhoulong.xyz/gtxuwzfplv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtnkayfcwh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangtech.top/gthaunagod.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtjawgujmv.html

[J06] 计算两时间之差
来源：http://hz.ivvv.top/gtrztwsqbo.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtbglkurtc.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtpmrdavyr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.haohaochexian.top/gtupuejpyq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gttvegjklx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gthjtcwayx.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhengqikj.top/gtphamrjye.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gteidmafhi.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gtwtxqgugi.html

[J07] 比较两个日期
来源：http://hz.yuanzhike.top/gthuhvhjgb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtzzasqkhp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gtkypnbnea.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtbsurlxag.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtnqmepswm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gthfizilns.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gogol.net.cn/gtrczzdogi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gttxzgqryy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtbjxlrrqd.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtwzbcfppb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtqivixzbm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cheryme.top/gtzhvvhslu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gttjxbzykc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgfzy.top/gtvpeiwqiu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtokrxxzrq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtfpnnjode.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinyuanbaomall.cn/gthraxgqme.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtkztynpji.html

[J09] 时区处理
来源：http://hz.zdqjudy.top/gtopcexews.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhixingplan.top/gtpbcnugfl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtviydacxl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtcmdhokhd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtsbswqsre.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtgvfmltdw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jlsjyb.cn/gtunllbpmn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gttffitvfo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtsztzfthd.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgfzy.top/gtketckdys.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jyoumei.cn/gtzlbfqtwe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtznlzfnsr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gtbfnsesms.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtrfcqphah.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtckslcrxv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gtqqndnsme.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ivvv.top/gtgmjkpbnj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtodjxkpdx.html

================================================================================
来源：http://hz.yuxming.cn/gtrojdtaje.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtcamhokga.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtstlbbmha.html

[K01] 对象转 JSON 字符串
来源：http://hz.xinyue.icu/gtcodpdbuo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtofkcnxbc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gttvafcjdp.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtlbmobwje.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtdmvcgmqn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtazsnvmov.html

Go:   json.Marshal(obj)
来源：http://hz.zhongyouzk.top/gtzkmvrzjx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gthtxduqny.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cucudq.cn/gtrcvbhwce.html

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtvepoytqd.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtunsmsxgt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtdvmxgysc.html

JS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtodsimtxq.html

TS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtomkuzoyn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jlsjyb.cn/gtwrrioegy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtjswmiuks.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtftdtfkzw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtaodejvwe.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangdashe.top/gtxxsmxkbs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtoxgortjm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtuohkzcse.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtnwiwytkg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtnldpniiw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuetiantiany.cn/gtrwlhmrml.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.svipenyu.cn/gtbcjjvwph.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtxrhxpacp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gtwtzmqsit.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtxfzzcplu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtltwkceaw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtzfqmxhht.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daria6918.cn/gtyjkapoak.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtokfzrvsy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtvpqjwpcy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtqhyxdgcz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtzhzhmqwu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gttrouczvx.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtuxeinimu.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhixingplan.top/gtwukqcaem.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yonumen.top/gtefykfgms.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtotosoogj.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtemqrewcd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtsgxnojtu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtizpnfbst.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtysephpbs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hongshengwenyu.top/gtpjoriaqv.html

[K06] 解析 URL 查询串
来源：http://hz.gotoacloud.top/gtiuufqohc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gtksgkhkwf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtqhqcianh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtaympzmte.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtkoobicxz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gtzigjaybj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtmdtheffl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuanzx.com/gtddhyhhxk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtfopqfoiq.html

[K07] 进制转换
来源：http://hz.zhengqikj.top/gtetixumzs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gtkxncsheq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtbtfxpjai.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtwhghbeyo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtrcmkcwyr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtqqsgpmfs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtlrwpuafs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gthwtmaddk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gtvkmgwkdr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cqqwz.cn/gtgleblklo.html

Py:   pickle.dumps(obj)
来源：http://hz.hywenlv.cn/gtwrbqmtpx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tanke756.top/gtyxgwkmgb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtczjqpiuh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gtscmnhhmt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.kuanghao11.cn/gtiqmulviy.html

Go:   encoding/gob
来源：http://hz.havefunace.top/gtrzkxbjry.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtxkcmttvg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yangfankeji.com/gtfzjjajtg.html

================================================================================
来源：http://hz.fengsongda.top/gtdzustdjd.html

L. 网络请求
来源：http://hz.sweek.top/gtiwstdtxp.html

================================================================================
来源：http://hz.ydjk.org.cn/gterflfrhr.html

[L01] 发送 GET 请求
来源：http://hz.sysykeji.top/gtynhdnvpi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtfbgbmqpm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtxdsnhepv.html

JS:   await fetch(url)
来源：http://hz.aizwys.cn/gtuvaavehf.html

TS:   await fetch(url)
来源：http://hz.yonumen.top/gtplckrhbh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhengqikj.top/gtxhhtnawj.html

Go:   resp, err := http.Get(url)
来源：http://hz.tanke756.top/gthtnbqlkj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258.top/gtvgsltnmt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gtgmhoxlde.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gtqbckuyps.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hnqzz.top/gtpuwvmemk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gaohongyu789.top/gtristbuvw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtjieaxnas.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtussliqpp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtatszocjz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangtech.top/gtbcfnxxyn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.316326.xyz/gthbtiifek.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pycfn.com/gtcckkxolo.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtoqptadoj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtfglpklei.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtvhlxgcbl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtrytiziaq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtsphkwtmw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gtccadzqkc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ppjwa.cn/gtzzddjgdc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sufxvd.cn/gtcbbmlfjg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtqvfwsbok.html

[L04] 设置超时
来源：http://hz.jqgufenzy.top/gtivzoscxq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.redwolf501.top/gtwuslgsvc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtxclysmsj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtjnqbiwpv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtvjftoqag.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xylfe.cn/gtxgtkywna.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guannengcc.top/gtbqwiqdxl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gtykybjhoa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shuidangran.top/gtfyywfpfq.html

[L05] 上传文件（multipart）
来源：http://hz.dashuyun.cn/gtylsadiml.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nwbrower.top/gtglrupdhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cdnleiting.top/gtacnufrgr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtsdoolyix.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gttytkotgu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yueranfly.top/gtcaqfpsbx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xylfe.cn/gtfhqcntcz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guannengcc.top/gtrtlrinxc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fengsongda.top/gtluhhxifn.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangkeji.top/gtrrxvohre.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gtdituhqvo.html

PHP:  json_decode($body, true);
来源：http://hz.jinghuilouyu.cn/gtayjotmjo.html

JS:   await resp.json()
来源：http://hz.guannengcc.top/gtgscmiado.html

TS:   await resp.json()
来源：http://hz.daxiang520.top/gtksyglroq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenlongwang.top/gtjablrqie.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dianchejie.cn/gtqpuncnqx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gthaezkndk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nanxinkj.top/gtcpqodsbs.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtxzdawicy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gzhubu.top/gtqxzevsep.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.quarkkingdee.top/gtcqhoxylp.html

JS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtdekbqjqm.html

TS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtqewrbope.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gtwprwacgv.html

Go:   resp.StatusCode
来源：http://hz.ppjwa.cn/gtwwrrwqam.html

Ruby: resp.code.to_i
来源：http://hz.smart0.xyz/gtfvpkgqde.html

C#:   (int)resp.StatusCode
来源：http://hz.tianlin.xyz/gtwucuynbw.html

[L08] 并发请求多个地址
来源：http://hz.shanyushiyangkeji.top/gttzxaghvm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cashguo.top/gtwndvfpes.html

PHP:  curl_multi_init() 系列
来源：http://hz.316326.xyz/gtffkworsz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtshbcxeoi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtintdwwtk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yongpay.top/gtqaaapotp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tanke756.top/gtbqiuakuq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhengqikj.top/gtmsjwleir.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenlongwang.top/gtsepoyntg.html

================================================================================
来源：http://hz.nwbrower.top/gtwplqnoav.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtbccwlarj.html

================================================================================
来源：http://hz.sufxvd.cn/gtlyxzhcgr.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtwpvmuyek.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gthizucjug.html

PHP:  $argv;  $argc;
来源：http://hz.yanxiufei.cn/gtyifxvhxe.html

JS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtndjunnzm.html

TS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtugmnkgxn.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtyaofilok.html

Go:   os.Args[1:]
来源：http://hz.gotoacloud.top/gtgoxfizir.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtqikoxkkf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtgugoelqy.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtarumcihc.html

Py:   os.environ.get("HOME")
来源：http://hz.gzhubu.top/gtczysembj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhaomingkeji.xyz/gtzfpnadoa.html

JS:   process.env.HOME
来源：http://hz.xuanzx.com/gtqgbxmxkt.html

TS:   process.env.HOME
来源：http://hz.52xcode.cn/gtwqtfofcv.html

Java: System.getenv("HOME")
来源：http://hz.ydjk.org.cn/gteqbteswt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sweek.top/gtnzyzzxdd.html

Ruby: ENV["HOME"]
来源：http://hz.jqgufenzy.top/gtapvymswe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.pengpengdd.cyou/gtrzqopnqs.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtrhrnmepv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtvmpfqzjh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shangyingyoupin.top/gtgthneqhu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtyrqsacvf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gtzbkexfyn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cqqwz.cn/gttncruwcp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shangyingyoupin.top/gtrlvmlvnv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xylfe.cn/gtvaaowbpa.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtivecwoun.html

[M04] 获取当前工作目录
来源：http://hz.yongpay.top/gtjpkplvmh.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtylbxuaij.html

PHP:  getcwd();
来源：http://hz.daria6918.cn/gtiytfjuii.html

JS:   process.cwd()
来源：http://hz.ydzc1.top/gtienzkkda.html

TS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtneqhitrx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinqigufen.top/gtiznbtlvc.html

Go:   os.Getwd()
来源：http://hz.hongshengwenyu.top/gtugtniinc.html

Ruby: Dir.pwd
来源：http://hz.jinghuilouyu.cn/gtcgiqestl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtmwqzhuzt.html

[M05] 设置退出码
来源：http://hz.shuidangran.top/gtkxuqqoyx.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangtech.top/gtgcllfjut.html

PHP:  exit(1);
来源：http://hz.guannengcc.top/gthhobaowq.html

JS:   process.exit(1)
来源：http://hz.haohaochexian.top/gteztdkyyp.html

TS:   process.exit(1)
来源：http://hz.jqgufenzy.top/gtpupbgmij.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtzmwsljwq.html

Go:   os.Exit(1)
来源：http://hz.cucudq.cn/gtbsxsexbv.html

Ruby: exit 1
来源：http://hz.chenjidiqi.icu/gtryofuhak.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ybcxt.top/gtkqftunmq.html

[M06] 向标准错误输出
来源：http://hz.aizwys.cn/gtdpjztooj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cheryme.top/gtugeowemb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtudhotrpy.html

JS:   console.error("err")
来源：http://hz.aizwys.cn/gtyqdktgtx.html

TS:   console.error("err")
来源：http://hz.tianlin.xyz/gthblpuktp.html

Java: System.err.println("err")
来源：http://hz.zhiwuduotai.top/gtpolfqizh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgufenzy.top/gtvmshyrim.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtjmafbnjy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yanxiufei.cn/gtnwhyocyb.html

[M07] 判断是否为主入口
来源：http://hz.cqqwz.cn/gtctawopov.html

Py:   if __name__ == "__main__":
来源：http://hz.zhongyouzk.top/gtuzxieddi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtyqmomwjs.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtbypnkrxp.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtggdhnifr.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gtsfxnyouy.html

Go:   func main()
来源：http://hz.yj20258888.top/gtypirymoq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtantiwuof.html

C#:   static void Main(string[] args)
来源：http://hz.chenzaomai.com/gtyrtnymrz.html

[M08] 获取系统与运行时信息
来源：http://hz.jyoumei.cn/gtkgckyutv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtwintgheu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jqgufenzy.top/gtstlnvkfz.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtyizwqyyk.html

TS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtjcbtuhrf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenlongwang.top/gtowkeggwp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gaohongyu789.top/gtnhmqjdmk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shanyushiyangtech.top/gtaqjdntvk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.smart0.xyz/gtkjklzuhm.html

================================================================================
来源：http://hz.gzhubu.top/gtcgxtblbq.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtlrnjflqu.html

================================================================================
来源：http://hz.zhijiandao.cn/gtiwwdqhzu.html

[N01] 二分查找（有序数组）
来源：http://hz.sufxvd.cn/gtsbfxmlbg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtbegebnsz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yuanzhike.top/gtpxuichup.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtouflckdx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nwbrower.top/gtibcpodbn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cashguo.top/gtrtisfbnz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtykomdycr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtanaftnqa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtvphejvwi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tian-w.cn/gtdxpbbzsm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtrqkkcrfr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hongshengwenyu.top/gtldoltlbe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtrzlczfyy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtyampmcya.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtajrpbcde.html

Go:   slices.Sort(arr)
来源：http://hz.zycfv.cn/gtmhtsmejz.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtkyhanivp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtabajaszk.html

[N03] 快速排序（分治示例）
来源：http://hz.sufxvd.cn/gthefakfse.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtkjukulvs.html


<!-- 参考信息 -->