代发 wailian999

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gtkmcvuzde.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtkcvoignn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtlzdmiaie.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtnlgjjmni.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtesqfeswp.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtlkgjuzew.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gtlqbemcoo.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gthurvjcfx.html

[J07] 比较两个日期
来源：http://hz.cheryme.top/gtwfkxsrsh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtcougsgno.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtmnbtkwiy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtsfkmqlwn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtptmiyxio.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nwbrower.top/gtlfmdjvni.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258.top/gtnzngymba.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtptwxurvx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtimogfwti.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gtucqfwyrq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhiwuduotai.top/gtuijtdoti.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtguqhowwz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtqmfyoyoq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtrwkvgodz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtkvuqfzck.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangshuangyany.cn/gtuqnyxscr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtrygoktwa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gtplitvsxu.html

[J09] 时区处理
来源：http://hz.chenjidiqi.icu/gtmeygmagv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tanke756.top/gtevgherwe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.9152youxi.cn/gtpexxcqbf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gthssnstif.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtinqziugw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gttlrpybsp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jianghu66.top/gticfugkpb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.pengpengdd.cyou/gtwmiasuzi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.kuanghao11.cn/gtehumqqtm.html

[J10] 取今天 / 本月第一天
来源：http://hz.aizwys.cn/gtknriigew.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gtktnzocto.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hysaishi.cn/gtxpfbfjka.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtspuywoip.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cheryme.top/gtvdzqtelm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtxtlefcnc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtidtorzzg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yonumen.top/gtfbymvzca.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tanke756.top/gtwminrqyf.html

================================================================================
来源：http://hz.c1oappe.top/gtsddqcuch.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtjqshnidm.html

================================================================================
来源：http://hz.sysykeji.top/gtqeczsqcf.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtwdzfiurj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtxedovnbl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtvjwsbqvv.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtnaxfhbhx.html

TS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtmlqppdte.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhongyouzk.top/gtavvvoygx.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtuybkzcwj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtpyqgwcmy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guannengcc.top/gtsfbfpqds.html

[K02] JSON 字符串转对象
来源：http://hz.jianghu66.top/gthqmpedyk.html

Py:   json.loads(s)
来源：http://hz.yuxming.cn/gtdonqargp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daria6918.cn/gtmmzdnnjn.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtyiwnuzur.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtbguizkzq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gteqdzqket.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtfhtvoggj.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtzpfjbbqy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtcbhffcbf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtqhtovusc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtflzmjiwu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.svipenyu.cn/gtbzniwiue.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtshuyzbux.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtmtvepwdx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtgcvhqeqs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pengpengdd.cyou/gtyxvyqawr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenlongwang.top/gtaxzpeljd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtfrqfcplx.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtxuoicool.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtlhwwnzge.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtzcdscrjk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtslcfqaie.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtfquzlxas.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangkeji.top/gteubcbzth.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gttbnrbzkf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gtsregerbf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtdcdmlabu.html

[K05] 深拷贝对象
来源：http://hz.shangyingyoupin.top/gtqulnhqvh.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gtwkuyqnjx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtfieknzud.html

JS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtmovojtkf.html

TS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtfjfdbwrl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtffyqeinb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtsoywnmxk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aibaodan.cn/gtheyakhgq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cdnleiting.top/gtrlizfjoh.html

[K06] 解析 URL 查询串
来源：http://hz.yonumen.top/gtumikxtju.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtibupcmie.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.haohaochexian.top/gtdmtoynox.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtjsaabcez.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtibtnhtdk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zdqjudy.top/gtqzwbimwt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sysykeji.top/gtiscrzwnf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gthpbgeept.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtnywmhfdz.html

[K07] 进制转换
来源：http://hz.fengsongda.top/gtgmipnozw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnxiangtu.top/gtoigrouuv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cashguo.top/gtmprgdaga.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtmuehhlmr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtzhbxldzn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtkiaamedk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxuanxn.top/gtrefxspcd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtggqnzxtf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xylfe.cn/gtvvdgyghn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gtrgwczpul.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtoofzeifi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtlolujkwd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtojbcxmhq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtxosvuxxg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.iojbl.cn/gtsvtwcpbh.html

Go:   encoding/gob
来源：http://hz.shanyushiyangtech.top/gtjyfqbfuw.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtermgelkq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtlyolaljf.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpguthlvi.html

L. 网络请求
来源：http://hz.yuanzhike.top/gtrpxnapof.html

================================================================================
来源：http://hz.zhoulong.xyz/gtymwyyuxz.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gttngjfvtb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtklsyqdnm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.andypj.xyz/gtztdssclj.html

JS:   await fetch(url)
来源：http://hz.wangshuangyany.cn/gtxcscryan.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtoogmuwuk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gteavemrvl.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinqigfzy.top/gtjryqjmkt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nanxinkj.top/gtjyjjqqgd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.vqdsnc.cn/gtjmnxudjt.html

[L02] 发送 POST JSON
来源：http://hz.havefunace.top/gtvmncdovw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhengqikj.top/gtvtccuwpj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtmgypbzrg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtmsgkmifp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gttzcrtwld.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.redwolf501.top/gtlhlmrzzr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gtqjtozokq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gttzuvpzbh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.9152youxi.cn/gtpgqpnojd.html

[L03] 设置自定义请求头
来源：http://hz.redwolf501.top/gtmgjcmuth.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtfrtwvisq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxuanxn.top/gtxapjkjuj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigfzy.top/gtxecuveaj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gogol.net.cn/gtlnksxabb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cdnleiting.top/gtabazkkuc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtrlvoyvul.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xziqi.cn/gtcovsieog.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangdashe.top/gtbykuyull.html

[L04] 设置超时
来源：http://hz.ybcxt.top/gtidpeedgs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangshuangyany.cn/gtmkhbiuiu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhixingplan.top/gtqmmgfdmy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtdeuanjym.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtrqijvqnq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtbimshfok.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gzhubu.top/gtbdiapzfi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtrlozizez.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.0kj1m.cn/gtzdvrbhtx.html

[L05] 上传文件（multipart）
来源：http://hz.dashuyun.cn/gtixnoteax.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sweek.top/gtzpdorhcz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.snrcjt.cn/gthmbjaklp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtkqcjlnfp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtzikmdwfj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pycfn.com/gtpfjcqvdt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenzaomai.com/gtkumlagey.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtlhyxwbxp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hysaishi.cn/gtgmexxhrn.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtlyignrqe.html

Py:   resp.json()
来源：http://hz.tianlin.xyz/gtdwcvxspa.html

PHP:  json_decode($body, true);
来源：http://hz.vqdsnc.cn/gtwjajprco.html

JS:   await resp.json()
来源：http://hz.aibaodan.cn/gtfgyqjkdt.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtfmklksjl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.quarkkingdee.top/gtoqhyreoy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtutzvugmx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aizwys.cn/gtbxlynxzk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtmmfgcenr.html

[L07] 处理 HTTP 状态码
来源：http://hz.birdmap.top/gtaeffxgjz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daria6918.cn/gtrzgsvsid.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gttrflisxs.html

JS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtctfflnam.html

TS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gtzahyrtkk.html

Java: resp.statusCode()
来源：http://hz.jqgufenzy.top/gtlwwjqztf.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtupwzdmov.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtunratevl.html

C#:   (int)resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtbasnacjv.html

[L08] 并发请求多个地址
来源：http://hz.feifeiyinyue.top/gtuxwiiupv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shuidangran.top/gtjkclwozo.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtlxucqyiu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenlongwang.top/gtjiowavge.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gtkresvmom.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.52xcode.cn/gtznyklfmi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aibaodan.cn/gtpnlzlsko.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gtehgilddu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtmbezflrf.html

================================================================================
来源：http://hz.zhengqikj.top/gthctshzcm.html

M. 命令行 / 进程 / 环境
来源：http://hz.tian-w.cn/gtdittledz.html

================================================================================
来源：http://hz.ivvv.top/gtmxkhtqhq.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtsvfczrat.html

Py:   sys.argv[1:]
来源：http://hz.fzhhl.top/gtvmeuhyap.html

PHP:  $argv;  $argc;
来源：http://hz.nanxuanxn.top/gtifrqtkkl.html

JS:   process.argv.slice(2)
来源：http://hz.52xcode.cn/gtydspzofh.html

TS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtdthqvqxr.html

Java: args 数组（main 方法参数）
来源：http://hz.cqqwz.cn/gtjlotqfmn.html

Go:   os.Args[1:]
来源：http://hz.aizwys.cn/gtdwonypov.html

Ruby: ARGV
来源：http://hz.yvedp.cn/gtpurvjhyx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.fengsongda.top/gtvkrramnc.html

[M02] 读取环境变量
来源：http://hz.tian-w.cn/gtuglheokd.html

Py:   os.environ.get("HOME")
来源：http://hz.yuxming.cn/gtieybtvpr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.svipenyu.cn/gtwfhovvwd.html

JS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtahtbkolg.html

TS:   process.env.HOME
来源：http://hz.mhx1999.top/gtrwllxxrj.html

Java: System.getenv("HOME")
来源：http://hz.aibaodan.cn/gtpfffthjl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhongyouzk.top/gtvdhpxwin.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258888.top/gtactmwxku.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zdqjudy.top/gtksswutde.html

[M03] 执行外部命令
来源：http://hz.gzhubu.top/gtjxffbnjo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gtrvliovww.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtvxndiypm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtstcnshqi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtxfbnntrs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhengqikj.top/gtgftzdpap.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yanxiufei.cn/gticdtrbla.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtrybiukbr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ybcxt.top/gtmjpsfhlr.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gthfpqkgax.html

Py:   os.getcwd()
来源：http://hz.bjfxy.top/gtkejjrukb.html

PHP:  getcwd();
来源：http://hz.jyoumei.cn/gtngzwrrwr.html

JS:   process.cwd()
来源：http://hz.aibaodan.cn/gtzsdsurgt.html

TS:   process.cwd()
来源：http://hz.jiagoushi.top/gtfmyzsryp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinghuilouyu.cn/gtydggspui.html

Go:   os.Getwd()
来源：http://hz.xuanzx.com/gtspyrehar.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtfzgdgxbd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtbvxrlvar.html

[M05] 设置退出码
来源：http://hz.xuanzx.com/gtssrxjidz.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtdnnhqxkf.html

PHP:  exit(1);
来源：http://hz.shanyushiyangtech.top/gtrfhiqnww.html

JS:   process.exit(1)
来源：http://hz.hfpthk.cn/gtlrpamppq.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtwjttoopq.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtjvuzrbvi.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtfkponnmf.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtzlnoygja.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtuyyphtea.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gtqxrzqffm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtuvkpakqq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtdzhfsfpe.html

JS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtpeaodtku.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtatqpuiar.html

Java: System.err.println("err")
来源：http://hz.shangyingyoupin.top/gtvjanxyvj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtaygcdvwv.html

Ruby: warn "err"
来源：http://hz.ybcxt.top/gtzxqnilez.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydzc1.top/gtalcrkwmh.html

[M07] 判断是否为主入口
来源：http://hz.dianchejie.cn/gtzukunhtc.html

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtkpvpmpsm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtxdfbnujz.html

JS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtretrwdiv.html

TS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtuflazres.html

Java: public static void main(String[] args)
来源：http://hz.wangdashe.top/gtbxrjzaix.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtefkcjzll.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jqgufenzy.top/gtvehuchdi.html

C#:   static void Main(string[] args)
来源：http://hz.snrcjt.cn/gtbxhngywk.html

[M08] 获取系统与运行时信息
来源：http://hz.yongpay.top/gtwnrtwvhl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtzpskokdv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuanzx.com/gtlcqznsmj.html

JS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gthhrmeutm.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtkxquhhby.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gthsuozcsu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.9152youxi.cn/gtuvzmhevo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daxiang520.top/gtehulhwxf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.c1oappe.top/gtxgtgljiu.html

================================================================================
来源：http://hz.sysykeji.top/gtjxpegzof.html

N. 数据结构与算法
来源：http://hz.jianghu66.top/gthxzsnrxw.html

================================================================================
来源：http://hz.ivvv.top/gtwjyxluaq.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gtwqlnvlfc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgfzy.top/gtazucvlkx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj202588.top/gtwzyazvab.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtvdznoopo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuanzx.com/gtwbeyqgyh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.iojbl.cn/gtarfnfomb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtazmnsyls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.iojbl.cn/gtjxgzfkdg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtcetwecti.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daria6918.cn/gtpezxdchk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtpebtmtdz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.9152youxi.cn/gtifohcrdd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtmhzhbund.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtoztgdmcz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.iojbl.cn/gtctkyyava.html

Go:   slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gteceiskwg.html

Ruby: arr.sort
来源：http://hz.chenlongwang.top/gtaeokqjmr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.daria6918.cn/gtiaresysr.html

[N03] 快速排序（分治示例）
来源：http://hz.bjfxy.top/gtfmwojanv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.snrcjt.cn/gtjikosetf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gtncpryzbs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtcgwjbxzc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtyypqhubp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ehwqpu.com/gtdusuyigj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gtmukwsajo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jiagoushi.top/gtxxtzhujp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pengpengdd.cyou/gtnavmfrzy.html

[N04] 斐波那契数列
来源：http://hz.ybcxt.top/gtchcnocny.html


<!-- 参考信息 -->