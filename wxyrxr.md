代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gtbzkgdnkb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zdqjudy.top/gtckspohyb.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtxxeiyqlx.html

Py:   now + timedelta(days=7)
来源：http://hz.xuanzx.com/gteppoovbi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.dashuyun.cn/gtenehourc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtpoqgprgs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtxogsfprw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtwouuhgwr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtzvpckvpo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtrehrzhpl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tianlin.xyz/gtgseryqvt.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtaxivjluz.html

Py:   (end - start).total_seconds()
来源：http://hz.xziqi.cn/gtbtmhmece.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtfqganhcy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tanke756.top/gtytzrompv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aibaodan.cn/gtplcpyndx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtrkebemem.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtlkaahzpe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sxryk.cn/gtovustscu.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtlpsukako.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtokgohzhq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtulttwpfs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.meibo888.top/gtigckoanp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhixingplan.top/gtjdaklibq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtthveodtw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhaomingkeji.xyz/gtjclkidfp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gotoacloud.top/gthcyiavnt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtelywrsgp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtekeigfpn.html

[J08] 提取年月日与星期
来源：http://hz.xuanzx.com/gtaigpwxuv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sweek.top/gtyqbvjlsn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtpbdxdttw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zdqjudy.top/gtdjcbluki.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dashuyun.cn/gtcxnjugoq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxinkj.top/gtarjefrzm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gogol.net.cn/gtkaonxxuk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtijzctukd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gtgjdkdatq.html

[J09] 时区处理
来源：http://hz.shzxlz.cn/gtatyoafyp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigufen.top/gtxtyjugvn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.bjfxy.top/gtnrstclnb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtowhptdnb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtjhgvagff.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgufenzy.top/gtainsqciy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pycfn.com/gtyarwgfyo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tianlin.xyz/gtirrncvbv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtxeroelxb.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtlpfvcwqt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtutaemycw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tanke756.top/gtrlrzbfze.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtwlcspirc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtoubfemek.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.mhx1999.top/gtksousrwk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xziqi.cn/gtcfddeqxk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtqcnuplyb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxuanxn.top/gtvtutixgb.html

================================================================================
来源：http://hz.zycfv.cn/gtnmiwvnko.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtvtzeadda.html

================================================================================
来源：http://hz.c1oappe.top/gtthlmocdr.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenjidiqi.icu/gtglhxutmy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.haohaochexian.top/gtxzudggnh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtpqllwtqz.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtuptbagsh.html

TS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtrzitljtn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtbwullznn.html

Go:   json.Marshal(obj)
来源：http://hz.hysaishi.cn/gtmwkguerz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtxypiawun.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtizhgtzmm.html

[K02] JSON 字符串转对象
来源：http://hz.zhaomingkeji.xyz/gtoscfjiar.html

Py:   json.loads(s)
来源：http://hz.xuanzx.com/gtaryoincl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.feifeiyinyue.top/gtvaxlvjdv.html

JS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gthjvztljz.html

TS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtcsxbqzdk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtlqiibipq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtxhgvgqxb.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtywieihiu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yueranfly.top/gtihkhcbrv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gtetohzgof.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtwmaslkyl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtkjfdwfyf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtqgwomnqy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gttrglbnvr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtlcermsiv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jyoumei.cn/gtpcvfxbag.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.iojbl.cn/gtonlsmnhp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.havefunace.top/gtaesxxzcy.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtczbfogce.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtcvpgnwhy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zdqjudy.top/gtmwovphiu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtynjfhutz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtjqhpbpjt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.c1oappe.top/gtvfoyaskn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtwqvmexir.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtuybgvqeu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hysaishi.cn/gtudidmdre.html

[K05] 深拷贝对象
来源：http://hz.snrcjt.cn/gtodfvauuq.html

Py:   copy.deepcopy(obj)
来源：http://hz.ivvv.top/gtdbxhdhgw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtwahpgbqt.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtvabiltrc.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gthorljlqf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtoruoszcg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tianlin.xyz/gtfnropvje.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cqqwz.cn/gtqcbpvjcu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yongpay.top/gtasdrlcgg.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtklvmrfgq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zycfv.cn/gtezcuqfkt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pengpengdd.cyou/gtjotmmyox.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtubqzoino.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gthrxflxnc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhoulong.xyz/gtxqtfikak.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtpfbsbfur.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtueiftjau.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtrcdkdgjy.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtdlzpkgje.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenzaomai.com/gtujybqsjq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.c1oappe.top/gtobzxboni.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtmjsvslsr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtwfyeyzfz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtfirnrjpn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gtgbyciidq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtgjsjsllv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtojwubllb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gthplkxbqr.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtixyvxvtx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cashguo.top/gtjzcdgxae.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.pengpengdd.cyou/gtosmxgwvi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtccfyojtv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtbijqxzjz.html

Go:   encoding/gob
来源：http://hz.dianchejie.cn/gtyteddyjf.html

Ruby: Marshal.dump(obj)
来源：http://hz.jlsjyb.cn/gtlragngmd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gtynqremku.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzphdvkxs.html

L. 网络请求
来源：http://hz.zhengqikj.top/gtrfzxcfoi.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtniirjsjk.html

[L01] 发送 GET 请求
来源：http://hz.cdnleiting.top/gtkzkoexyb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgufenzy.top/gtkhkozosc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.9152youxi.cn/gtqlpbjsco.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtnfbicncp.html

TS:   await fetch(url)
来源：http://hz.gogol.net.cn/gtwqrbcjqn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tianlin.xyz/gtywkbivxw.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhengqikj.top/gtsytugbzw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gtnlaukauz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cucudq.cn/gtknwzotff.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtosdspyop.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtcwpliyfd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gttpnrigxp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenjidiqi.icu/gtishhfhhe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtipauxaho.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtajsvbibo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aizwys.cn/gtqvhfbgxa.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtwxrwsslb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cashguo.top/gtfmxbxvxn.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtvalglacz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtotqzhlgd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtebrfxips.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtgcodfacc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtyssqrlyx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtlnqliqas.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtukcxdody.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtzwuicbzl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtjrarqwxi.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtmisopqyp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gthbzocweb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gtyqulvzzg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ivvv.top/gtkftfoian.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtxsweeuzq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.quarkkingdee.top/gttgdtormp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuxming.cn/gtbljonblh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtpxwjerdp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sweek.top/gtzsecneex.html

[L05] 上传文件（multipart）
来源：http://hz.zhoulong.xyz/gtbqjqrssi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.iojbl.cn/gttwyhygrj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhengqikj.top/gtwduvfven.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtygwwamge.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtqmbxgjfw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jianghu66.top/gtovzddhya.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gtzxaqfmia.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuanzhike.top/gtxtglgkko.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtigdzates.html

[L06] 解析响应为 JSON
来源：http://hz.guowangkeji.top/gtlrwhvauy.html

Py:   resp.json()
来源：http://hz.aizwys.cn/gtxqwkdbzl.html

PHP:  json_decode($body, true);
来源：http://hz.jinyuanbaomall.cn/gtvjtwvhxv.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtieeterfd.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtomcgvnxc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.52xcode.cn/gtgojjlnap.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ehwqpu.com/gtpilfayhe.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtjyilrkel.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnxiangtu.top/gtauhwbtwn.html

[L07] 处理 HTTP 状态码
来源：http://hz.hywenlv.cn/gtvezudhbc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gtxtnvsdeb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cucudq.cn/gtkybajnjq.html

JS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtsquyehlc.html

TS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gtdyydsahe.html

Java: resp.statusCode()
来源：http://hz.0kj1m.cn/gtzxgwcrke.html

Go:   resp.StatusCode
来源：http://hz.chenzaomai.com/gtbuxdvvua.html

Ruby: resp.code.to_i
来源：http://hz.ydzc1.top/gtyaoycyov.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gtezbbjiqc.html

[L08] 并发请求多个地址
来源：http://hz.dashuyun.cn/gtmrnafymz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydjk.org.cn/gtmxhavssc.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenlongwang.top/gtrssojxol.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtiyawqnrl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gttkjsober.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gtpvycyvkt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtvvsfazdq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fengsongda.top/gtykefiacf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhiwuduotai.top/gtneejeznn.html

================================================================================
来源：http://hz.chenzaomai.com/gtaznzcdsi.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gteziyyskf.html

================================================================================
来源：http://hz.xylfe.cn/gtnswemeda.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gtepnscozp.html

Py:   sys.argv[1:]
来源：http://hz.yongpay.top/gthfhcjnaz.html

PHP:  $argv;  $argc;
来源：http://hz.chenlongwang.top/gtyfgiouuk.html

JS:   process.argv.slice(2)
来源：http://hz.jyoumei.cn/gtjneexcqk.html

TS:   process.argv.slice(2)
来源：http://hz.ehwqpu.com/gtxzugwtcz.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtwlhfwwit.html

Go:   os.Args[1:]
来源：http://hz.ybcxt.top/gtkikhgkfw.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtbylqrkix.html

C#:   args 数组（Main 方法参数）
来源：http://hz.kuanghao11.cn/gtmhoavvld.html

[M02] 读取环境变量
来源：http://hz.yuanzhike.top/gtboyhcqhw.html

Py:   os.environ.get("HOME")
来源：http://hz.shzxlz.cn/gtiltjjxie.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtxemdjgan.html

JS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtebdxsezg.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtxruxgfog.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtixghycda.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gttlhuzfyb.html

Ruby: ENV["HOME"]
来源：http://hz.chenlongwang.top/gtvwuoajkn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtvubsnatl.html

[M03] 执行外部命令
来源：http://hz.xingfuxueyuan.xyz/gtvhnmnzcl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangkeji.top/gtypgthcqd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtzhrtture.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gthyzdpwte.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gttjyusnhl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.316326.xyz/gtzhavsjmf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jyoumei.cn/gtrzrwjgqx.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangdashe.top/gtkbjpwlsb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cqqwz.cn/gtpwdguhlh.html

[M04] 获取当前工作目录
来源：http://hz.cqqwz.cn/gtookodshy.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtzdgyejtt.html

PHP:  getcwd();
来源：http://hz.havefunace.top/gtdwppcxwf.html

JS:   process.cwd()
来源：http://hz.hywenlv.cn/gtxpyxcaih.html

TS:   process.cwd()
来源：http://hz.xylfe.cn/gtcrdpzjnh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daxiang520.top/gtrvnngtju.html

Go:   os.Getwd()
来源：http://hz.ybcxt.top/gtjtlnhokb.html

Ruby: Dir.pwd
来源：http://hz.jqgfzy.top/gtvimqbgxm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuetiantiany.cn/gtaqdmiskb.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtbtnmafgj.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtrfjcbunk.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtaeuqutwc.html

JS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtflncouyj.html

TS:   process.exit(1)
来源：http://hz.yvedp.cn/gtuiszfcar.html

Java: System.exit(1)
来源：http://hz.zhengqikj.top/gtydyltgaj.html

Go:   os.Exit(1)
来源：http://hz.ehwqpu.com/gtevtlznts.html

Ruby: exit 1
来源：http://hz.ywan-chungtsiang.top/gtasqrajva.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gtraoazewz.html

[M06] 向标准错误输出
来源：http://hz.jianghu66.top/gtyhjqdlpy.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhiwuduotai.top/gtzpaaqdgc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.birdmap.top/gtgztfdaav.html

JS:   console.error("err")
来源：http://hz.iojbl.cn/gtxrsjkqyi.html

TS:   console.error("err")
来源：http://hz.havefunace.top/gtljxqlwoi.html

Java: System.err.println("err")
来源：http://hz.zhixingplan.top/gtozhxyrah.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtnxvwodkr.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtuficxggk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gtmkajulzy.html

[M07] 判断是否为主入口
来源：http://hz.tian-w.cn/gtubkjkczn.html

Py:   if __name__ == "__main__":
来源：http://hz.meibo888.top/gttrivqqjb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shuidangran.top/gtqnfvpfuj.html

JS:   require.main === module
来源：http://hz.jqgfzy.top/gtzadmvlcp.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gtiqhyomyh.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtztqgprwm.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtwducigbd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtifontjlh.html

C#:   static void Main(string[] args)
来源：http://hz.cucudq.cn/gtcbzqziqi.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtqqvgmkli.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yj202588.top/gtsfvkaklr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj20258888.top/gtzxhgtozz.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gthoahtgmo.html

TS:   process.platform;  process.version
来源：http://hz.dashuyun.cn/gtdneptjpo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.redwolf501.top/gtwetgbahu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jiagoushi.top/gtecimvwvb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtsutjtifx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cucudq.cn/gtknasmtxl.html

================================================================================
来源：http://hz.sysykeji.top/gtulonyccc.html

N. 数据结构与算法
来源：http://hz.gotoacloud.top/gtowqbkzlw.html

================================================================================
来源：http://hz.yuanzhike.top/gtkedjzqnc.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtjsuyybvt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sweek.top/gtwfzluzbd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yonumen.top/gtvixcmbua.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtdcckrgqk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gttpgbbzdx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xinyue.icu/gtfsnkexcb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtatlpylrt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.bjfxy.top/gtaxwwuwpe.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ppjwa.cn/gtjcljavcq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shanyushiyangtech.top/gtltxyjccj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtswemybgc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hysaishi.cn/gtquxorjff.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtebrdmrus.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtgsyiomeb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtnaflkcjm.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtzaduuwrt.html


<!-- 参考信息 -->