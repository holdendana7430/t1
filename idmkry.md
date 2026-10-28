代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtvbzpkjli.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtwzbvympv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtzyayshts.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gtnzqrhdvv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtoxqtlztb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtunzaqeqa.html

[J05] 时间加减（加 7 天）
来源：http://hz.fzhhl.top/gtsxijjtex.html

Py:   now + timedelta(days=7)
来源：http://hz.tanke756.top/gtafshckwp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hfpthk.cn/gtmanxqzub.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtjaupuaur.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtsipkqwaq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xziqi.cn/gtudtrgakc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtddltbejj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gticfcqsxf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnxiangtu.top/gtwcbuoold.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gtmsuypdpm.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtdteyqhfp.html

PHP:  $end->diff($start)->days;
来源：http://hz.zdqjudy.top/gtbfhqrmop.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gtjtoucirq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hysaishi.cn/gtfywwtzmu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gttjmpeafm.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gthwgrendq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtrnibkyoz.html

C#:   (end - start).TotalSeconds
来源：http://hz.hywenlv.cn/gtacytftyc.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtbyqyudmq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtwzecgojf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yvedp.cn/gtrubwsiwa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtwdqxvaae.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtynnyvxav.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.0kj1m.cn/gtjnpfwjah.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ybcxt.top/gtkxiwrnaf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtcysvtanm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtyemovazh.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gttuqbfxyc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gteaabanvd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.iojbl.cn/gtvjvfhion.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtvufgimln.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtmuuiletu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.haohaochexian.top/gtzhmrcnki.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhiwuduotai.top/gtvsxlcuho.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gttduxmhdl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxinkj.top/gtyrgczguf.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtrqkufmfu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gtcqzjlihg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jianghu66.top/gtbqvhjxnq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gthouttlse.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtxtjtqthf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hongshengwenyu.top/gtdkgrxlet.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gthzhbsorp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtnhgddjdp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtsnojckxv.html

[J10] 取今天 / 本月第一天
来源：http://hz.birdmap.top/gtoeajfjhx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhixingplan.top/gtgkkdxega.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtrfepntjq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hywenlv.cn/gtyzdgqrze.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tanke756.top/gtiauychjp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ybcxt.top/gteujqtljp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yueranfly.top/gtbwpootww.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtajjtweno.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fzhhl.top/gtldywfouo.html

================================================================================
来源：http://hz.tian-w.cn/gtojfpotzb.html

K. JSON 与序列化
来源：http://hz.yj20258888.top/gtwipoxgjw.html

================================================================================
来源：http://hz.fengsongda.top/gtslfnpaoj.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtmplulztb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yonumen.top/gtupmbmtpe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtmatfrxfy.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtlymjgusp.html

TS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtfwdyyhim.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.9152youxi.cn/gtpgcotksd.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtlpgmwzxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gthrcgfnsz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.smart0.xyz/gtgixsnqip.html

[K02] JSON 字符串转对象
来源：http://hz.guowangkeji.top/gthbeowhpk.html

Py:   json.loads(s)
来源：http://hz.yvedp.cn/gtlglbfqiz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zycfv.cn/gthxbxkbtm.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtydkreonu.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtyddodhsd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtssqikhnl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtazuvqfxr.html

Ruby: JSON.parse(s)
来源：http://hz.zhengqikj.top/gtznfaufpv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cqqwz.cn/gtegskqxer.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xziqi.cn/gtjpxqdxhv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtcsfzcfyt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtcbvyeyrw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nwbrower.top/gtgawibcit.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtfxuirgfo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhengqikj.top/gtsntdrbnd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtjgwkalyq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gthjtcbtkz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shuidangran.top/gtsixmjznr.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtayxisfmk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.kuanghao11.cn/gthrrgueve.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.52xcode.cn/gtvuqumtjx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtjhmkphgg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtxrkytitk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgfzy.top/gtblwgoqiy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtsloaraij.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuxming.cn/gtaawotulj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuanzhike.top/gtgcrmlsde.html

[K05] 深拷贝对象
来源：http://hz.gaohongyu789.top/gtrhvyaifl.html

Py:   copy.deepcopy(obj)
来源：http://hz.tian-w.cn/gtcmwmvckm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hywenlv.cn/gtreuuxdsg.html

JS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtbdsneknl.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtkjlfloka.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtaaftevrp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tian-w.cn/gtootuwwpc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tianlin.xyz/gtgnkhwrdx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtxeokncrl.html

[K06] 解析 URL 查询串
来源：http://hz.guowangkeji.top/gtnwhijdyx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtasqqffoa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yongpay.top/gtevfbpbri.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtrvrqqwni.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtexezcvqq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.andypj.xyz/gtanlaglhy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtzamkvjbf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtimeswuja.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tianlin.xyz/gtwgapqagp.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtdrqmjcoh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yangfankeji.com/gtoypqiqqy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtyrhpiriv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtcodzpbpp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtuzrdapth.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtzwrmhuzu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ybcxt.top/gthslzomjn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuanzx.com/gtqemzpsic.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxinkj.top/gtgrnjtrhh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuanzhike.top/gtghhqhltm.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gtsniaqaga.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cashguo.top/gtstrzxgiz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtkhpfgmqc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtcdttbufu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtkeaemret.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gtlzgslrbe.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtppsnhwyi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuanzhike.top/gtnkzefqkc.html

================================================================================
来源：http://hz.316326.xyz/gtyxwinjbv.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtvcucuidn.html

================================================================================
来源：http://hz.gogol.net.cn/gtjeschcqx.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtisqhwhpy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sxryk.cn/gtfnmbtiua.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigufen.top/gtuepohadt.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtnpnhnfgs.html

TS:   await fetch(url)
来源：http://hz.zdqjudy.top/gtmttbmtbu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cucudq.cn/gtdwyvuemp.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtrvqtjbgh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aibaodan.cn/gterzwoxff.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gogol.net.cn/gtcytrpupo.html

[L02] 发送 POST JSON
来源：http://hz.zhixingplan.top/gtwhvhvtfb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258.top/gtkxwqltkq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fzhhl.top/gtnrswopha.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gthcqcbccj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtibwdjvuw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtxhdpsrzn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangshuangyany.cn/gtmzbyzndp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigufen.top/gtxwrhtzci.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtmnyafyng.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtxgewbysr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daria6918.cn/gtywskpfwy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xziqi.cn/gtwpkswbxr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtryryfvxp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtzhvxqedx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtmwpdztiv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtujogsltt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gtoanreldr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtsppnslwo.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtaqpvvtsj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.meibo888.top/gtdvgsauql.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.c1oappe.top/gtrxskhmot.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtzeilhiyg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtidxsnctl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhiwuduotai.top/gtohwbsxki.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xylfe.cn/gtnzmklepu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtukulmvir.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuanzx.com/gtuzkrsefg.html

[L05] 上传文件（multipart）
来源：http://hz.jqgfzy.top/gtacxevtbg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cucudq.cn/gtaugdcdzg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxinkj.top/gtwkkfyozl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtyvahlbqz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtmeunlzzy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigfzy.top/gtkaruabjv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtilylaziv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daxiang520.top/gtubyzvlob.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuxming.cn/gtdhmmnkxw.html

[L06] 解析响应为 JSON
来源：http://hz.gogol.net.cn/gtsecbjsdg.html

Py:   resp.json()
来源：http://hz.shanyushiyangkeji.top/gtuyvccnvu.html

PHP:  json_decode($body, true);
来源：http://hz.tanke756.top/gtamrijfph.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtehhjqhdo.html

TS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtdbngtwht.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gtcionpdkh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gtxsluaxid.html

Ruby: JSON.parse(resp.body)
来源：http://hz.dianchejie.cn/gtpkfytrhm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hysaishi.cn/gtjuajntzq.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtebmexwru.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtdrboavyt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtmwufozhq.html

JS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtmdpesqcv.html

TS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtktfihlls.html

Java: resp.statusCode()
来源：http://hz.yangfankeji.com/gtblnraper.html

Go:   resp.StatusCode
来源：http://hz.9152youxi.cn/gtmaqwrefk.html

Ruby: resp.code.to_i
来源：http://hz.yangfankeji.com/gtmqgbjsjp.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtalkwoqvg.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gtuvluwqct.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtwteknqzm.html

PHP:  curl_multi_init() 系列
来源：http://hz.daxiang520.top/gtvzkmxixj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtonxlqsmj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtdaqocsas.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtajqugitq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.tianlin.xyz/gtgnrrbvmv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtucgtqajk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.9152youxi.cn/gtwvxrxesw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtdhubjjnd.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtumkswwwk.html

================================================================================
来源：http://hz.sweek.top/gtinuduiqf.html

[M01] 读取命令行参数
来源：http://hz.gotoacloud.top/gtevvgtdvk.html

Py:   sys.argv[1:]
来源：http://hz.chenlongwang.top/gtdcjncfbj.html

PHP:  $argv;  $argc;
来源：http://hz.hywenlv.cn/gtjgrwnlup.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtoqsfuclj.html

TS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtdemkfkgn.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gtlzuppsfr.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtfxmejcry.html

Ruby: ARGV
来源：http://hz.tianlin.xyz/gtxjajvlnr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fzhhl.top/gtwbnsmpbm.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtvphfqmui.html

Py:   os.environ.get("HOME")
来源：http://hz.redwolf501.top/gtdtpgbkvo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cucudq.cn/gthclouguw.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtzpqabuds.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtgyeqdpkt.html

Java: System.getenv("HOME")
来源：http://hz.xinyue.icu/gtjtdyoflm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gttpvxhuqa.html

Ruby: ENV["HOME"]
来源：http://hz.iojbl.cn/gttrynzvbo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cucudq.cn/gtqkjxtjhk.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtznjelyno.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gaohongyu789.top/gtigrirmwz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtvpqmfvpv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.andypj.xyz/gtzzsufywc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtbwuwfsek.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtohrotgzh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtrwofxlwg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.0kj1m.cn/gtmkbytysy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhaomingkeji.xyz/gtmllrklny.html

[M04] 获取当前工作目录
来源：http://hz.jinyuanbaomall.cn/gtbforeynx.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtpkhaozps.html

PHP:  getcwd();
来源：http://hz.nwbrower.top/gttpbxcthc.html

JS:   process.cwd()
来源：http://hz.zdqjudy.top/gtsttbprfx.html

TS:   process.cwd()
来源：http://hz.jinyuanbaomall.cn/gtwmhkxrsp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.redwolf501.top/gtitjazuga.html

Go:   os.Getwd()
来源：http://hz.52xcode.cn/gtyahjjkik.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtcgkyjevh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtpatkvvvg.html

[M05] 设置退出码
来源：http://hz.pengpengdd.cyou/gtbhkhdmfn.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtgtiqygev.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtehjldkxk.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtlcfvqzed.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gthsrpqutf.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtzalnnfvr.html

Go:   os.Exit(1)
来源：http://hz.cashguo.top/gtijpfyiip.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtpauaclum.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hywenlv.cn/gtiltbsmgn.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtdjnfbjko.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenzaomai.com/gtpvqcatty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.quarkkingdee.top/gtfolgtelt.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtnkkzvjid.html

TS:   console.error("err")
来源：http://hz.guannengcc.top/gtawblovyi.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtoreztfdz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cheryme.top/gtrqocsjdr.html

Ruby: warn "err"
来源：http://hz.cashguo.top/gtazequwxu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hysaishi.cn/gtrwmdykki.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gtaeuvnrqm.html

Py:   if __name__ == "__main__":
来源：http://hz.havefunace.top/gtxrqrthst.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gotoacloud.top/gtrwqxkyad.html

JS:   require.main === module
来源：http://hz.aizwys.cn/gtzhxoxlgr.html

TS:   require.main === module
来源：http://hz.zycfv.cn/gthpsalhbf.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtqlcdtvse.html

Go:   func main()
来源：http://hz.guannengcc.top/gtxfcdfmax.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gttisiugaz.html

C#:   static void Main(string[] args)
来源：http://hz.nanxinkj.top/gtrhutipmh.html

[M08] 获取系统与运行时信息
来源：http://hz.shangyingyoupin.top/gtnsspnngn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtlyvxthsu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtblhezfwl.html

JS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtngbyrkvd.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gtkwvejwin.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gtuygzqofu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtqpertffg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtyanpvnbk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.9152youxi.cn/gtugabsbpq.html

================================================================================
来源：http://hz.pycfn.com/gtjjtyywiq.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtqygwrmwt.html

================================================================================
来源：http://hz.bjfxy.top/gtppljawmg.html

[N01] 二分查找（有序数组）
来源：http://hz.shanyushiyangkeji.top/gtfbrzajjw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gthxyflbpg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.kuanghao11.cn/gtrxhhserc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtciuufbej.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gthyvtiyme.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hongshengwenyu.top/gtcrzclwut.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtjfanrvrm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guowangkeji.top/gtwfhrltny.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gttlantncm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gzhubu.top/gthdlbpsyh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtilvmnizw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jyoumei.cn/gtlzyvqfqt.html


<!-- 参考信息 -->