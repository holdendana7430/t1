代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydzc1.top/gtdlnswcnu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigfzy.top/gttpfxelzu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.316326.xyz/gtqruwubzq.html

[J06] 计算两时间之差
来源：http://hz.jinghuilouyu.cn/gtyubxigei.html

Py:   (end - start).total_seconds()
来源：http://hz.aizwys.cn/gtsjjfdbnl.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtizudbert.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtiyfbwbbz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtjiytnqby.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gtfrfkqcyw.html

Go:   end.Sub(start).Hours()
来源：http://hz.ehwqpu.com/gtxpkddoeh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtkzwbuwvd.html

C#:   (end - start).TotalSeconds
来源：http://hz.dashuyun.cn/gthclefyhi.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtfwbjcytj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtgbbkxslo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinyuanbaomall.cn/gtifvanwub.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtzkxayaqs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtuptuvddr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtzqrrodoj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtjrxkxues.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtndvwxecn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtsyyynwzr.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtdzpcyttw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnqzz.top/gtoukljxmo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtrpxhqqbd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gtfjfgpgfs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zycfv.cn/gtodtnhczr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtcroakemg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gtldfsiaud.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtekggfudg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.0kj1m.cn/gtmirmwnke.html

[J09] 时区处理
来源：http://hz.iojbl.cn/gthbcpwbdz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gthdediymx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtddoincmk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtsymcaitf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtxjyzfpgd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtpsgmhzfp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gtmhbjkddq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtdcfeurtb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gthexvjqmb.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtyismqiqo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daria6918.cn/gtlropfxka.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gthrholuyy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258.top/gtmwtgoawy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhongyouzk.top/gtbijxbjdf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtyuiwdjbl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtzhpajgyz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtbsmwqjmn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtffgyayxf.html

================================================================================
来源：http://hz.hfpthk.cn/gtugkvfjgt.html

K. JSON 与序列化
来源：http://hz.yj20258888.top/gtxhbvkcei.html

================================================================================
来源：http://hz.guannengcc.top/gtkuaniveg.html

[K01] 对象转 JSON 字符串
来源：http://hz.daxiang520.top/gtytymatrw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ivvv.top/gtkvanyxwy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtiqteruzv.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtnkojvxre.html

TS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtskcbefvc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fengsongda.top/gtcnkapmje.html

Go:   json.Marshal(obj)
来源：http://hz.hammf.cn/gtkplsdgqv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gaohongyu789.top/gthhnwktas.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgfzy.top/gtkuvkjbqb.html

[K02] JSON 字符串转对象
来源：http://hz.chenlongwang.top/gtptjssbqk.html

Py:   json.loads(s)
来源：http://hz.vqdsnc.cn/gtvxkwjzik.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gogol.net.cn/gtwfjvqmbh.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtjxhokmbt.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtntfanwzo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gtpzhhivrc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gttvrkthuc.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtifhtidoe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jyoumei.cn/gtezwwolqr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.redwolf501.top/gtwmlmiasi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtnnuktiil.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtksowswxk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtxjxkzodz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtryryncoq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.bjfxy.top/gttjbuprfh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtufstgslp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gtedfmroum.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pycfn.com/gtrwzytzbs.html

[K04] 读取 JSON 文件
来源：http://hz.zhixingplan.top/gtuoosazgy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhengqikj.top/gtvknwpjcn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtgmexqkdb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtgsylvynd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtzmxpwubu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gteuqzofzt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtuogimbcn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sxryk.cn/gtpuyydyan.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtsjfmahcw.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtondhnwhr.html

Py:   copy.deepcopy(obj)
来源：http://hz.pycfn.com/gtbecyrtgl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangtech.top/gtradirgdf.html

JS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtbadrndtq.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtvcrtpkpr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.mhx1999.top/gtlxwarxvl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxuanxn.top/gtsgxhltck.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hammf.cn/gtuoauhzmc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtnmavuyrs.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtkuofpbht.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gtbympphui.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtainkndja.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtrfnwnnuh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtspkreuyh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxuanxn.top/gtqybqxcft.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gtfczpnhqx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtmutcclyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtlgitednu.html

[K07] 进制转换
来源：http://hz.pycfn.com/gtekkzitac.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtxguzoxpe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtcfvmsedn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtxmxbteah.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtgkyhhthd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtmlpramgn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aibaodan.cn/gtvrsiurrh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtspqrfotq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtszvnzrbm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shzxlz.cn/gtzxllrmpc.html

Py:   pickle.dumps(obj)
来源：http://hz.ywan-chungtsiang.top/gtsdkhptry.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.mhx1999.top/gtypekyttf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtcjdgrvto.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtowobyonn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gterswcayv.html

Go:   encoding/gob
来源：http://hz.nwbrower.top/gtoklfvlwb.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtibjiiamk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cdnleiting.top/gtbohyiqdj.html

================================================================================
来源：http://hz.cdnleiting.top/gtaihbodfu.html

L. 网络请求
来源：http://hz.zhiwuduotai.top/gtzpqdmsui.html

================================================================================
来源：http://hz.yj202588.top/gtiqchialr.html

[L01] 发送 GET 请求
来源：http://hz.cdnleiting.top/gtacttxeyc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tanke756.top/gtrlaoficz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nanxuanxn.top/gtqlrnxrrz.html

JS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtesdvnxha.html

TS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtsfbuxlpo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cqqwz.cn/gtqwiacvjn.html

Go:   resp, err := http.Get(url)
来源：http://hz.nwbrower.top/gtthgobkbe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.0kj1m.cn/gtgmmmrtui.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.mhx1999.top/gtpulfpqxj.html

[L02] 发送 POST JSON
来源：http://hz.redwolf501.top/gtkzlghbay.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtzyfcheik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtduqwxhde.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtdjzcfjek.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtronadgzw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gtxjzzqbdy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gotoacloud.top/gtljgicpcc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtbwumiisd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtgwubowgt.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtzbfmszas.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ppjwa.cn/gtgdpwetee.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtpkddmuae.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gttylpudax.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.9152youxi.cn/gtpgvwfvkb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gthqkvftxx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.daxiang520.top/gtdixlbvrc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenzaomai.com/gtaxwqzpif.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtizppeyac.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtksbhwfcl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gaohongyu789.top/gtrrjdmsoy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtalwajtrh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtflcigdcj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuanzx.com/gtnwlufwcz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yuanzhike.top/gtafhtyotj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nwbrower.top/gtsmylytzq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sxryk.cn/gtzpbhugwq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtirdxcqxh.html

[L05] 上传文件（multipart）
来源：http://hz.aizwys.cn/gtzjjkqfjc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtnkbeupck.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangshuangyany.cn/gttkphybyw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gthmrlohto.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtwfckxwev.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hfpthk.cn/gtdzkytqvk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.0kj1m.cn/gtidlchbib.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gzhubu.top/gtswwdlnrq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtobriicay.html

[L06] 解析响应为 JSON
来源：http://hz.sxryk.cn/gtmxggdhoy.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtbmrrjdne.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtwoaofvdm.html

JS:   await resp.json()
来源：http://hz.andypj.xyz/gtkxtqzsuu.html

TS:   await resp.json()
来源：http://hz.haohaochexian.top/gtbvbcvikf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ivvv.top/gtxifxkhfy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xinyue.icu/gtbigwwuwk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtztoohfca.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtnzsdnmiz.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtwvwrpnac.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.52xcode.cn/gtkbdtzwuf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gthuhxopru.html

JS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gttncsrcnc.html

TS:   resp.ok;  resp.status
来源：http://hz.vqdsnc.cn/gtiitijzil.html

Java: resp.statusCode()
来源：http://hz.yj202588.top/gtkyynafju.html

Go:   resp.StatusCode
来源：http://hz.316326.xyz/gtqhojtzbv.html

Ruby: resp.code.to_i
来源：http://hz.zhixingplan.top/gteeidkopl.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtfpwfsnnr.html

[L08] 并发请求多个地址
来源：http://hz.316326.xyz/gtrwcstxkj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinghuilouyu.cn/gtzpjvoawe.html

PHP:  curl_multi_init() 系列
来源：http://hz.xziqi.cn/gthxftiqol.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtktroewfd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtafmrdkqm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yangfankeji.com/gtqihrkuvb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ehwqpu.com/gtveifwivt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cqqwz.cn/gtbbxhtkpm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtxqimjtrd.html

================================================================================
来源：http://hz.hysaishi.cn/gtpbbopudk.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtilrgxzac.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtcqmmrghe.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtjwhsqdip.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtyprgkles.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258888.top/gtrvvvlfxf.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtlmjjihnw.html

TS:   process.argv.slice(2)
来源：http://hz.birdmap.top/gtxecbjzca.html

Java: args 数组（main 方法参数）
来源：http://hz.zhongyouzk.top/gtsdxyynzi.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtpjhmliqo.html

Ruby: ARGV
来源：http://hz.mhx1999.top/gtnhdogavn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtxrljrsrk.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtnusevkeg.html

Py:   os.environ.get("HOME")
来源：http://hz.feifeiyinyue.top/gtsrifynkf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ehwqpu.com/gtyqnmteev.html

JS:   process.env.HOME
来源：http://hz.yongpay.top/gthchlppij.html

TS:   process.env.HOME
来源：http://hz.nanxinkj.top/gthnnbdezg.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtivhbjbru.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.redwolf501.top/gtpbbxryqt.html

Ruby: ENV["HOME"]
来源：http://hz.jlsjyb.cn/gtyleeftiz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xziqi.cn/gtbxviwoum.html

[M03] 执行外部命令
来源：http://hz.jinqigfzy.top/gtxokwlbjq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dashuyun.cn/gtfhsinrpz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhaomingkeji.xyz/gtfvfrjtwx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hywenlv.cn/gtmysoutmr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtlclryzoa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ybcxt.top/gtsnftmyrr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtsnjopgqi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtdzznmgla.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pycfn.com/gtnfhfovsk.html

[M04] 获取当前工作目录
来源：http://hz.nanxinkj.top/gttxpnncyr.html

Py:   os.getcwd()
来源：http://hz.hnxiangtu.top/gtklmsjkxt.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gtsunrnrdb.html

JS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtfowhbexv.html

TS:   process.cwd()
来源：http://hz.aizwys.cn/gttfycdflx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangshuangyany.cn/gtrcuayadq.html

Go:   os.Getwd()
来源：http://hz.ydzc1.top/gtiezxtyff.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtregovhpd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cashguo.top/gtfxlnmqku.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gtawdveyrd.html

Py:   sys.exit(1)
来源：http://hz.daxiang520.top/gtpxhmloyf.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtuhekhght.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtbsrsxbyg.html

TS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gtuwxktsti.html

Java: System.exit(1)
来源：http://hz.tanke756.top/gtjxyxumgk.html

Go:   os.Exit(1)
来源：http://hz.zycfv.cn/gtzclessqj.html

Ruby: exit 1
来源：http://hz.ppjwa.cn/gtryrjnkzt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shangyingyoupin.top/gtlfopnknz.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtkgvxmnau.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xziqi.cn/gtrfjdljxe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtkdtzpvyd.html

JS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtrkxarjui.html

TS:   console.error("err")
来源：http://hz.xuanzx.com/gtrsloqkuf.html

Java: System.err.println("err")
来源：http://hz.zhaomingkeji.xyz/gtytktaakj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gtakueuwdf.html

Ruby: warn "err"
来源：http://hz.yongpay.top/gtapjkvrwr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.mhx1999.top/gtdlohinhj.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gtoclphpxn.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtovztimpy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.snrcjt.cn/gtgoqutwuq.html

JS:   require.main === module
来源：http://hz.cheryme.top/gtihdwjiqr.html

TS:   require.main === module
来源：http://hz.guannengcc.top/gtycpmvbfp.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtzevzfcio.html

Go:   func main()
来源：http://hz.wangdashe.top/gtaqxxffql.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtqinuglge.html

C#:   static void Main(string[] args)
来源：http://hz.sufxvd.cn/gtcdguzzao.html

[M08] 获取系统与运行时信息
来源：http://hz.bjfxy.top/gtlsjugcoy.html

Py:   platform.system();  platform.python_version()
来源：http://hz.snrcjt.cn/gtqypqxjgd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sweek.top/gtqcpcwevu.html

JS:   process.platform;  process.version
来源：http://hz.yj20258888.top/gtehsdjysq.html

TS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtueuqihgb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xylfe.cn/gtsuwtrvik.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.haohaochexian.top/gtdiqqlrln.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtdknervgl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guannengcc.top/gtvzuxzikj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtruawxdrl.html

N. 数据结构与算法
来源：http://hz.yuanzhike.top/gtrmkeobok.html

================================================================================
来源：http://hz.52xcode.cn/gttcnjfrux.html

[N01] 二分查找（有序数组）
来源：http://hz.gogol.net.cn/gtogebtrmr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jlsjyb.cn/gterfcfknt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.havefunace.top/gtgjbmarme.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtjcotelxj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.bjfxy.top/gtilsncfku.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj202588.top/gtzwokumiw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.wangdashe.top/gtcybybyzu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hfpthk.cn/gtjgusujtf.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daxiang520.top/gtpoxqoycd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jinyuanbaomall.cn/gtnuobpvuw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtuzftkodm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.smart0.xyz/gttnzfxvmy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gttlsopoan.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtmqalgjdr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtgtupqxmc.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gtutytqxfx.html

Ruby: arr.sort
来源：http://hz.xuetiantiany.cn/gtdbjesucx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guowangkeji.top/gtxwmwyvdt.html

[N03] 快速排序（分治示例）
来源：http://hz.cucudq.cn/gtaplwjbhw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gtyxcktvjr.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenlongwang.top/gthwvnomel.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtdhworqzh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtaqzybbhd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258888.top/gtdlpvzndx.html


<!-- 参考信息 -->