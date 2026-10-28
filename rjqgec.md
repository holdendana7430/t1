代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fengsongda.top/gtepwllxvw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hywenlv.cn/gthfruaojq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtrmptpvpy.html

[J06] 计算两时间之差
来源：http://hz.gogol.net.cn/gtjhuyafej.html

Py:   (end - start).total_seconds()
来源：http://hz.andypj.xyz/gtlimczsou.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gtwqfwadel.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cqqwz.cn/gtfawpwqxx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtmwnuhhoe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtzvcplytz.html

Go:   end.Sub(start).Hours()
来源：http://hz.snrcjt.cn/gtetestynn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtwnpnblvh.html

C#:   (end - start).TotalSeconds
来源：http://hz.9152youxi.cn/gtqteyydqm.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtnxzevdkj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtpgixtaxe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuetiantiany.cn/gtnleukhmc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtygpfqkxm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gttusqyhpl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtihtdmwaj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gtrzcwgikl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gttxrpckop.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtzctwbzcj.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtkevmrilc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gttcvwkwkr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtpijwyiuy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gotoacloud.top/gthuctutnb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxinkj.top/gtsydyecxw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.mhx1999.top/gtsawfwycr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtebwdzvzb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtbrwjhrrx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hnxiangtu.top/gtsrfmxurs.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtcozybkhh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hywenlv.cn/gtcbalzbto.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtpdvoozup.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtianrrzjm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtxmvqrkmz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.vqdsnc.cn/gtdzrxtxag.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtnrkcezjl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.vqdsnc.cn/gtagcmvzfs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydjk.org.cn/gtiebchqwj.html

[J10] 取今天 / 本月第一天
来源：http://hz.pycfn.com/gtgotjybzz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dianchejie.cn/gtyllyhfcx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtlwkcxlxd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yongpay.top/gtozxlkxim.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtzxbimtqb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gtigtzfcdx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigfzy.top/gtheknwqmm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtuwqelzwo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtiztxmkkw.html

================================================================================
来源：http://hz.gzhubu.top/gtkcvcfjvj.html

K. JSON 与序列化
来源：http://hz.daria6918.cn/gthkxpzuli.html

================================================================================
来源：http://hz.yonumen.top/gtzokxcted.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtlvmfgevt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtlpkwzcwc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtjhekkqyw.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtowealirb.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtfvhirfll.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtboctlcbz.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtkwqngibt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtbvqszaug.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtbpudkuyk.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gtsjfqufhn.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gthcrsirxk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtohuexhqf.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtosjjitxg.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtnymolgsm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.redwolf501.top/gtttgeeggu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtuqnduwuq.html

Ruby: JSON.parse(s)
来源：http://hz.snrcjt.cn/gtvpvrqyvc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ppjwa.cn/gtwmdfmjac.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtndhcdvxq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtlzvsiaxz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtsezpaics.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtzlzqyosd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtoydoauqz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.feifeiyinyue.top/gtzkoszgfb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtbuvykqvj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.0kj1m.cn/gteklnpvda.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtnyfvvyro.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtdrfhxifg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aizwys.cn/gtyvndduwe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj202588.top/gtazwgxzeu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtuxsjwleq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtwedgfjfz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gttfberytb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtmusdmlmg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtqbkdtfjf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gthobuckmt.html

[K05] 深拷贝对象
来源：http://hz.ybcxt.top/gthpvkrfhh.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuxming.cn/gtwfzbsokd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gogol.net.cn/gtylvuzqkm.html

JS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtnkdcjlvk.html

TS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtbvhnlgmq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.vqdsnc.cn/gtqgroriao.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.smart0.xyz/gtsxhlrsiq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pengpengdd.cyou/gtukojyiou.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangkeji.top/gtfzsztywa.html

[K06] 解析 URL 查询串
来源：http://hz.yj20258.top/gtykirnnkz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sysykeji.top/gtjsshwpoj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ehwqpu.com/gthloykaah.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtgptdpnng.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dianchejie.cn/gtyhmkblql.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gtenrbrrrk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gttbhybgqo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hammf.cn/gtldmfrbjz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gtzvovowfm.html

[K07] 进制转换
来源：http://hz.sweek.top/gtjwdtzqbw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtgeiwkwdg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtmezesjlv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtnpjbebvg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yongpay.top/gtsmaapjre.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtymamupse.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cucudq.cn/gtuswiptbi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhixingplan.top/gtccbwdwex.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tanke756.top/gtmlexvezd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.vqdsnc.cn/gtiesdnnxn.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtvjudvmpj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigufen.top/gtahceyjak.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtwvyqexfi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtxmhgmhts.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtfnqwsptp.html

Go:   encoding/gob
来源：http://hz.pycfn.com/gthavggbnb.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtkwktgfmq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtwazrxkvs.html

================================================================================
来源：http://hz.cdnleiting.top/gtqalbfcer.html

L. 网络请求
来源：http://hz.shangyingyoupin.top/gtndapvtvm.html

================================================================================
来源：http://hz.hnqzz.top/gtslpjfufg.html

[L01] 发送 GET 请求
来源：http://hz.yuanzhike.top/gtvpnyippk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtekdhwopa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tianlin.xyz/gtecptvcip.html

JS:   await fetch(url)
来源：http://hz.smart0.xyz/gtlprijxng.html

TS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtlavvoxgw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigfzy.top/gtfabizkzc.html

Go:   resp, err := http.Get(url)
来源：http://hz.quarkkingdee.top/gtkexjounr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhongyouzk.top/gtsocgxqgu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhengqikj.top/gtlbpecdgn.html

[L02] 发送 POST JSON
来源：http://hz.xinyue.icu/gtfnjyjmct.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhixingplan.top/gtyobilkwl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jiagoushi.top/gtkgosshsf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtrprgzgfn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtlemgqhbb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigufen.top/gtpxkakuqf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ppjwa.cn/gthpmzansw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.mhx1999.top/gtmhjyngtg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hnqzz.top/gtyfyxcpny.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtuqdmusci.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtcjxtiwle.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtiitqkrsf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtwzmllzrl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtidzzzmce.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jyoumei.cn/gtcpvxpbfd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aibaodan.cn/gtsicjzanw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtgsuviods.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cucudq.cn/gtmipdgshn.html

[L04] 设置超时
来源：http://hz.shanyushiyangtech.top/gttpxdcvfr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhijiandao.cn/gtgxapvlbt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hammf.cn/gtdzhdtlgs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtjnnwwbox.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtlubtyelu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtoxvvdviy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gtunkrawmj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtasmbvzsq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtacorczyi.html

[L05] 上传文件（multipart）
来源：http://hz.hfpthk.cn/gttkwsffkd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xylfe.cn/gtybqewkkn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxinkj.top/gtlyzkhipj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.vqdsnc.cn/gtqbzbzxvk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtcgebhvhl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.svipenyu.cn/gthlhfgzvs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cheryme.top/gtzndozifj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nanxinkj.top/gtjnqbiauh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhijiandao.cn/gtweovgcgw.html

[L06] 解析响应为 JSON
来源：http://hz.iojbl.cn/gtpsriyixb.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtytnplilm.html

PHP:  json_decode($body, true);
来源：http://hz.daxiang520.top/gtuqvsxage.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtigcxyboq.html

TS:   await resp.json()
来源：http://hz.chenzaomai.com/gtkmzmamvn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nwbrower.top/gtesbzireb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.snrcjt.cn/gtzpoywadn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtmzqyczhd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtlwksshnw.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtqzyrivna.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenzaomai.com/gtovtvwgbr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.dianchejie.cn/gtctdzisdy.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtlxjanfps.html

TS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtyowctbue.html

Java: resp.statusCode()
来源：http://hz.yanxiufei.cn/gtdtjvhhca.html

Go:   resp.StatusCode
来源：http://hz.meibo888.top/gtngfpufly.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtxbwrjwxr.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtqjmhcmbm.html

[L08] 并发请求多个地址
来源：http://hz.xingfuxueyuan.xyz/gtmdyfjreg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhiwuduotai.top/gtwkiofkub.html

PHP:  curl_multi_init() 系列
来源：http://hz.ehwqpu.com/gtqxwfeyuy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhijiandao.cn/gtvyeansmj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtiwsnnkwu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtqkucewhi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fzhhl.top/gtopxlnuvl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtqselyrzg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.redwolf501.top/gtxkwxbtds.html

================================================================================
来源：http://hz.yvedp.cn/gthtvupoyv.html

M. 命令行 / 进程 / 环境
来源：http://hz.guowangkeji.top/gttvvlogay.html

================================================================================
来源：http://hz.zhijiandao.cn/gtpbvjiwue.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtevkfloay.html

Py:   sys.argv[1:]
来源：http://hz.kuanghao11.cn/gtbnnmexkr.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtfvwzeslz.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtjjiycnjz.html

TS:   process.argv.slice(2)
来源：http://hz.pycfn.com/gtytbyezhm.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtyuhdwtwe.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtaulgolvg.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtfsxuqoou.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuanzx.com/gtebixtivk.html

[M02] 读取环境变量
来源：http://hz.ydjk.org.cn/gtganyhmog.html

Py:   os.environ.get("HOME")
来源：http://hz.jinyuanbaomall.cn/gtikzovjhm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gttdaltfyt.html

JS:   process.env.HOME
来源：http://hz.svipenyu.cn/gthigcmjeg.html

TS:   process.env.HOME
来源：http://hz.xinyue.icu/gtriwzpyli.html

Java: System.getenv("HOME")
来源：http://hz.yj20258.top/gtlsvtqddb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtxoxsnllr.html

Ruby: ENV["HOME"]
来源：http://hz.zdqjudy.top/gtwunrkelr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ppjwa.cn/gtzbwgmgdl.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtcikyvakd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jyoumei.cn/gteedjcqke.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gttsctcjwe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtqeghpqis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtguhbtoho.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hongshengwenyu.top/gtjfyzenyt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtyhwdqqxp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtodltessl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.daria6918.cn/gtfopkztep.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtyoetedro.html

Py:   os.getcwd()
来源：http://hz.pycfn.com/gtwxdoimxg.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtlugoynzj.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtvmxbtzvh.html

TS:   process.cwd()
来源：http://hz.xziqi.cn/gtoxdsmfbm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pengpengdd.cyou/gtplwpveot.html

Go:   os.Getwd()
来源：http://hz.dashuyun.cn/gtdbdvwnre.html

Ruby: Dir.pwd
来源：http://hz.cqqwz.cn/gtxqvrpham.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtbzykxabd.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtjvibbroc.html

Py:   sys.exit(1)
来源：http://hz.aizwys.cn/gtvzxejdar.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtfvoqrkft.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gtctbqalcg.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtiodbrjfx.html

Java: System.exit(1)
来源：http://hz.daxiang520.top/gtveuhmekn.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtcmxojhvp.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtatnrknxz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtwisctwqc.html

[M06] 向标准错误输出
来源：http://hz.tanke756.top/gtydyzbuek.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtlgfvoxlv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenzaomai.com/gtywuckjyo.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtfkbndpyp.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gtnqjzeehb.html

Java: System.err.println("err")
来源：http://hz.9152youxi.cn/gtgedxhbqy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangkeji.top/gtdgwvlxvy.html

Ruby: warn "err"
来源：http://hz.birdmap.top/gthokjdzum.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.wangshuangyany.cn/gtebnrlwdc.html

[M07] 判断是否为主入口
来源：http://hz.jinyuanbaomall.cn/gtrxzsrstj.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtmvqetndd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.birdmap.top/gtmoixvsox.html

JS:   require.main === module
来源：http://hz.gaohongyu789.top/gtojacowkq.html

TS:   require.main === module
来源：http://hz.kuanghao11.cn/gtnrpfybma.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtwtivjzch.html

Go:   func main()
来源：http://hz.aizwys.cn/gtfkdretlj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shuidangran.top/gtmyeaomxo.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtxcqrtyhe.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gttjyreeob.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtdeyuzwqh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.pycfn.com/gtjnodhgtj.html

JS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtpwhyfsfu.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtrkpydfys.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.redwolf501.top/gtjbhulsbc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtusycnpdj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtqadmgzcs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yueranfly.top/gtjprzsraa.html

================================================================================
来源：http://hz.zhengqikj.top/gtcbzlycub.html

N. 数据结构与算法
来源：http://hz.sufxvd.cn/gtxfdqpzbc.html

================================================================================
来源：http://hz.xziqi.cn/gtnfbarytn.html

[N01] 二分查找（有序数组）
来源：http://hz.cucudq.cn/gttfnblrwq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gtyukhedpg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gtdsbijacj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtpvsjexua.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtjbcayqyy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtvyiwkmbn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.svipenyu.cn/gtxdtdnsrc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xinyue.icu/gtaxjtbkfu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tianlin.xyz/gtmvhhjyji.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtbhhttjsm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gtfpdfwgqx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yvedp.cn/gtlolbzeqy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.fengsongda.top/gtknlkruht.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtkvicekwy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenlongwang.top/gtnbxlhuld.html

Go:   slices.Sort(arr)
来源：http://hz.yuanzhike.top/gtqominsdy.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtsqeytwhm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhaomingkeji.xyz/gttdroepes.html

[N03] 快速排序（分治示例）
来源：http://hz.ppjwa.cn/gtleyxqgxp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtebgeujzv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtgrksvjjs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtukaorkgu.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hongshengwenyu.top/gtcqmytirg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtviuamygz.html


<!-- 参考信息 -->