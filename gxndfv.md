代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtlshthgzv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtadcrgqti.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtzufycnpy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtuiwdsjyc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtylullyab.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gthvgeafpl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hammf.cn/gtypjelmji.html

[J06] 计算两时间之差
来源：http://hz.0kj1m.cn/gtsowfzdqu.html

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gtkdezmewd.html

PHP:  $end->diff($start)->days;
来源：http://hz.fengsongda.top/gtowhcbjqe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gtvhlhpmrs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtvcwmjnjd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zdqjudy.top/gtdrqoweut.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinyuanbaomall.cn/gtqvacwwlm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtyfvjshlz.html

C#:   (end - start).TotalSeconds
来源：http://hz.hongshengwenyu.top/gtqbykhodj.html

[J07] 比较两个日期
来源：http://hz.meibo888.top/gtugqvnnlp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtyvydgfzh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtzzhcsjkv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtvmhsngcj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sxryk.cn/gtmenqxcne.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gthkyphglj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.9152youxi.cn/gtevebabfa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtlncoocwn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtvcbemdos.html

[J08] 提取年月日与星期
来源：http://hz.wangdashe.top/gtepotbnju.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fengsongda.top/gtfsvbxrcg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hammf.cn/gtiiwbtdxf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtqyqprkdb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtvvkclnrx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhengqikj.top/gtrrckranh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cdnleiting.top/gtuskqevfr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guannengcc.top/gtpknwtdlf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cashguo.top/gtfvodbiyb.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtgmocutzl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guowangkeji.top/gtxicbpiyo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sysykeji.top/gtnndqkmqh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtaqidbffo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtwrqbdhqf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shangyingyoupin.top/gtnhvlzfdc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtsnzebxyp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtdsuqnpac.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtgqthbrpw.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangshuangyany.cn/gtsyrreqfc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gthafucxzp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtjpniflgk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cheryme.top/gtmgqvziyx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtelyibbpl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtsrvnxdwl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gttrywgypx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenlongwang.top/gtqrabqtso.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.smart0.xyz/gtzhasmdtz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtbohkcbzn.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtbqygkfme.html

================================================================================
来源：http://hz.dianchejie.cn/gtbxciowwh.html

[K01] 对象转 JSON 字符串
来源：http://hz.ywan-chungtsiang.top/gthfoykwqr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtclebrpvn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtbhagstex.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtjlinetnu.html

TS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtihlfunac.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ybcxt.top/gtdsemhspv.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtawkgrudp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtiymijflc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtxxijscpi.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gteawegois.html

Py:   json.loads(s)
来源：http://hz.aizwys.cn/gtimvfimbw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xinyue.icu/gtifoainaq.html

JS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtwdmrdqjz.html

TS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtyejnvvno.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yangfankeji.com/gtpoutnxlc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtayfhlafb.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtbpdrbmpm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhongyouzk.top/gtjdbgrkfy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtbztszlrr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gttvlfeztw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtiuhkcedj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtnewsuxih.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtirrhnifq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtxqubqtck.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtnlnasisc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xingfuxueyuan.xyz/gtqffaschw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.52xcode.cn/gtpcgyoumq.html

[K04] 读取 JSON 文件
来源：http://hz.ivvv.top/gtxjybusix.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.316326.xyz/gtrbjafcri.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtkvneylfz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtxkqpkpjg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtgrxxtlnl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenjidiqi.icu/gtnqzwpqsw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtyqcxnftv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gtcyoinwbf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sufxvd.cn/gtngvcfmpe.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gtrcezqqek.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gtdchifhnv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtputalezg.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtswqwyaae.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gttnaaceka.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gtwynopntb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtglthzbbn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yanxiufei.cn/gtnchrnqfg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ivvv.top/gtsausnklm.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtcxoqzvwj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhengqikj.top/gtynlsrjec.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gtxarbfgvl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtdwfnwpsz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtjsxgkspi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jiagoushi.top/gtojpppqwj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.havefunace.top/gtoqotjxcy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtuvxswusu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtzdtjhpkf.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gteaxwybkt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zdqjudy.top/gtyvkeviyy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pycfn.com/gtkquyodfr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtbjtufotw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtxmrzeljs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtqfplojzz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtirenidef.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtxmmukghj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgufenzy.top/gtnajdrqkx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hysaishi.cn/gtjfbxacqo.html

Py:   pickle.dumps(obj)
来源：http://hz.feifeiyinyue.top/gtosophvmp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shuidangran.top/gtwjnliavs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtpllaqmkl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtgdfmfhza.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtpvhsqyzd.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtqlsaaldj.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhixingplan.top/gtlyvwkhve.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtblodecar.html

================================================================================
来源：http://hz.cdnleiting.top/gtpdxlwpmz.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtlersbmne.html

================================================================================
来源：http://hz.fengsongda.top/gtqkdjbyxb.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtubflesec.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhijiandao.cn/gtvetckhwk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtvmrxguju.html

JS:   await fetch(url)
来源：http://hz.zhixingplan.top/gtmtrbqdiz.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtqikivsej.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtyiyizche.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gttywugzkm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtgwvjaswp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtocgvarle.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtuxasardk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtznlmhqer.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtfmiepcyw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtecspsclj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnqzz.top/gtxnwkwing.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zycfv.cn/gtlvzrcsoo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gotoacloud.top/gtctrnncdl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtegxrlabh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gthehsfrpz.html

[L03] 设置自定义请求头
来源：http://hz.havefunace.top/gtitzqempk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydzc1.top/gtmyrzpjpw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yuanzhike.top/gtcejcugky.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtuhnmezbl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtxiuadren.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ivvv.top/gtdmbbonbp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zycfv.cn/gthwxcshag.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuxming.cn/gtmnnoyzgb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtjihkndth.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtaxogkzjd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtnvfivlmt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gtmavvifdv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtxkzoixbw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtfjuwkpqs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.316326.xyz/gtcmzjdkjj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.vqdsnc.cn/gtifpoopsd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aibaodan.cn/gtgtkevbbb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gtqzdivvqp.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gttjdyrjef.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgufenzy.top/gtqbtnwuqi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.c1oappe.top/gtcgniwlkl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtyspkuyqu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtkcljljqq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jianghu66.top/gtzcvpusxj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.0kj1m.cn/gtmowrbecl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtpoodsnpk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yonumen.top/gtygpabqav.html

[L06] 解析响应为 JSON
来源：http://hz.0kj1m.cn/gtxmvyurnm.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtpckmltgd.html

PHP:  json_decode($body, true);
来源：http://hz.hammf.cn/gtecrauize.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtsifhpnfu.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gttaujyrxh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yangfankeji.com/gtmzaeqgvs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jianghu66.top/gtrghzrjlc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj202588.top/gttosbiobh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jyoumei.cn/gtykrtyvei.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtmdncmsmo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtmxrarqof.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gtxztyrkpo.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtaxhjrhbt.html

TS:   resp.ok;  resp.status
来源：http://hz.shzxlz.cn/gtdefmiypd.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gthratjqnn.html

Go:   resp.StatusCode
来源：http://hz.iojbl.cn/gtypotjnyd.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtzlfexcla.html

C#:   (int)resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gthlecorov.html

[L08] 并发请求多个地址
来源：http://hz.pycfn.com/gtagwcteyu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hywenlv.cn/gtztitelrb.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtaitpkgap.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtupppkpdy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtfnkorjlb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cqqwz.cn/gtvgnqsiyq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gzhubu.top/gtunlhcdfn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gtkapnzwuh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtbudpxdzi.html

================================================================================
来源：http://hz.nwbrower.top/gtbdxxzqxc.html

M. 命令行 / 进程 / 环境
来源：http://hz.dashuyun.cn/gtkrnclvws.html

================================================================================
来源：http://hz.ydzc1.top/gtneddupff.html

[M01] 读取命令行参数
来源：http://hz.zhoulong.xyz/gtaznwphtc.html

Py:   sys.argv[1:]
来源：http://hz.feifeiyinyue.top/gtqyjebfen.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gtchxjweze.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtnfqxacrk.html

TS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gteczvdziu.html

Java: args 数组（main 方法参数）
来源：http://hz.hywenlv.cn/gtlgjtjbhg.html

Go:   os.Args[1:]
来源：http://hz.gaohongyu789.top/gtvsykqgur.html

Ruby: ARGV
来源：http://hz.cashguo.top/gtmjqyavoz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.haohaochexian.top/gtcpsakqfj.html

[M02] 读取环境变量
来源：http://hz.vqdsnc.cn/gtazfvxafy.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gtvdtfljlk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.havefunace.top/gtsuwdmbcj.html

JS:   process.env.HOME
来源：http://hz.meibo888.top/gtknqplugq.html

TS:   process.env.HOME
来源：http://hz.vqdsnc.cn/gtytpdfuqk.html

Java: System.getenv("HOME")
来源：http://hz.hywenlv.cn/gtoxdixxel.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sxryk.cn/gtyrmoelpz.html

Ruby: ENV["HOME"]
来源：http://hz.yvedp.cn/gtxuybjzyp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gttuehojxr.html

[M03] 执行外部命令
来源：http://hz.0kj1m.cn/gthbnpwkum.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.quarkkingdee.top/gtgwupuwky.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangdashe.top/gtrjmpsjlv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj202588.top/gtdkotrjmk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtudcsunkv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ehwqpu.com/gtlojjkjlq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtyvpkfjsg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.meibo888.top/gtbfbmimwo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtyvhffpgn.html

[M04] 获取当前工作目录
来源：http://hz.yueranfly.top/gtkuedhoep.html

Py:   os.getcwd()
来源：http://hz.meibo888.top/gtzqhscblj.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtogjjqjcd.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gthythtppx.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtesswsiid.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtfzsomlzf.html

Go:   os.Getwd()
来源：http://hz.yongpay.top/gtmltovoex.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtylbjglen.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yj20258888.top/gtwxauavjv.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gtlxyflenk.html

Py:   sys.exit(1)
来源：http://hz.yanxiufei.cn/gtqmyksmee.html

PHP:  exit(1);
来源：http://hz.daria6918.cn/gtixjgbruc.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtjyfndtzu.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtmnxqfdam.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtptdvigxs.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtdgicrdjm.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtydooxplx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtfckylgqm.html

[M06] 向标准错误输出
来源：http://hz.0kj1m.cn/gtzfxyeefr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtvcauncwu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sysykeji.top/gtalokphdk.html

JS:   console.error("err")
来源：http://hz.dianchejie.cn/gtdudwznrw.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtppaadlod.html

Java: System.err.println("err")
来源：http://hz.yueranfly.top/gtnvsethnd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangshuangyany.cn/gtjrijpmcv.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtleqsredc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydjk.org.cn/gteqxhxckg.html

[M07] 判断是否为主入口
来源：http://hz.shangyingyoupin.top/gttupfewaa.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtaznljzdj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtfapwljol.html

JS:   require.main === module
来源：http://hz.jinghuilouyu.cn/gtzcutdnsi.html

TS:   require.main === module
来源：http://hz.daria6918.cn/gtwbgnqxpl.html

Java: public static void main(String[] args)
来源：http://hz.jiagoushi.top/gtqxcdtbmw.html

Go:   func main()
来源：http://hz.vqdsnc.cn/gtrkguudja.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hfpthk.cn/gtkgaleohs.html

C#:   static void Main(string[] args)
来源：http://hz.xuanzx.com/gtaqfaocbv.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gthirinmwo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jiagoushi.top/gtvedfrqgr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuetiantiany.cn/gtfxlhcrpz.html

JS:   process.platform;  process.version
来源：http://hz.pycfn.com/gtzrmpshym.html

TS:   process.platform;  process.version
来源：http://hz.ivvv.top/gtmgfbhajp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinqigfzy.top/gtdrcxtwnl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtcxaauhmt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.quarkkingdee.top/gtkhmamekl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tanke756.top/gtxahnykdv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtunxhzlge.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtpupkkfwb.html

================================================================================
来源：http://hz.jiagoushi.top/gtrcycnnnn.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtxnmsipzu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sufxvd.cn/gtgvwzxsok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gtumnelgbr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gotoacloud.top/gtxixeloli.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuxming.cn/gtgvkcnqtw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtftmjvpdn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtuihrhvpx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gaohongyu789.top/gtplsyajbo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hammf.cn/gtgbzrapoy.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yvedp.cn/gticegwhff.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cucudq.cn/gtwfumclqp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhoulong.xyz/gtmynrvhou.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtbxepsnen.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtpjmffzuy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtokannicq.html

Go:   slices.Sort(arr)
来源：http://hz.tian-w.cn/gthmqkouvt.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtqwjvbzah.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxinkj.top/gtuniddqzd.html

[N03] 快速排序（分治示例）
来源：http://hz.ybcxt.top/gtwaachtkm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yonumen.top/gtajedacab.html


<!-- 参考信息 -->