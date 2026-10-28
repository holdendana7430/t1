代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gogol.net.cn/gtguvwcoqf.html

Go:   end.Sub(start).Hours()
来源：http://hz.vqdsnc.cn/gtrbqriiqc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtbnqkhjej.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtkfmyoumm.html

[J07] 比较两个日期
来源：http://hz.cheryme.top/gtcjsecbll.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtuqtqdabs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gtywfcgywf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtkbludcgx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtanhskqok.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gtxsvaycoc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gtigqjzens.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gttozxxqar.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtpipsyhji.html

[J08] 提取年月日与星期
来源：http://hz.wangshuangyany.cn/gtdgssairq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtzxbcvkbv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtusgajjbp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuanzx.com/gttyzwkloa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtdagyjkno.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gtxfftmqch.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtgwtkmmbh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gthxblbhbv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtkaklgjcg.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtxorzodro.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtnopfkflv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gtvsbbnkju.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtpfrtynjr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtthcbdwpc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtvnyiktzz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtwaamfmxl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydjk.org.cn/gtwcgcjazb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gtgmpqvkhj.html

[J10] 取今天 / 本月第一天
来源：http://hz.sufxvd.cn/gtiqhpkccb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtmltbpiqy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtibpenxrx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtjhfoynyj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cqqwz.cn/gtctmaoflb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guowangkeji.top/gtxanoutgy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtrfxjyykh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.9152youxi.cn/gtczcinjxy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuetiantiany.cn/gtvbzzdhmp.html

================================================================================
来源：http://hz.andypj.xyz/gtmpznashf.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtzzywgkwg.html

================================================================================
来源：http://hz.svipenyu.cn/gtpmkxwbkl.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangkeji.top/gtgddqvuww.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gteftyafqv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtstsoiavx.html

JS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtocyxkywf.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtduqutcvd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtyymddoms.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gtvvyfswqf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gtanyrxbze.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtpbuawqgb.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtbmyljzyp.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtqnzlwrvz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtprnygobz.html

JS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtpiyayusc.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gthoszihwq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hysaishi.cn/gtudaojhpl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtygimwqfs.html

Ruby: JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtblqejssd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yongpay.top/gtppthqdts.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtoamdgqfc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtbelhuoxh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtepoeyvpc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gthghmbnvv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtnvoryipz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.c1oappe.top/gtkvrthygf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtmtqppcmx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtwerqgnae.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zycfv.cn/gtbochegsq.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtqnqcylhz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtbzltzmge.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtwjsrhrlw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtviurwwun.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtppwgbxqv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtqhgojgio.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtcolxglad.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.redwolf501.top/gtbkubdiws.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtlelkpbik.html

[K05] 深拷贝对象
来源：http://hz.yj20258888.top/gtzbjpekvu.html

Py:   copy.deepcopy(obj)
来源：http://hz.dashuyun.cn/gtysssbhgp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhixingplan.top/gtyqutphhn.html

JS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtzfpwbphb.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtjksjgnxo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yongpay.top/gtkmtkeejf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenzaomai.com/gtlsvwvsyi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuanzhike.top/gtydnvrgwy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.meibo888.top/gtqcqwdxlt.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtffdlympe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtfsnheugk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtwzkdtztf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtgbyslhoa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtvquwhhuv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtuctmvyss.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yvedp.cn/gtgaruoyjs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtuefvifaw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtayrwldxh.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtxjzmsmtb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtdmymsakq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtzajirsml.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtsgwuxhdf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtqcezswxa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtzsumkfid.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtdqjarddn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cdnleiting.top/gtqnzyzlrk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtczslgnaa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hammf.cn/gtsfxudzma.html

Py:   pickle.dumps(obj)
来源：http://hz.shangyingyoupin.top/gtrmlwjbzg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtmsybkcgk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtvhhwoodx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtoelrejoc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gttkyehpqe.html

Go:   encoding/gob
来源：http://hz.jqgfzy.top/gtmnigsxgq.html

Ruby: Marshal.dump(obj)
来源：http://hz.xziqi.cn/gtfafjbqxp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtunciewjx.html

================================================================================
来源：http://hz.xylfe.cn/gtpmmfdehp.html

L. 网络请求
来源：http://hz.shangyingyoupin.top/gttziiestn.html

================================================================================
来源：http://hz.cashguo.top/gtztxwlrbq.html

[L01] 发送 GET 请求
来源：http://hz.xinyue.icu/gtpfjdjpyi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuetiantiany.cn/gtpndmclxq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zdqjudy.top/gtyjzrfagf.html

JS:   await fetch(url)
来源：http://hz.fengsongda.top/gtiojpguva.html

TS:   await fetch(url)
来源：http://hz.daxiang520.top/gtqzoassll.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nwbrower.top/gtymjcljfx.html

Go:   resp, err := http.Get(url)
来源：http://hz.shzxlz.cn/gtsydyrfnb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hammf.cn/gtdvsxrose.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtutzoaqrw.html

[L02] 发送 POST JSON
来源：http://hz.cucudq.cn/gtshpuyhgd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtbgvnmwhw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yueranfly.top/gtrhpqbsfq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtwlvmjvke.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtvslcqhoa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtafbqcmnu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtantrkjbe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.feifeiyinyue.top/gtgzscfbpr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtqrncwvpo.html

[L03] 设置自定义请求头
来源：http://hz.zhiwuduotai.top/gttcugbaxn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtiydjwlvn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gzhubu.top/gtjiqcpgri.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtzpvhpzgk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtydfjuzjs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj202588.top/gtaosxnrea.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtotmhicxd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gogol.net.cn/gtfojbjekd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtgnfsrknp.html

[L04] 设置超时
来源：http://hz.pengpengdd.cyou/gthwtdjjwu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtypucshjn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhongyouzk.top/gthqhlvgrz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtqqpbxamb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gthfnkpdou.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gteoznfubq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gtdzuolhnv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtqzaklmgk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yvedp.cn/gtrwbrllmq.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangtech.top/gtcftclise.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cheryme.top/gtaslrdyrl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtpznrknzh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.feifeiyinyue.top/gtshlakdaf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtdijklque.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtquorsumx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtftabliop.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gtnggyncrl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sufxvd.cn/gtfrxlgazz.html

[L06] 解析响应为 JSON
来源：http://hz.mhx1999.top/gtrckqvamd.html

Py:   resp.json()
来源：http://hz.jinqigfzy.top/gtmvjbvihr.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtzibjjpgf.html

JS:   await resp.json()
来源：http://hz.sxryk.cn/gtrgvskfdw.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtckxsquug.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jlsjyb.cn/gtlyysceaz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gotoacloud.top/gtmpiczzsh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtfovnqnjd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtypjyqbis.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtsmghiynn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gthesdrnhr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtjbwxnbti.html

JS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtcgcalevb.html

TS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtbiqcmfyj.html

Java: resp.statusCode()
来源：http://hz.chenzaomai.com/gtvnghpkls.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtdyptmugi.html

Ruby: resp.code.to_i
来源：http://hz.cdnleiting.top/gtphqmrckd.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gtrqiglzrt.html

[L08] 并发请求多个地址
来源：http://hz.hnxiangtu.top/gtgnzexeue.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtvokywptw.html

PHP:  curl_multi_init() 系列
来源：http://hz.shzxlz.cn/gtoztkdfjw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtudonekkk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtxmfjpxkt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.iojbl.cn/gtdatyolwq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xuanzx.com/gtagshzmcp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hnqzz.top/gtpscadhfv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aizwys.cn/gtckbhixku.html

================================================================================
来源：http://hz.sweek.top/gtqjsmxohl.html

M. 命令行 / 进程 / 环境
来源：http://hz.ehwqpu.com/gtjapgnkta.html

================================================================================
来源：http://hz.jianghu66.top/gthtidqpna.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gtqtstbqsi.html

Py:   sys.argv[1:]
来源：http://hz.yuanzhike.top/gtbkikjszj.html

PHP:  $argv;  $argc;
来源：http://hz.zhoulong.xyz/gtzmzvedhs.html

JS:   process.argv.slice(2)
来源：http://hz.xuanzx.com/gtwxzbmnbr.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtuduznsfu.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gthlctukoz.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtxfguykhc.html

Ruby: ARGV
来源：http://hz.pycfn.com/gttzyvmorn.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtgsrppsch.html

[M02] 读取环境变量
来源：http://hz.guowangkeji.top/gtteqjpkpz.html

Py:   os.environ.get("HOME")
来源：http://hz.shzxlz.cn/gtogjqeysw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtxhcvrdsx.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtczgdgphv.html

TS:   process.env.HOME
来源：http://hz.hnqzz.top/gtcslvzbiw.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gtirzwhaxe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gtrpmdrshp.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gtihoyuiyc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zycfv.cn/gtbgcbtxlp.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtkenwogwl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.iojbl.cn/gtcnahkkbq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtxswvwmjr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cucudq.cn/gtfqweyhbh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtjtkgqgap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hywenlv.cn/gtexqwzpwe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.svipenyu.cn/gtvatlcsqd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tianlin.xyz/gtawhwccrq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtpwcatcrn.html

[M04] 获取当前工作目录
来源：http://hz.pengpengdd.cyou/gtbdyjwokv.html

Py:   os.getcwd()
来源：http://hz.shuidangran.top/gtcurzhxjw.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtfmnwwoun.html

JS:   process.cwd()
来源：http://hz.dianchejie.cn/gtdgkwrmmt.html

TS:   process.cwd()
来源：http://hz.jqgfzy.top/gtphhvqggn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gtektnbbvn.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtpmddemho.html

Ruby: Dir.pwd
来源：http://hz.chenlongwang.top/gtynjkefec.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.haohaochexian.top/gtnwhwdgbc.html

[M05] 设置退出码
来源：http://hz.quarkkingdee.top/gtqitujelf.html

Py:   sys.exit(1)
来源：http://hz.wangdashe.top/gtjqnwoafi.html

PHP:  exit(1);
来源：http://hz.jinghuilouyu.cn/gtkmjgjifg.html

JS:   process.exit(1)
来源：http://hz.birdmap.top/gtrmklkotm.html

TS:   process.exit(1)
来源：http://hz.nanxuanxn.top/gthboulacw.html

Java: System.exit(1)
来源：http://hz.jinqigfzy.top/gtxrbxsvoy.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gtigwojzmo.html

Ruby: exit 1
来源：http://hz.aizwys.cn/gtkzcqxwyj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtglukvdyf.html

[M06] 向标准错误输出
来源：http://hz.meibo888.top/gtstjxczbm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtijoyxqnf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xuanzx.com/gtghjepntu.html

JS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtullwduyi.html

TS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtjrnhnkvo.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtcgzrynaz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gtyytvmsxt.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtcbbnkuzg.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtucecfznw.html

[M07] 判断是否为主入口
来源：http://hz.zhengqikj.top/gtvxnhnrbo.html

Py:   if __name__ == "__main__":
来源：http://hz.quarkkingdee.top/gtfluzllfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtydkzrked.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gtvfujdbwi.html

TS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtxxplbqot.html

Java: public static void main(String[] args)
来源：http://hz.guowangkeji.top/gtjordihpn.html

Go:   func main()
来源：http://hz.dashuyun.cn/gttydjxweu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guowangkeji.top/gtojxgsdvb.html

C#:   static void Main(string[] args)
来源：http://hz.hnqzz.top/gtnlygqsbs.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtitynktql.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtfpmnhyfh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ywan-chungtsiang.top/gtgrbmwpqa.html

JS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtfgiysbjg.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtaqtugvcq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnxiangtu.top/gtbabdhume.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.haohaochexian.top/gtyzmqwgro.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.guowangkeji.top/gtwmlnovts.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.316326.xyz/gtkbcyjjox.html

================================================================================
来源：http://hz.0kj1m.cn/gtuqgtuyww.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtsxrasicl.html

================================================================================
来源：http://hz.wangdashe.top/gtxjwrsuaf.html

[N01] 二分查找（有序数组）
来源：http://hz.chenlongwang.top/gthhshmmyg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yanxiufei.cn/gtiqgqywki.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guowangkeji.top/gtzxousngz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtqxjmugkx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daxiang520.top/gtoonlrfxm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ybcxt.top/gtdciijzoy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtqxohzjrk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtpmnvmiov.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtqfokzice.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jiagoushi.top/gttffvilvg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhiwuduotai.top/gtesgvbtjq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtnkvwabjt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtowynitnm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtqiicgpiv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fzhhl.top/gthzgfolio.html

Go:   slices.Sort(arr)
来源：http://hz.yueranfly.top/gttvcxhskq.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtgbidyuzf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.snrcjt.cn/gtifmliwet.html

[N03] 快速排序（分治示例）
来源：http://hz.cqqwz.cn/gtxsvcgfkc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinghuilouyu.cn/gtctsqdqbn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtwaantafb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtarnhfuib.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtqpakxgps.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ppjwa.cn/gtyjxzhkaa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ybcxt.top/gtnerdggqr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tanke756.top/gturihclfu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nanxuanxn.top/gtgqefvzyz.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtufadrewq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtvqdqngny.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtppfxybge.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxuanxn.top/gtffpruufy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtrssknmbk.html


<!-- 参考信息 -->