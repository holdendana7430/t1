代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.mhx1999.top/gtapnzphub.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtpbrgdlrb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gtowikldvq.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtgfvgdizc.html

Py:   (end - start).total_seconds()
来源：http://hz.sxryk.cn/gtwiltriae.html

PHP:  $end->diff($start)->days;
来源：http://hz.sufxvd.cn/gtcnhqsmpg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtpevfurpy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gtiuwvqipr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtihhrqsvt.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtdyrqhnvg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gtdfobtqiy.html

C#:   (end - start).TotalSeconds
来源：http://hz.yueranfly.top/gtpejkvlxn.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtfscvaryo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtnslqdpbe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtiuedxkpv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.redwolf501.top/gtihbvbhzm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtnlfceqhs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtdxxrgxyb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtwzdyicam.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtpukddqln.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtpdlxydfp.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gtiazsziyj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.9152youxi.cn/gtossruktw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tian-w.cn/gtvinmozpt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtjrzzkytw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cqqwz.cn/gtptsqnszo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhaomingkeji.xyz/gtkgolrzwl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtnpewenrs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtgdhabmei.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtrgfeufdw.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtthnjyejf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daxiang520.top/gtcodgyfnv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuanzx.com/gtqnobnvrn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtwnudbckz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gotoacloud.top/gtwssruyns.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.9152youxi.cn/gtoiewwmry.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sxryk.cn/gtoslddofn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.52xcode.cn/gteegwvkwm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtodfmtvnj.html

[J10] 取今天 / 本月第一天
来源：http://hz.cashguo.top/gtxkssrfjd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtjxnbrqyc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gzhubu.top/gtvdeeqjkq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.birdmap.top/gtmevbkvfs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gthziwuwmb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtaceaxzrs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.mhx1999.top/gtajdvteow.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ehwqpu.com/gteypwwwlf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gttxratoho.html

================================================================================
来源：http://hz.redwolf501.top/gtzljkhknv.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtddndrvyg.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtgzmbyhvk.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gtpvmechar.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtdralllph.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtnosqxkkn.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtpzbuhvhz.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtotyaxqca.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.52xcode.cn/gtjnakpkub.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtxsnndptu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hysaishi.cn/gtbwccuwzr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtlpkamzbl.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtylhztsrh.html

Py:   json.loads(s)
来源：http://hz.sweek.top/gtvnxrhfzp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtzjhsgygl.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtfmwokbgq.html

TS:   JSON.parse(s)
来源：http://hz.sweek.top/gturdfzdko.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yuxming.cn/gtjhftmtek.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtyygssyfs.html

Ruby: JSON.parse(s)
来源：http://hz.cheryme.top/gtpozzjvtq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtyrfwmeeg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daria6918.cn/gtjddipard.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtrpdecjbx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtcyivskiu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtpkzceulz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtjxgqymhn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cheryme.top/gtgabiwhct.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtsvnvpyrf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhaomingkeji.xyz/gtfmxzattp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhijiandao.cn/gtwoxlsqmx.html

[K04] 读取 JSON 文件
来源：http://hz.zycfv.cn/gturoekhun.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhijiandao.cn/gtggcqbjyt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtvnaeckue.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtdtpaujpb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtknjifuca.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtdxpncwzv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gttxdzihma.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangtech.top/gtarjtdnru.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xziqi.cn/gtyphlidfs.html

[K05] 深拷贝对象
来源：http://hz.hywenlv.cn/gtysotekao.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtnlyfasib.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtfxqomqig.html

JS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gtoydmrvvl.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtmjhuamav.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gttpneedlc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtniqwxees.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtdaytjjao.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gthygcflob.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtiuindinx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gtrdvfhunr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.haohaochexian.top/gtpnpteuyz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtzqmiemlb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gthmyglwzx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.0kj1m.cn/gtttgesuxh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtunavxhvw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yvedp.cn/gtlatqnzbx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhixingplan.top/gtzxtbtzxa.html

[K07] 进制转换
来源：http://hz.zhaomingkeji.xyz/gtjprzdvcl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigufen.top/gtshkwpcxp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangdashe.top/gttdeztgpf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtpqrkfvtj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtsgblldct.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtgeoweitu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenjidiqi.icu/gtazpesivn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenlongwang.top/gtvzqreioc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sufxvd.cn/gtupmgbnts.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtkuycuxfe.html

Py:   pickle.dumps(obj)
来源：http://hz.jiagoushi.top/gtwscjtwoi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sweek.top/gtjtixfzmm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtbyjfmyix.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtuaxmbxvs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.meibo888.top/gtywobpmym.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gttvcjajkd.html

Ruby: Marshal.dump(obj)
来源：http://hz.sxryk.cn/gtkwwwugfl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ppjwa.cn/gtankmfhnk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmryqedas.html

L. 网络请求
来源：http://hz.guannengcc.top/gtplzqloig.html

================================================================================
来源：http://hz.jlsjyb.cn/gtoxdjhqqv.html

[L01] 发送 GET 请求
来源：http://hz.nwbrower.top/gthrcsklqs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtcnulfwjt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtbywwutzo.html

JS:   await fetch(url)
来源：http://hz.yonumen.top/gtotammwsk.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtdevksfck.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangdashe.top/gtawtonwuw.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtozqdavol.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.feifeiyinyue.top/gtfvckhvdn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yvedp.cn/gtxjyawddp.html

[L02] 发送 POST JSON
来源：http://hz.xinyue.icu/gtnodrewln.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cdnleiting.top/gtfaatzmxp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nwbrower.top/gtysudsdvs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtnemngnct.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtjdaiavkq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yvedp.cn/gtzcqtslvb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.havefunace.top/gtdfwxczge.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtewlnkxmi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtedgbtpqy.html

[L03] 设置自定义请求头
来源：http://hz.birdmap.top/gtdkjmjeep.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shangyingyoupin.top/gtvxdjnpli.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xingfuxueyuan.xyz/gtieqpojhd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtqllaspil.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtacyfzidk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hfpthk.cn/gtdnbldimv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xinyue.icu/gttnasmzcq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.shanyushiyangtech.top/gtguexbvga.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinyuanbaomall.cn/gtgthgctnl.html

[L04] 设置超时
来源：http://hz.fzhhl.top/gtyabprbkg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daxiang520.top/gtwkjaxqzj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gtdomspfyr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtpgimyqow.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtybalnfkc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gtqtpesrld.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuanzx.com/gttxpbripk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtoilkwyos.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtrasrxeuk.html

[L05] 上传文件（multipart）
来源：http://hz.sufxvd.cn/gtweyzykdp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtowpqqxwx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sweek.top/gtilkllsvc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtpkfcmlne.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ivvv.top/gtkzexxqou.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtiskjtgiw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tianlin.xyz/gtzbzsqakl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zycfv.cn/gtlyhjukhu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yuanzhike.top/gtmyrmazau.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258888.top/gttihgsenv.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtulqqbifg.html

PHP:  json_decode($body, true);
来源：http://hz.jinghuilouyu.cn/gtigjhikri.html

JS:   await resp.json()
来源：http://hz.0kj1m.cn/gtxhktmwwm.html

TS:   await resp.json()
来源：http://hz.cheryme.top/gthxmvwcsa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtrjlnfike.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.0kj1m.cn/gthllzaiec.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtioakxilz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yanxiufei.cn/gtrgbrrncf.html

[L07] 处理 HTTP 状态码
来源：http://hz.zycfv.cn/gtrnzwnpvg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dianchejie.cn/gtfyjpusnr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daria6918.cn/gtfbiwfovs.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtewlrccvr.html

TS:   resp.ok;  resp.status
来源：http://hz.tanke756.top/gtfdmdqprl.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtektfymiv.html

Go:   resp.StatusCode
来源：http://hz.vqdsnc.cn/gtmdirgzpc.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtuabedvny.html

C#:   (int)resp.StatusCode
来源：http://hz.52xcode.cn/gtsfoewsjx.html

[L08] 并发请求多个地址
来源：http://hz.sweek.top/gtxhaikotm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xingfuxueyuan.xyz/gtbkyuzwpm.html

PHP:  curl_multi_init() 系列
来源：http://hz.feifeiyinyue.top/gthyhnsgsj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtoiqlaixy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtoxlxjkoo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtodnzgbgx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jinqigufen.top/gtwaybpjcn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.daxiang520.top/gtdsrnhyhn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.mhx1999.top/gtrzqjkwmt.html

================================================================================
来源：http://hz.vqdsnc.cn/gtfwfagzrp.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtufkfbujk.html

================================================================================
来源：http://hz.aizwys.cn/gtoifzzfgg.html

[M01] 读取命令行参数
来源：http://hz.cheryme.top/gtgesletkw.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gttarfmdcm.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtizstdkja.html

JS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtahzcemlm.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtirfvnvdi.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgufenzy.top/gtdcifwpmf.html

Go:   os.Args[1:]
来源：http://hz.jinqigfzy.top/gtzdopldfh.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtkjwlmgsx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gzhubu.top/gtcrhcccaq.html

[M02] 读取环境变量
来源：http://hz.xylfe.cn/gtubyetbpj.html

Py:   os.environ.get("HOME")
来源：http://hz.zycfv.cn/gtijtjirvw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gtfwfmwxsr.html

JS:   process.env.HOME
来源：http://hz.yvedp.cn/gtqyymnohi.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtxndismqs.html

Java: System.getenv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtzqcbvuqs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenlongwang.top/gtcvzpezpq.html

Ruby: ENV["HOME"]
来源：http://hz.316326.xyz/gtiylesfqz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinghuilouyu.cn/gttyhphylo.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtoskdhzjv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.havefunace.top/gtaebeqacc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zycfv.cn/gtnrqwkjpn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtrrptluvl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtonyhkrhu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtqhyckxjr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cashguo.top/gtomjnpdmf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtmsrxiica.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtlzmyyxvl.html

[M04] 获取当前工作目录
来源：http://hz.vqdsnc.cn/gtxmhesmzd.html

Py:   os.getcwd()
来源：http://hz.redwolf501.top/gtmkitdfca.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gtgqbzgltt.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtmpidxnmc.html

TS:   process.cwd()
来源：http://hz.zhixingplan.top/gtosiksamt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pengpengdd.cyou/gtqbzfiqpq.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtwlqtoeib.html

Ruby: Dir.pwd
来源：http://hz.cucudq.cn/gtrzghegbe.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shangyingyoupin.top/gtqoqohkjx.html

[M05] 设置退出码
来源：http://hz.ybcxt.top/gtktscjppd.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gthxemxzkx.html

PHP:  exit(1);
来源：http://hz.tian-w.cn/gtiiqsldix.html

JS:   process.exit(1)
来源：http://hz.quarkkingdee.top/gtxzdwmuiy.html

TS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gttolqcvtq.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gtrmpevohi.html

Go:   os.Exit(1)
来源：http://hz.guowangkeji.top/gtbwameqrr.html

Ruby: exit 1
来源：http://hz.yj202588.top/gthchqrlpa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtvyfmlcmt.html

[M06] 向标准错误输出
来源：http://hz.jinqigufen.top/gtyxcghdji.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtkhwugbrm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.svipenyu.cn/gtpwhxouoj.html

JS:   console.error("err")
来源：http://hz.havefunace.top/gtlnjaawhh.html

TS:   console.error("err")
来源：http://hz.xylfe.cn/gtalqmdwet.html

Java: System.err.println("err")
来源：http://hz.nanxinkj.top/gtkcfslbok.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.9152youxi.cn/gtokthcvwl.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtzqufonhp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtcuusocho.html

[M07] 判断是否为主入口
来源：http://hz.xuanzx.com/gtavqhcyda.html

Py:   if __name__ == "__main__":
来源：http://hz.ywan-chungtsiang.top/gtuahpqdgp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.quarkkingdee.top/gtzebdkujh.html

JS:   require.main === module
来源：http://hz.guowangkeji.top/gtjysmpzwd.html

TS:   require.main === module
来源：http://hz.bjfxy.top/gtcwphtdwf.html

Java: public static void main(String[] args)
来源：http://hz.cashguo.top/gttecqldhh.html

Go:   func main()
来源：http://hz.cashguo.top/gtzgyyoggd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.meibo888.top/gtdzruxepm.html

C#:   static void Main(string[] args)
来源：http://hz.52xcode.cn/gtulqxepjq.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gtmixmzzrb.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtwsnowhca.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gthhjoqukr.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtufnctvwm.html

TS:   process.platform;  process.version
来源：http://hz.kuanghao11.cn/gtseeuvxgd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtlomqufov.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nanxuanxn.top/gtuhnrhrtz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.pycfn.com/gtujyclyta.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hfpthk.cn/gtmqtsqluw.html

================================================================================
来源：http://hz.cucudq.cn/gtcvqeiwbu.html

N. 数据结构与算法
来源：http://hz.zycfv.cn/gtdtuwebcw.html

================================================================================
来源：http://hz.meibo888.top/gteflmotsv.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtucayiyrd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yonumen.top/gtqyctynlq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cucudq.cn/gtuhskpavd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtlvpgiiso.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhoulong.xyz/gtztsgpfwv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtmjomievj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuanzhike.top/gtxwcevsgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fengsongda.top/gtpfqljzbj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gogol.net.cn/gtxenajddm.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xylfe.cn/gtkeirbsiy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.svipenyu.cn/gtlbuqerio.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenzaomai.com/gtzydvecga.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuanzx.com/gtreqycavn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtvrpbkvpw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zdqjudy.top/gtiwgeqihe.html

Go:   slices.Sort(arr)
来源：http://hz.birdmap.top/gtskuuivmq.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtdfhnesab.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xziqi.cn/gtuyyrvurt.html

[N03] 快速排序（分治示例）
来源：http://hz.quarkkingdee.top/gtifiojzqf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xylfe.cn/gtwmfuthwt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gotoacloud.top/gtsecvjlfk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.fengsongda.top/gtzlhfqlju.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aibaodan.cn/gtxyymuulx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dianchejie.cn/gtdzcxhdox.html


<!-- 参考信息 -->