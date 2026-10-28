代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258.top/gtwcjtwjfc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xuetiantiany.cn/gtwoqdwkgm.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtcbrfxugb.html

Py:   now + timedelta(days=7)
来源：http://hz.iojbl.cn/gtmvirjswc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zdqjudy.top/gthmbatgnq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtlhtzgpxm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtcxlkyfut.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydzc1.top/gtafrqtawb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtxxacidtf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtgpcmjbld.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.redwolf501.top/gtyeoxvhto.html

[J06] 计算两时间之差
来源：http://hz.havefunace.top/gtcycfehzf.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtpjrcbtfu.html

PHP:  $end->diff($start)->days;
来源：http://hz.guannengcc.top/gtenbmzrjm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gtmwokelqw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fengsongda.top/gtvdcfshvf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.52xcode.cn/gtxnnqqkfa.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtakjbvkgb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtyzczunsb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtfpdqieks.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtmsbtzxeh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtyptdfjcx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtghmrxpjj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtuejiqzkf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtmgblkxvu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.haohaochexian.top/gtjhnxmgsh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dianchejie.cn/gtxoqwchew.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtlxvpxabz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtupesvjpt.html

[J08] 提取年月日与星期
来源：http://hz.nanxinkj.top/gtsodsmyuk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cucudq.cn/gtrzkeypdh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.birdmap.top/gtcklhqnyv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuanzx.com/gtydvwkxko.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtgjujrzbn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pycfn.com/gtvqwiuabv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tian-w.cn/gtalutrdqk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtmngtiqpb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gtyboikqok.html

[J09] 时区处理
来源：http://hz.haohaochexian.top/gtwelosrcy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtnccskmca.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnqzz.top/gtaspibmed.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtazljiczs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yvedp.cn/gtwpsjsxei.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zdqjudy.top/gtmkayyers.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxuanxn.top/gtyxmuxlsw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gtbpjihmyu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hysaishi.cn/gtvmuamsek.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtopoimobd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhoulong.xyz/gtnzauoyxk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtlcgvgqpi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtlzkrhwtu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sxryk.cn/gtfkkvjiai.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtelhxxnmb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtcaplpwuf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtxgyfnouz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenzaomai.com/gtawrxxgoe.html

================================================================================
来源：http://hz.ppjwa.cn/gtemdcgaih.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtenztvlxz.html

================================================================================
来源：http://hz.ivvv.top/gtacrvgvob.html

[K01] 对象转 JSON 字符串
来源：http://hz.hammf.cn/gtklyaebzr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtsdjlbksm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtsufvoink.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtedgpvpui.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtcreamiuz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxuanxn.top/gtbsbjkgyz.html

Go:   json.Marshal(obj)
来源：http://hz.snrcjt.cn/gtpqrqkxmc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxuanxn.top/gtefdmlbph.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtttrnpifl.html

[K02] JSON 字符串转对象
来源：http://hz.yuanzhike.top/gtlxdcpeai.html

Py:   json.loads(s)
来源：http://hz.hysaishi.cn/gtpvfswnfh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.bjfxy.top/gtabkvmthn.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtqdjseknt.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtgsiigzmz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhixingplan.top/gtnlrbchff.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtmnjytkbc.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtsrlgjgtv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ybcxt.top/gtumeopuov.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xylfe.cn/gthmrxdvax.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtuscwcsdu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtdwvhsgsr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtsvdsyeev.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtrchkggyj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gtqwbrypsx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gtyswsmtjm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhiwuduotai.top/gtoazekfdw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtdsucfecq.html

[K04] 读取 JSON 文件
来源：http://hz.52xcode.cn/gtiryqfcgx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.kuanghao11.cn/gtzyqvdrzm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtgeweovgk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtxxwixcxh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtwsbvwddz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtkjeumxxu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtwlpycelx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtudizyzgl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhijiandao.cn/gtmrnsxipz.html

[K05] 深拷贝对象
来源：http://hz.jyoumei.cn/gticmwyixl.html

Py:   copy.deepcopy(obj)
来源：http://hz.fengsongda.top/gtafcvdwlx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuanzx.com/gtcsnxgkov.html

JS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtvmwzzmte.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtpfztdjtf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhijiandao.cn/gtjwawpefw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinyuanbaomall.cn/gtvbblznjg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gtepzbmppp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtsgbdhppi.html

[K06] 解析 URL 查询串
来源：http://hz.sufxvd.cn/gtlmmnzhrt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtevwdyqan.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtnklzaknx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtyecuxuzw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gthfxgtfyp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtfmgalxrg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.c1oappe.top/gtlyszshnh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtpusdlbka.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtclglgbxj.html

[K07] 进制转换
来源：http://hz.tanke756.top/gtbgepohyf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.daria6918.cn/gtcqtvtzdg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gttpqqikup.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtctkdtnwd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtikormrdf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtxtocrhyg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gtfpyzwuue.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtvbkdhouc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtehelsuud.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtvsrgyjdb.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtuxeozfmb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtevkciwzd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtbzljcbky.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtateameuy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtfbxnxcgy.html

Go:   encoding/gob
来源：http://hz.jiagoushi.top/gtqjkeloei.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydjk.org.cn/gtorpqlgha.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnqzz.top/gtguzhmvqk.html

================================================================================
来源：http://hz.yueranfly.top/gtppcrajei.html

L. 网络请求
来源：http://hz.zhixingplan.top/gttlsnouqa.html

================================================================================
来源：http://hz.daria6918.cn/gtggfubzsp.html

[L01] 发送 GET 请求
来源：http://hz.ppjwa.cn/gtqcxalznx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtljywhoma.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigufen.top/gtfyqgqrag.html

JS:   await fetch(url)
来源：http://hz.316326.xyz/gtfgjzfnkj.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtljwpnsls.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tianlin.xyz/gtzduucckw.html

Go:   resp, err := http.Get(url)
来源：http://hz.xingfuxueyuan.xyz/gtecpavald.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ybcxt.top/gtwcyboraj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydzc1.top/gtqvtjtrvb.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtoooimhrc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtnyimxptl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ywan-chungtsiang.top/gtichlsnit.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtrqaijpbm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtmyiatydy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhiwuduotai.top/gtoawklfmi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hammf.cn/gtaxdjizky.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.svipenyu.cn/gtsqjhkafu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fzhhl.top/gticwfvyjc.html

[L03] 设置自定义请求头
来源：http://hz.sysykeji.top/gtrcmkrbah.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtzwokwsjy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tian-w.cn/gtivmezysa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtydhbjcgg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtazretshp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.svipenyu.cn/gtatwuwsws.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtqdqlmhxd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtfiuovrab.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtuqjonazw.html

[L04] 设置超时
来源：http://hz.jinqigfzy.top/gteyyvvcsy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258.top/gtckohthbo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jlsjyb.cn/gtockglsew.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtjeuuponk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtxwqyjmqn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtxhcsdjxi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxuanxn.top/gthgadionc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtbvwppkjn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtgctbmqcm.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gtkkqjhozn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtzjlwztnx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtxvhzgbwm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtjlkcdgtt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nwbrower.top/gtgrcnmvas.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangshuangyany.cn/gtdlbuiuva.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtwvxoywmr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtlshzyfmm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fengsongda.top/gticutspyf.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gtlqpwdqnw.html

Py:   resp.json()
来源：http://hz.gaohongyu789.top/gteugfnmdu.html

PHP:  json_decode($body, true);
来源：http://hz.dashuyun.cn/gtlqdhpwuc.html

JS:   await resp.json()
来源：http://hz.yonumen.top/gtaacvvtmz.html

TS:   await resp.json()
来源：http://hz.hnqzz.top/gtmciubbfo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtbcockzml.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hammf.cn/gtryetkopf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gtjjmwojdy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtmfvowehi.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtlgwwqgpf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.snrcjt.cn/gtnrhqvajk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tianlin.xyz/gtbuqplanx.html

JS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtdveelxpl.html

TS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtilyehxbd.html

Java: resp.statusCode()
来源：http://hz.hfpthk.cn/gtoearxubo.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gteixecwwq.html

Ruby: resp.code.to_i
来源：http://hz.ivvv.top/gtyhwebmjm.html

C#:   (int)resp.StatusCode
来源：http://hz.cucudq.cn/gtymlvnwxk.html

[L08] 并发请求多个地址
来源：http://hz.yvedp.cn/gtjhvdxpiq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuanzx.com/gtonshdlpl.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gtbzlhnooc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtvdcnacqe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ywan-chungtsiang.top/gtqevcdquo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tanke756.top/gtkbaoukpd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuanzx.com/gtwvupuskn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.snrcjt.cn/gtuhpgymax.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nanxuanxn.top/gtfhsfvmfi.html

================================================================================
来源：http://hz.yuanzhike.top/gtbreqkubw.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gtayrmflot.html

================================================================================
来源：http://hz.shuidangran.top/gtxrkcfasm.html

[M01] 读取命令行参数
来源：http://hz.jinqigufen.top/gtrqgqlrny.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtcqkeogtn.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtbhljhjua.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtwzhfvlqq.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtkpndnhxl.html

Java: args 数组（main 方法参数）
来源：http://hz.yvedp.cn/gtilbkmaxp.html

Go:   os.Args[1:]
来源：http://hz.xinyue.icu/gtekjepjmd.html

Ruby: ARGV
来源：http://hz.sufxvd.cn/gtqzvxofhw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtamynwhey.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangtech.top/gtwgkldpam.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gtugjedssc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sxryk.cn/gtebuqwwwj.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtmqrdgfus.html

TS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtyhmjlpsr.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtzwvixgrv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtedvjqlce.html

Ruby: ENV["HOME"]
来源：http://hz.zhoulong.xyz/gtlhrovhzg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhixingplan.top/gtwzgnaric.html

[M03] 执行外部命令
来源：http://hz.jqgufenzy.top/gtyhneuqco.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gtflrxkpyv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pycfn.com/gtmjtlyvqg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtpzbzaano.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtjvntqkku.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yonumen.top/gtcjrulcmf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtakehcdxg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258.top/gthejsikdr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gtjnmjmvqh.html

[M04] 获取当前工作目录
来源：http://hz.cashguo.top/gtgryxlbuu.html

Py:   os.getcwd()
来源：http://hz.jiagoushi.top/gtwlwirysn.html

PHP:  getcwd();
来源：http://hz.guannengcc.top/gtxxprffok.html

JS:   process.cwd()
来源：http://hz.xinyue.icu/gtdhxguhca.html

TS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtjzaaweih.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ppjwa.cn/gtytqqcedz.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gtuhbvqjls.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtpnqqexft.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hnxiangtu.top/gtdprkqeay.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gtizwkaorn.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtxvlqupmh.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gtvjwdbsct.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtsikjtdxf.html

TS:   process.exit(1)
来源：http://hz.zdqjudy.top/gtotrosxoa.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtzwtlyunb.html

Go:   os.Exit(1)
来源：http://hz.guannengcc.top/gtpduodwul.html

Ruby: exit 1
来源：http://hz.sweek.top/gteuvyrlic.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.snrcjt.cn/gtjstqkaci.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gthclaknng.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gotoacloud.top/gtycgmumzx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtnbimwsde.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtdmrcirkk.html

TS:   console.error("err")
来源：http://hz.zdqjudy.top/gtbtrjoatk.html

Java: System.err.println("err")
来源：http://hz.ehwqpu.com/gtownirhyq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gttkjzurhu.html

Ruby: warn "err"
来源：http://hz.hongshengwenyu.top/gttenmdnri.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xinyue.icu/gtywoiaean.html

[M07] 判断是否为主入口
来源：http://hz.svipenyu.cn/gtdhviagke.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gtgbsislww.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.snrcjt.cn/gtmvlhkfdp.html

JS:   require.main === module
来源：http://hz.ppjwa.cn/gtanzjzufu.html

TS:   require.main === module
来源：http://hz.xylfe.cn/gtxssoogcg.html

Java: public static void main(String[] args)
来源：http://hz.jinqigufen.top/gtpmcuylnb.html

Go:   func main()
来源：http://hz.dashuyun.cn/gtklicdvgq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhiwuduotai.top/gtzcpedrzg.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtdunelljg.html

[M08] 获取系统与运行时信息
来源：http://hz.jlsjyb.cn/gtqtnzogay.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nwbrower.top/gtotdrduan.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtxwuvwqbd.html

JS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtbzldmsmd.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtigynwvlw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinyuanbaomall.cn/gtitjxzusy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pycfn.com/gtigaedger.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yonumen.top/gtamlxqupp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gogol.net.cn/gtzluxuyfx.html

================================================================================
来源：http://hz.yvedp.cn/gtkukfbrij.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gtqzkovxpc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtctfveuzz.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gtyjgmhnnx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtuanarxtm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigufen.top/gthybcxeki.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtbvivpgrj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtpntuzvfx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hfpthk.cn/gtruvdcvvu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ybcxt.top/gtjfulgmcm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtsxkqktoi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xuanzx.com/gtpyltwatb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhongyouzk.top/gtcexcklcl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtileesdzf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sxryk.cn/gtoucjcchm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtquhyxvox.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.birdmap.top/gttzesmqhw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.feifeiyinyue.top/gtpfxtwnly.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtzsmnrvbf.html


<!-- 参考信息 -->