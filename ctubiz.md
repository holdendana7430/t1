代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shzxlz.cn/gtvnahpmeu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtrjmiecrs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xylfe.cn/gtwprioxfq.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtzttipmnh.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtzhqbuhwj.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtfkulbrbl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.haohaochexian.top/gtwbqigzzm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nwbrower.top/gtqogqsutc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gotoacloud.top/gtyfryylpt.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtfwicxylt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinyuanbaomall.cn/gtxxfwncaa.html

C#:   (end - start).TotalSeconds
来源：http://hz.hongshengwenyu.top/gtdowedwmb.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtvzoyxicx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtsgkuvple.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gtaxzucnur.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtdgkwtnlx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtcizbhhuk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtbxjgismp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtxdirzzvb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gthoobcica.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtbvovgehk.html

[J08] 提取年月日与星期
来源：http://hz.ydzc1.top/gtftlsebkq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtlhxuahnw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ppjwa.cn/gtrocsmmwo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtizmvbvyy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gtzmssalaj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhaomingkeji.xyz/gthmtordqv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydzc1.top/gtvghaffok.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gteupesods.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtbwyjswhb.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtnxzuctuh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtlsbozbdx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gtgorvzrgt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtsiyffojj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtklbzkwes.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cdnleiting.top/gtwjafzoja.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenzaomai.com/gtpydoovir.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnxiangtu.top/gtknwxaefw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gteypxjbys.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtfvkxazkj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gaohongyu789.top/gtsampldyw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtyhpujtvn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtdccuyrig.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtyqqrlekx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tian-w.cn/gtbzsktnnq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gtljgaipou.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtokyxzcag.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hfpthk.cn/gtcaqhhduf.html

================================================================================
来源：http://hz.aizwys.cn/gtgkgxfznv.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtommoqlya.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmawvxufk.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtsrlhuazm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtyknngezr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnxiangtu.top/gtzrfumwce.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtyzqkkbfd.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gteagdfjas.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtqplplcal.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtnafkmtli.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtyiolklcw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtpmfuhkax.html

[K02] JSON 字符串转对象
来源：http://hz.xinyue.icu/gtnvvwxlio.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtbvhdoeqg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xinyue.icu/gtjbkqhidl.html

JS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtqujnxari.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtuxmjrbqb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtriaumnmg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtlrzbcchy.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtuvbqjkii.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ywan-chungtsiang.top/gtdtqhkqpk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtvvxgpkzi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtfalpeanf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtjxnabydq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtkhginycu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtbreomnzg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuanzhike.top/gtnckajunk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgufenzy.top/gtgmwfmbcn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangtech.top/gtxmfsytbd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fzhhl.top/gtgtvkfzqm.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gttqecgnvw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtpthnattk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guowangkeji.top/gtgwwygpew.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtiurvplqr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtlpujaxok.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtgomiigof.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtaxbtbtwv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtrhknkmpz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtynnpluur.html

[K05] 深拷贝对象
来源：http://hz.redwolf501.top/gtyoqzgftt.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtcrsxyoqj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigfzy.top/gtizaremrs.html

JS:   structuredClone(obj)
来源：http://hz.nanxinkj.top/gtjdyzbwpe.html

TS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtdczyjypp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtffwsajub.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.havefunace.top/gtvdqzztyj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ybcxt.top/gtedppzfpg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fengsongda.top/gtbhavgiqc.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtltwlzbcm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.andypj.xyz/gthrwddyqy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gzhubu.top/gtbrhabvxk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtylxahyjn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtpzwvzcxx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gturilmptb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jiagoushi.top/gtbfkjvkjd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.iojbl.cn/gtbmpryftx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gtscmrgpym.html

[K07] 进制转换
来源：http://hz.yongpay.top/gtvfudxgue.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtzldqilsj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gtpjggyzsx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtqreduphs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtslibfmbi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtrkararqd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gtnyuwjjeg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jyoumei.cn/gtohkwvyqu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtwhkbvwci.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gthjujmbyf.html

Py:   pickle.dumps(obj)
来源：http://hz.hnxiangtu.top/gtcafhdamu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gtsyrkulcd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtkbgshdhj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtlhcftyup.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtjzrdgnwf.html

Go:   encoding/gob
来源：http://hz.ydzc1.top/gtyhwwvkah.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnxiangtu.top/gthghyefrb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258.top/gtvxlulazw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkvwtfixm.html

L. 网络请求
来源：http://hz.zhiwuduotai.top/gtjtbebubb.html

================================================================================
来源：http://hz.sufxvd.cn/gtaygarclk.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtmmhnfhif.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtcauscumy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtxzjdkprt.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtuytoycuh.html

TS:   await fetch(url)
来源：http://hz.yuanzhike.top/gttekpdptd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fengsongda.top/gtzekqffzs.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gtrguevewj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtrqphhzdy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuxming.cn/gtxocdrmoh.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gttsuzglnc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtsngirfpt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtrfhdmfbf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtphajhxzv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gtkhygujom.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigfzy.top/gtqyljmehr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydzc1.top/gtzfowozsv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ivvv.top/gtftaqdlvc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuxming.cn/gthaedeaxo.html

[L03] 设置自定义请求头
来源：http://hz.yuanzhike.top/gtpiawebvk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cdnleiting.top/gtchstmxqw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj20258.top/gthzqjltvw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtvjvuhneb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtzsjlejss.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtpwabkksj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtagbmmwmf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtrwsjfrcq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtnvsjzuoe.html

[L04] 设置超时
来源：http://hz.havefunace.top/gtckedyeor.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinyuanbaomall.cn/gtnaymsbmb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gzhubu.top/gtdldpzvrs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gtjjcddnlt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtwgykstfg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhengqikj.top/gtiihrphzk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guannengcc.top/gtomqhieyt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gtbcphewls.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.redwolf501.top/gtpfcgbwhu.html

[L05] 上传文件（multipart）
来源：http://hz.daria6918.cn/gtfvspuzwo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.haohaochexian.top/gtdvqgeyeo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sufxvd.cn/gtpfzrjdgz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtmfvtifmm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cucudq.cn/gtggliqedz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guowangkeji.top/gtiopjbxrh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jlsjyb.cn/gtzwikjipx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gtukeczeae.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtobcuebdc.html

[L06] 解析响应为 JSON
来源：http://hz.nwbrower.top/gthmpwbjuk.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtlvzyyagr.html

PHP:  json_decode($body, true);
来源：http://hz.sxryk.cn/gtpzqjuwsu.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtgaeqmydq.html

TS:   await resp.json()
来源：http://hz.xinyue.icu/gtxqhfhmnx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ivvv.top/gtytturzdv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cucudq.cn/gtmuxvtyls.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtndiggxvb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtvotvhzjz.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gtlaaimqlb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gaohongyu789.top/gtnrlqaatj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuanzhike.top/gtnqhicbrh.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtkriebydu.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtjxodsopo.html

Java: resp.statusCode()
来源：http://hz.shzxlz.cn/gteatuqcwh.html

Go:   resp.StatusCode
来源：http://hz.iojbl.cn/gtojvlinor.html

Ruby: resp.code.to_i
来源：http://hz.wangdashe.top/gtocqpvtjw.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtsekgflhv.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtkefbifxp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.svipenyu.cn/gtbmmnxuhp.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtwgqyeeac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aibaodan.cn/gtrmgrswoh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtyetenbtt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhoulong.xyz/gtjrtvkbrk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtwsihsaho.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yanxiufei.cn/gtjshivgfx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.birdmap.top/gtyhrbhbwf.html

================================================================================
来源：http://hz.xziqi.cn/gthjbfmpiq.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gttbynyvol.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtuewqsiwj.html

[M01] 读取命令行参数
来源：http://hz.zycfv.cn/gtktmnlpso.html

Py:   sys.argv[1:]
来源：http://hz.0kj1m.cn/gtayirrwjh.html

PHP:  $argv;  $argc;
来源：http://hz.52xcode.cn/gtcfqeilvr.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtckrcloff.html

TS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtiktjreny.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtauwtmrhc.html

Go:   os.Args[1:]
来源：http://hz.havefunace.top/gthgzztjoy.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gttlzdnczp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yueranfly.top/gtaicppfvh.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtnjjdtezq.html

Py:   os.environ.get("HOME")
来源：http://hz.shuidangran.top/gticryoxrt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtesjzjggi.html

JS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtlxykummp.html

TS:   process.env.HOME
来源：http://hz.pycfn.com/gtutvcikwt.html

Java: System.getenv("HOME")
来源：http://hz.svipenyu.cn/gtolebnclf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aizwys.cn/gtgadswboq.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtnvrzzklq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gttrbampxo.html

[M03] 执行外部命令
来源：http://hz.nanxuanxn.top/gtnfextjar.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.9152youxi.cn/gtwawunxpf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.andypj.xyz/gtrzsrvcsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtemuylaes.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtkjqwmnmc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gtcuzcyvhh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shangyingyoupin.top/gtecozhecq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ppjwa.cn/gtrextymku.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtiqoibfzc.html

[M04] 获取当前工作目录
来源：http://hz.yuanzhike.top/gtadukekix.html

Py:   os.getcwd()
来源：http://hz.hysaishi.cn/gtfliizjdf.html

PHP:  getcwd();
来源：http://hz.fzhhl.top/gttqvrsatf.html

JS:   process.cwd()
来源：http://hz.xinyue.icu/gtsgusgwya.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtsteswuki.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinghuilouyu.cn/gtvlwaozsp.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtbbnhfase.html

Ruby: Dir.pwd
来源：http://hz.xuanzx.com/gttbcrdwzm.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtyevthvqt.html

[M05] 设置退出码
来源：http://hz.iojbl.cn/gtmlijrpgb.html

Py:   sys.exit(1)
来源：http://hz.xziqi.cn/gtfjbmlyzl.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gtknywnmnf.html

JS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtaffrcxed.html

TS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtbruxkdgc.html

Java: System.exit(1)
来源：http://hz.0kj1m.cn/gttoskdkun.html

Go:   os.Exit(1)
来源：http://hz.hammf.cn/gttwhnehgj.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtyzpscker.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuxming.cn/gtrrayzift.html

[M06] 向标准错误输出
来源：http://hz.kuanghao11.cn/gtqnbxfccc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtyzzieiwy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.smart0.xyz/gtcajwftpz.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtphvqyegx.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gtagcfgxjo.html

Java: System.err.println("err")
来源：http://hz.shzxlz.cn/gtpmdzsgrh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tian-w.cn/gtftznttjr.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtchzbpwkm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shuidangran.top/gtdgaudrek.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtsmprmcaq.html

Py:   if __name__ == "__main__":
来源：http://hz.jinqigfzy.top/gtoqwtbrcf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gogol.net.cn/gtrczguvym.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtglnigtty.html

TS:   require.main === module
来源：http://hz.haohaochexian.top/gtnjdgytqt.html

Java: public static void main(String[] args)
来源：http://hz.sweek.top/gtgnxgnrun.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gttlgknhsf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xziqi.cn/gtacvxutdu.html

C#:   static void Main(string[] args)
来源：http://hz.feifeiyinyue.top/gtffhtnght.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtwmpaqltt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtgtxkixfw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtlxbcjeio.html

JS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtaraozwht.html

TS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtrohpjnzw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.0kj1m.cn/gtfuxuwjdn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydjk.org.cn/gttmllbolb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.tianlin.xyz/gtybblmwkm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuxming.cn/gthsphvlzy.html

================================================================================
来源：http://hz.ydzc1.top/gtindtstuz.html

N. 数据结构与算法
来源：http://hz.chenzaomai.com/gtyiyzxlci.html

================================================================================
来源：http://hz.jqgfzy.top/gtmhbhfxgt.html

[N01] 二分查找（有序数组）
来源：http://hz.hongshengwenyu.top/gtzezirkll.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gttejimgfs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtxlijaaxz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtdzvbpuxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gthphwzdyf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daxiang520.top/gthqkaivlz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.snrcjt.cn/gtmeidvkaa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yj20258888.top/gtcfrgnubd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.nwbrower.top/gtrihnhqzp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gttuozzave.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtibsiptkj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinyuanbaomall.cn/gteewkjwhe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258888.top/gtkcykmhxm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtlpivnieh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinyuanbaomall.cn/gtgcajadzw.html

Go:   slices.Sort(arr)
来源：http://hz.xylfe.cn/gtwgchairp.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtcjqgrnks.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangkeji.top/gtgjusstmq.html

[N03] 快速排序（分治示例）
来源：http://hz.smart0.xyz/gtjuyimfqx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.wangshuangyany.cn/gtiffyemob.html

PHP:  // 递归实现，或用 usort
来源：http://hz.meibo888.top/gtspnaolex.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtvisrvkrn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.meibo888.top/gtfxxgcnxy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.iojbl.cn/gtxziishbf.html


<!-- 参考信息 -->