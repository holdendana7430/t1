代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.ivvv.top/gthzmdtwhr.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangtech.top/gtrweeidzf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gogol.net.cn/gtcbpgqryj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.meibo888.top/gtaoeqaugs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtmvimweqn.html

Go:   end.Sub(start).Hours()
来源：http://hz.nwbrower.top/gtqjardpkv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gttmkynhas.html

C#:   (end - start).TotalSeconds
来源：http://hz.bjfxy.top/gtorrrvocy.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gtjwltlplu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtnnepqbcf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtubejulie.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtwbhhfwyp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtoxnqvaya.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtwcttchnu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhixingplan.top/gtymimzdxe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtfimogxvz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtevqeoyej.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtvtlelniw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtsnnqffjf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtpweavxkn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtrjzqlpbl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtsyiiehsi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dashuyun.cn/gthexokawi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guowangkeji.top/gtyjygmfjb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.iojbl.cn/gtyryjpvjy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtikoxqyxs.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtcuptdpax.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtcryiigdm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.bjfxy.top/gtpxdggiud.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtljlisstk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtaddiayja.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sysykeji.top/gtqcacebun.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daxiang520.top/gtisimcuxf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtcojbbrma.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gzhubu.top/gtybtdlglv.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtaluddqaq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258.top/gtxzoikcsz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtkpixqbyc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtktyonzjj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtdsxbsxdb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jiagoushi.top/gtylplbqjo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.iojbl.cn/gtivazmgno.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtsvtgryqz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtavmapfly.html

================================================================================
来源：http://hz.nwbrower.top/gtkbreiwqc.html

K. JSON 与序列化
来源：http://hz.316326.xyz/gtalcdqbjq.html

================================================================================
来源：http://hz.daxiang520.top/gtqupiqzrj.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuanzhike.top/gtjqntsagh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtqhdlimgl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtkxdwaybf.html

JS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtminfxfsp.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtftcseqcs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.0kj1m.cn/gthkkxlyqa.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigufen.top/gtneftoidh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.0kj1m.cn/gttlprszxv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtzhrceycs.html

[K02] JSON 字符串转对象
来源：http://hz.fengsongda.top/gtrgilvtiy.html

Py:   json.loads(s)
来源：http://hz.hywenlv.cn/gtyiejbdbq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtacdkjzry.html

JS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gthrdgwmrq.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtjqnhhyrc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.9152youxi.cn/gtigftpwda.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtguqtaogp.html

Ruby: JSON.parse(s)
来源：http://hz.316326.xyz/gtqpgffaob.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zdqjudy.top/gtcgvevstq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.0kj1m.cn/gtyinstpoo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtufurzjqp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtupgrhduk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.andypj.xyz/gtcjsjfeuh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtkipqpssy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydjk.org.cn/gtamncbepl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtezzvppnj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxuanxn.top/gtqpbxvnqm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gtvfozdapc.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigfzy.top/gtbhjcynau.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtlcyejoaw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtnpbqlnda.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtrtrvvnhb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtfbpqesjt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtggygzbav.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtznmurpct.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtiljiusts.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gteulewhhm.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangkeji.top/gtfxsizchx.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtltuztjxj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangkeji.top/gtfylfsrxj.html

JS:   structuredClone(obj)
来源：http://hz.sweek.top/gtotikmujl.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtlhgexysk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtoguhrssm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guowangkeji.top/gtarnjxsof.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtavjsiavs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shzxlz.cn/gtgmntuyxi.html

[K06] 解析 URL 查询串
来源：http://hz.shangyingyoupin.top/gtwihczbrv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtcyxiwgdd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.52xcode.cn/gtipmhtxfp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtpbvzwqod.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtlssdiosp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gtcgbngyuw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.birdmap.top/gtniruolws.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pycfn.com/gtenulmlnl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gthtttoexa.html

[K07] 进制转换
来源：http://hz.ppjwa.cn/gtpxedtkpg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gteefevzti.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtmpqklssl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtnovumdfm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtldtrqjde.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gthllqeyth.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daria6918.cn/gtwlwcubgv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtlhsjstma.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtpgoflnlu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtxisfdnqn.html

Py:   pickle.dumps(obj)
来源：http://hz.fengsongda.top/gthvvtkgwh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zdqjudy.top/gtmlskwnfk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtsivjhdyb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtjmloufsz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zdqjudy.top/gtrheoxisr.html

Go:   encoding/gob
来源：http://hz.yonumen.top/gttvrlkciv.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtqwxuovvj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gtaatrbrxg.html

================================================================================
来源：http://hz.mhx1999.top/gtfxdtmkoi.html

L. 网络请求
来源：http://hz.zhengqikj.top/gtotpsrbfb.html

================================================================================
来源：http://hz.tian-w.cn/gtnqeukelj.html

[L01] 发送 GET 请求
来源：http://hz.pengpengdd.cyou/gtddgzojeg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtpiplafpe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtfdmvuxfh.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtjyivnevo.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gthvycgazw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgufenzy.top/gtzxvkseba.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtoamcghjo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gtuhjwfvwj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuanzhike.top/gtnzqpbpvo.html

[L02] 发送 POST JSON
来源：http://hz.jinqigufen.top/gtakxvnwnq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtuhpezuxv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.smart0.xyz/gtklexldye.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtelnnvhpk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtismpfkmw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtavocqonx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jlsjyb.cn/gtaplslxnl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtrnqpmqeu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhongyouzk.top/gtfcclykcj.html

[L03] 设置自定义请求头
来源：http://hz.hysaishi.cn/gtyjhewfrw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xingfuxueyuan.xyz/gtbdjojywh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.kuanghao11.cn/gtmgjqtxlu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.iojbl.cn/gtujkgkntm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtnlccmkib.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hfpthk.cn/gtnjyuxsrm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtiiqaataw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gterijpdhx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtkdicqfrk.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gteqchqvre.html

Py:   requests.get(url, timeout=5)
来源：http://hz.vqdsnc.cn/gtbbqgmzki.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydjk.org.cn/gtimnvptmd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtbupuclld.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aizwys.cn/gtphsnjzzi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.smart0.xyz/gtmmiqvxdo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.0kj1m.cn/gtobudnqwg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhixingplan.top/gtgmyqoqnt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gtwcwfzcxh.html

[L05] 上传文件（multipart）
来源：http://hz.svipenyu.cn/gtppngfbob.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydzc1.top/gtzrdcyvfu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxinkj.top/gtckfeuwep.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtgytcrnny.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tanke756.top/gtulrlmrkh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangdashe.top/gtzqveytrm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtgpwaclgg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cqqwz.cn/gtqfnbxsuc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258888.top/gtncksytoq.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtmvajmwwu.html

Py:   resp.json()
来源：http://hz.zhijiandao.cn/gteazdlkcd.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtriiesanc.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtjipcsicx.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtrgfrsuwo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydjk.org.cn/gtqwucxyao.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guannengcc.top/gtacyvaayx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sufxvd.cn/gtfhrmoayv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtjwixlkaz.html

[L07] 处理 HTTP 状态码
来源：http://hz.quarkkingdee.top/gtmlwprpac.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj202588.top/gthemwhgsm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangshuangyany.cn/gtzpzpshtj.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtxxnbqiwc.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtyovqboyl.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gtkbodndjj.html

Go:   resp.StatusCode
来源：http://hz.ydjk.org.cn/gtggoucvtu.html

Ruby: resp.code.to_i
来源：http://hz.9152youxi.cn/gtquxirrpb.html

C#:   (int)resp.StatusCode
来源：http://hz.zdqjudy.top/gthahyqmvu.html

[L08] 并发请求多个地址
来源：http://hz.chenlongwang.top/gtjfalvnrt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtahemlkvj.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtohetanys.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtdrrdweit.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtkzkxhuvo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yanxiufei.cn/gtrcilzxjo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jianghu66.top/gttkktwoao.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tanke756.top/gtzrdrqznt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtqfuuafsu.html

================================================================================
来源：http://hz.ehwqpu.com/gtxeporikw.html

M. 命令行 / 进程 / 环境
来源：http://hz.aizwys.cn/gtuerucmit.html

================================================================================
来源：http://hz.gzhubu.top/gtybabjodp.html

[M01] 读取命令行参数
来源：http://hz.kuanghao11.cn/gtavkmhfvu.html

Py:   sys.argv[1:]
来源：http://hz.hywenlv.cn/gtbadlgggs.html

PHP:  $argv;  $argc;
来源：http://hz.nanxinkj.top/gtxxxuulsg.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtpnocktkw.html

TS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtibjklykh.html

Java: args 数组（main 方法参数）
来源：http://hz.smart0.xyz/gtqllsfmtu.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtolpsvsch.html

Ruby: ARGV
来源：http://hz.hongshengwenyu.top/gtcksyeddx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jqgufenzy.top/gtrggdzbhe.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtdgxzggxo.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangkeji.top/gtlzcmpwju.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydjk.org.cn/gtiwmbjrof.html

JS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtoytiojnx.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtsflpefxs.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtmlqavghh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ehwqpu.com/gtwscjohpd.html

Ruby: ENV["HOME"]
来源：http://hz.zycfv.cn/gtsejrfcbj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtpdtokibp.html

[M03] 执行外部命令
来源：http://hz.ybcxt.top/gtaiivpaty.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangtech.top/gtcadinmcw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hysaishi.cn/gtmjflhonp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtwnjaefqc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sxryk.cn/gtoofzbnld.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ydzc1.top/gtjaekkqoq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zycfv.cn/gtfasrgcex.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtcikcoyix.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtlxtbvozy.html

[M04] 获取当前工作目录
来源：http://hz.havefunace.top/gtmegsqegq.html

Py:   os.getcwd()
来源：http://hz.aizwys.cn/gttfmfaxja.html

PHP:  getcwd();
来源：http://hz.hongshengwenyu.top/gttepudftk.html

JS:   process.cwd()
来源：http://hz.ivvv.top/gtodqxbcbe.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtvhgwjqwb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtijauqddt.html

Go:   os.Getwd()
来源：http://hz.bjfxy.top/gtnbgjitbr.html

Ruby: Dir.pwd
来源：http://hz.zhoulong.xyz/gtavvojnki.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtxcuhyrad.html

[M05] 设置退出码
来源：http://hz.aibaodan.cn/gtmljehjrv.html

Py:   sys.exit(1)
来源：http://hz.jlsjyb.cn/gtihthlgcq.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gtnisjsxpu.html

JS:   process.exit(1)
来源：http://hz.zycfv.cn/gtogaaicds.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtekflmdbg.html

Java: System.exit(1)
来源：http://hz.jiagoushi.top/gtqocichte.html

Go:   os.Exit(1)
来源：http://hz.zhoulong.xyz/gtlpmnrdhy.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gtjzoblsrz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.snrcjt.cn/gtunirbstk.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtetwbzduw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtljfpujtp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yongpay.top/gtgyvukoax.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtdozjhtig.html

TS:   console.error("err")
来源：http://hz.fengsongda.top/gtjrwcfztp.html

Java: System.err.println("err")
来源：http://hz.shuidangran.top/gtvkpspjuu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtmntotxmu.html

Ruby: warn "err"
来源：http://hz.chenjidiqi.icu/gtjuhfsnwg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jiagoushi.top/gtuwqotsts.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtefnkprvu.html

Py:   if __name__ == "__main__":
来源：http://hz.jiagoushi.top/gtxvmbgtqb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fengsongda.top/gtcsrujkmr.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtflucxxow.html

TS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gthaaworhq.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtumsevhsf.html

Go:   func main()
来源：http://hz.xinyue.icu/gtqehypcje.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.feifeiyinyue.top/gtrhgelcks.html

C#:   static void Main(string[] args)
来源：http://hz.zhengqikj.top/gtobchsjft.html

[M08] 获取系统与运行时信息
来源：http://hz.zhiwuduotai.top/gthijnjjen.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigufen.top/gtodswnjro.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.vqdsnc.cn/gttxcnauvb.html

JS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtecnnlfow.html

TS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtahkxcvlz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.meibo888.top/gtorsinudh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xziqi.cn/gtljutqkmb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shzxlz.cn/gttttlrdih.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gtupdkwjay.html

================================================================================
来源：http://hz.quarkkingdee.top/gtqixmndxg.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtauvhjxps.html

================================================================================
来源：http://hz.jinqigfzy.top/gtzrwlddqr.html

[N01] 二分查找（有序数组）
来源：http://hz.svipenyu.cn/gtwqdjaaex.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhiwuduotai.top/gtptfsknri.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhongyouzk.top/gtmmqlzikt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtnxgxbspi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtrnzvvhow.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aizwys.cn/gtypurljpd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.redwolf501.top/gtbkupzxht.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.chenlongwang.top/gtjtirscvm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sweek.top/gtpckylbuo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.bjfxy.top/gtlregetgu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtbtpjrbzp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangtech.top/gtiegjoaff.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtkqddohmh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtgflosxve.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhongyouzk.top/gtrokeodxk.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtvpdcsfvd.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtcxljqyky.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cashguo.top/gtnpancorv.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtwhkqdxhl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nwbrower.top/gteedxfwxo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtrihshrqg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtenmvpohb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtfiufqdhm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.bjfxy.top/gtzmvxdtif.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuxming.cn/gtgbptziwx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxuanxn.top/gtejczfumq.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.dashuyun.cn/gtrxruyzyd.html

[N04] 斐波那契数列
来源：http://hz.meibo888.top/gtumqsjkgd.html


<!-- 参考信息 -->