代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtjhcvnkta.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhongyouzk.top/gtcwnduxta.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hywenlv.cn/gtyjohjgsv.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtudkoemhu.html

Py:   (end - start).total_seconds()
来源：http://hz.smart0.xyz/gthskilicm.html

PHP:  $end->diff($start)->days;
来源：http://hz.gogol.net.cn/gtysebpova.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtymnivoie.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guowangkeji.top/gtpgqaxdtv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gthmowlgmf.html

Go:   end.Sub(start).Hours()
来源：http://hz.c1oappe.top/gtexheqseh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtnngnrplc.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtnztgoxan.html

[J07] 比较两个日期
来源：http://hz.hfpthk.cn/gtgthmjupj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtcypdrtnp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shzxlz.cn/gtwvbekhvo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtbdrkocnr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtjkghicei.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtsdmmodlw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xylfe.cn/gtyxvwbtnn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gthhqkvqvn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtspgbycje.html

[J08] 提取年月日与星期
来源：http://hz.chenzaomai.com/gtutqlfece.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigufen.top/gtrqabnvuc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtpyfeqmdg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtwnftuzma.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtcruqwzxk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gtvgyqyubd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtcnhwsepr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pycfn.com/gtxynjuuaj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuetiantiany.cn/gtmokibzru.html

[J09] 时区处理
来源：http://hz.yj202588.top/gtyikytouh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtbnwxjnsq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yongpay.top/gtvfiwesdu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtbhbtoygw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtodijgckl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gteokfzqdr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtrdpujcmn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sxryk.cn/gtaqpvixmo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.bjfxy.top/gteqbrfuxa.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtqycircfs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtsmnfnaek.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.havefunace.top/gtbvrjqbre.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.meibo888.top/gtbeehtuyh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.birdmap.top/gtvrsuqrsw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fzhhl.top/gtctlglpgt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgufenzy.top/gtvoehqjew.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtcwsirrce.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtylpgvttv.html

================================================================================
来源：http://hz.yanxiufei.cn/gtbfvmzojk.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtphrckdqc.html

================================================================================
来源：http://hz.gotoacloud.top/gtkdcisbwb.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtucovvkyz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtpxwerbrm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtxynsujgt.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtkdfjrdqk.html

TS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtkfjwxmiz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtgvrzvlkx.html

Go:   json.Marshal(obj)
来源：http://hz.jqgufenzy.top/gtwpueygoz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.mhx1999.top/gtgtlucciv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtqtrsdcmg.html

[K02] JSON 字符串转对象
来源：http://hz.xingfuxueyuan.xyz/gtwfvglsdw.html

Py:   json.loads(s)
来源：http://hz.yongpay.top/gttkoadzsp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtkircudpc.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtoxyrrvsw.html

TS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtucxpguoe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sysykeji.top/gteyngleba.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtzxsptnyv.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtisdtnihg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gtamyyquyk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangdashe.top/gterjuapbe.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtfxxqxfho.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtagslwrrr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtlrtsbiwe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtosswppfy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fengsongda.top/gtyckybzze.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.mhx1999.top/gtjqgtbvqn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gzhubu.top/gtrwlntszv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtvkpjhhhv.html

[K04] 读取 JSON 文件
来源：http://hz.gogol.net.cn/gtzecgznuo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sysykeji.top/gtoxhzbthw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.snrcjt.cn/gtgtpsxvon.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtbusfqmso.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtrpafqqzr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtqvpkewij.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtcqowdjbq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtsonghlzu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.svipenyu.cn/gtdzarvkeb.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gtafrfrzop.html

Py:   copy.deepcopy(obj)
来源：http://hz.gotoacloud.top/gtoobzvydo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ywan-chungtsiang.top/gtgwlxvuin.html

JS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtvhkvhlxe.html

TS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtenymiznh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigfzy.top/gtxdklsdxy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtyxbcjsqt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtiqtyriba.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gtanyybcea.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gtrodrndze.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtajrklpxh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.svipenyu.cn/gtgraivnpc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtxcksisqv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gttzjywxec.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenjidiqi.icu/gtaiflwlfb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cashguo.top/gtzprlfadh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtzhlvphaa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zdqjudy.top/gtvjrukruf.html

[K07] 进制转换
来源：http://hz.fzhhl.top/gtufrbwfrs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuanzx.com/gttknzmgyt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtanntgdia.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtcpzavnbb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtiylbjlow.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtatskixvz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhengqikj.top/gtaprvdtvh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gthfjiqiov.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtjsaefubd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yvedp.cn/gtemfhcfki.html

Py:   pickle.dumps(obj)
来源：http://hz.cucudq.cn/gtuegijibj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sysykeji.top/gtxdcvfyaz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtzmvstodq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daria6918.cn/gtfvamdhgt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zycfv.cn/gtyyxhsqta.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gtlcmbloiu.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenlongwang.top/gtvnmxbcez.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtpgthxzkl.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtafcoxeqj.html

L. 网络请求
来源：http://hz.yangfankeji.com/gtttqoosuf.html

================================================================================
来源：http://hz.yonumen.top/gteynqwkrl.html

[L01] 发送 GET 请求
来源：http://hz.chenzaomai.com/gtxphhtkwh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhoulong.xyz/gtjzyehpui.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.meibo888.top/gtvpfkvqhe.html

JS:   await fetch(url)
来源：http://hz.yongpay.top/gtssvlepry.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtuedznjyl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtdouyktxh.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtsdkahemk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gtsdollqlf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtuhwbiewd.html

[L02] 发送 POST JSON
来源：http://hz.gotoacloud.top/gtubxjasac.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtutkhuzpq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtomeogbnl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sweek.top/gtuzotuqdv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtwemvhpic.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gthexflxpe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cdnleiting.top/gtdsbvkyby.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtycltxfir.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenlongwang.top/gtffdvbeal.html

[L03] 设置自定义请求头
来源：http://hz.quarkkingdee.top/gtzfktufnd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gthfulcnmt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xuetiantiany.cn/gtnlwwflfa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtfmqgxlqv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtuqhwasmh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gtychivxou.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtrvgpkgxc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dianchejie.cn/gtntvuszzd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jianghu66.top/gtdmphlsho.html

[L04] 设置超时
来源：http://hz.guowangkeji.top/gtymjzmczk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhengqikj.top/gttimksqkm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.svipenyu.cn/gtmjvixhrw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtlditdhpn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtgcemvfad.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtuxvcizcn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gtjijgqnxn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ehwqpu.com/gtuosdqemn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ybcxt.top/gtaxizuhgv.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtgkvwlhal.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.vqdsnc.cn/gtlvzvrshe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhengqikj.top/gtutuxvbqy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtbcodsznb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtureiczjn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuxming.cn/gtbmhmoifv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenjidiqi.icu/gtmvenelxm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenlongwang.top/gthpsdxnwd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.c1oappe.top/gtkpmwzfup.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtzbdkiyth.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtsltekbou.html

PHP:  json_decode($body, true);
来源：http://hz.hnxiangtu.top/gtvwltczye.html

JS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtgigtixnq.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtzgbrdvbj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ivvv.top/gtnrsjnhan.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.vqdsnc.cn/gtdwlajxgg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gtwplpldwj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yj20258888.top/gtdciiiskh.html

[L07] 处理 HTTP 状态码
来源：http://hz.snrcjt.cn/gtvlqhbctw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigfzy.top/gtpsdtugpi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtnbztqsmm.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtiscwgwzy.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gthpyssigi.html

Java: resp.statusCode()
来源：http://hz.cqqwz.cn/gthgkjttid.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtjpmuvyre.html

Ruby: resp.code.to_i
来源：http://hz.daxiang520.top/gthmmaogqy.html

C#:   (int)resp.StatusCode
来源：http://hz.xziqi.cn/gtkecnpfvd.html

[L08] 并发请求多个地址
来源：http://hz.cheryme.top/gtkljeyezu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.0kj1m.cn/gtuqwsxbqx.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtqctbgkvi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtjywgleqd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gtvzppmgkk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sweek.top/gtxqirdrfo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fengsongda.top/gthpkvpccz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtdjrvyubv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jlsjyb.cn/gtmzncpeeo.html

================================================================================
来源：http://hz.jianghu66.top/gtffdubylw.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtszkuzuak.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmsycadvx.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtjvablzjh.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gthdncgixa.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258888.top/gtgdxcxtle.html

JS:   process.argv.slice(2)
来源：http://hz.shanyushiyangkeji.top/gtntlqyoby.html

TS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtzqjsgiip.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gtnbmfhrqv.html

Go:   os.Args[1:]
来源：http://hz.wangdashe.top/gtbpgytfta.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtibjfnxic.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtluunempp.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gtffkptjow.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtjfbfpxll.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.quarkkingdee.top/gtpzabbxcn.html

JS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtgguydlto.html

TS:   process.env.HOME
来源：http://hz.hywenlv.cn/gttzgzzven.html

Java: System.getenv("HOME")
来源：http://hz.aizwys.cn/gtgcbpkcut.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtjtrgcurj.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtsfkogluf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gtodkfkanx.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtbtwivzlx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtatzzfulc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sysykeji.top/gtptnotgwp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhaomingkeji.xyz/gtodmbjhjt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtkgvfgdsz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtysqvwscb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jiagoushi.top/gteuqiaytb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ppjwa.cn/gtmtgvkaad.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xziqi.cn/gtttdqkamm.html

[M04] 获取当前工作目录
来源：http://hz.yj20258.top/gthsirjdfm.html

Py:   os.getcwd()
来源：http://hz.fzhhl.top/gtsoapoqir.html

PHP:  getcwd();
来源：http://hz.yonumen.top/gtopuwxxwf.html

JS:   process.cwd()
来源：http://hz.guowangkeji.top/gtbidjptcf.html

TS:   process.cwd()
来源：http://hz.jyoumei.cn/gtlwodliiu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtkvucfmhd.html

Go:   os.Getwd()
来源：http://hz.yj20258.top/gtiqijcjmr.html

Ruby: Dir.pwd
来源：http://hz.nanxinkj.top/gtwkesnvll.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hfpthk.cn/gtulrcuacm.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtdsiarbez.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtfydsthem.html

PHP:  exit(1);
来源：http://hz.jyoumei.cn/gtynheiisg.html

JS:   process.exit(1)
来源：http://hz.redwolf501.top/gtoocyhvew.html

TS:   process.exit(1)
来源：http://hz.52xcode.cn/gtbvbyszxl.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gttrufmlie.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtyquvsjxc.html

Ruby: exit 1
来源：http://hz.0kj1m.cn/gtojrpcssh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangkeji.top/gtamvcgazc.html

[M06] 向标准错误输出
来源：http://hz.zhengqikj.top/gtzxmlrigp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtenztskkq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yongpay.top/gtaxkwgqbu.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtgigjmuqd.html

TS:   console.error("err")
来源：http://hz.zdqjudy.top/gtzanffbqg.html

Java: System.err.println("err")
来源：http://hz.shzxlz.cn/gtockpzwow.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nanxuanxn.top/gtbhvsfnfb.html

Ruby: warn "err"
来源：http://hz.jyoumei.cn/gtxthjwbtg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangkeji.top/gtdnxaoxlx.html

[M07] 判断是否为主入口
来源：http://hz.tianlin.xyz/gtzhdyminj.html

Py:   if __name__ == "__main__":
来源：http://hz.ehwqpu.com/gtuftvuwxa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tanke756.top/gtlvyvmyeg.html

JS:   require.main === module
来源：http://hz.sxryk.cn/gtdzmrsagr.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtlxrjwcjg.html

Java: public static void main(String[] args)
来源：http://hz.jinqigfzy.top/gtfpbzucql.html

Go:   func main()
来源：http://hz.sufxvd.cn/gthbrsxndq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtiadpmzwd.html

C#:   static void Main(string[] args)
来源：http://hz.tanke756.top/gtlziixvwk.html

[M08] 获取系统与运行时信息
来源：http://hz.ivvv.top/gtxmdtlvyf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.birdmap.top/gtuvsyersj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtmqxaikon.html

JS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtxzflujnb.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtbvdycosp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnxiangtu.top/gtiusbggcj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gteyqsfcbh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gotoacloud.top/gtkluwyila.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gotoacloud.top/gtmjxqshuh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwiahdlbz.html

N. 数据结构与算法
来源：http://hz.aibaodan.cn/gtnwdcxadq.html

================================================================================
来源：http://hz.jqgfzy.top/gtkuhvvrcz.html

[N01] 二分查找（有序数组）
来源：http://hz.daxiang520.top/gtzvqwicfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.dianchejie.cn/gtffjglgec.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shanyushiyangkeji.top/gtctcejbwh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtdjzqstvj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxinkj.top/gtbnexzvzk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.meibo888.top/gtitwkvuri.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jlsjyb.cn/gtqyotconm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.shanyushiyangtech.top/gtnisffdwt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gthmxoiqmf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sysykeji.top/gtnxmpuhas.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtjbeuvcqc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinyuanbaomall.cn/gtowcjxepx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gthgwhufdm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtnwsrssab.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtzobqiwqu.html

Go:   slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtjmnklnyi.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtjqnpxtqi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangtech.top/gtyxbwlwow.html

[N03] 快速排序（分治示例）
来源：http://hz.zhiwuduotai.top/gtdmoeqegc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinyuanbaomall.cn/gtwosxtlzr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nwbrower.top/gtylfjzpwo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.52xcode.cn/gtzjlusnqw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtsqcdgiua.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtgnpqjiwx.html


<!-- 参考信息 -->