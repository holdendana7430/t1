代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2jzmyrqdr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2uxfdhuqj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwasnuxt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yfudnebq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2khbfgofv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2hmgcmvnl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2vfdclcsl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2tqcjmhzl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2dsnlthgd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2gjozjopx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mpnweogw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2nalflecf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2tqgpgfgi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hptkxymt.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2hrgvqwva.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cmcnvcac.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2xvmziaap.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jctjtalu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2frqjjgfd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2graiesbk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kvsbbnxm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2dqffgfer.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ukneugwh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2lbdmrwrp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fqwtcoej.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2vnzmbxcc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2opzuagqp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2syvmvofq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2fykehjjf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2utnqcqcq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2rrjduuir.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qmpgkkje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwfysfcd.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2znzsesti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wszeabid.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pycjvaim.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rilguaks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uaeqawoo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcoecdwq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cvesjwkf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2rkztjhod.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yugtalti.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2yfzrbgqu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzlvyhdc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qlgtrfri.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2heklmuyt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2khpwxfgj.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umssxvkn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eykfytyb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ccwcebwk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2plgxqltj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kmuhpeli.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzthvvg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2vllwwwgr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qzfqnlzr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dawdmewo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lezsould.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vfeegtbb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xxqdhncs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wmjltwpq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vcvunlzd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2rhhhjggn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2sdxaryra.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2igikuupc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2tvsmfgre.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nwzgrbsm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2faexlxtm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ydosdbxr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rjswnaam.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wsmegdgk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ttoccetv.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2fqddyqia.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2bdfmrvnl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fskdkrou.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2upohglgt.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnihkuma.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2duhouswj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2loizkwrn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vlnrijew.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2bychyzbk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ndxwutdj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wjzwjkrz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mtelvezg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tqgdgppl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kbzhumlf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2olqjqmkd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lmczmrnh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vlitqgii.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2niwypoxx.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tofdbpdo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2anjbeixd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2arqyfvfu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2oibewvqo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ertgnteh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oiuffhqs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2jypemigo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmaabao.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2duzcdmyl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2aafnjgge.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vwzneuac.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2uxmxkzcd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zhndjazs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xggwughf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cgaabcot.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2rkqfgtio.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqwemhv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2goxfzsph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjuzkcda.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pjcmlkcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmhyezhe.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2vprnkkfv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ycjzlymb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jnvyjmol.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ulclqhxi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yaecrxma.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2flpxkocm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vegvrjxi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vdbdkpyc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2obasjdqc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bzwlndwr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2khmsrvmo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hbxjrfbr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2upffppou.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2epzajxno.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jlsrtokx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zqzuoyal.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2voskqavj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ppwxznlo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yxithoza.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nbydmafx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xnxymlae.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ktgsjbqm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ahwkcpfn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2qluknunv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rsqlzvmn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2nwqchxyz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fpjkerct.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2oornphuo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bknsfgdl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ksncdwzf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dtuiqoio.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yhbewmbe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jhsxatee.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ugheqbis.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gfdkkhhe.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vvqrhjgg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bdnuacmc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kufkxkat.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2dfpjdwjh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tptihtqn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2agqdilbc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2hkradzkc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mphwkqnx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2meyqtdjl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gziorzoc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vhbnrfwg.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xowuzqbd.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2szjpdkcr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mjfhskld.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yggmebuo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zffkkswq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ocjlaajy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jxooiumo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tnplrubr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jnpwxeiz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ttdkglrm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wptqviwk.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rqjxbpit.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lbjofjvk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nypooohe.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lwhhbzdj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2uxxcagjj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cjfyeoiy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2eioabcui.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2dgnpaach.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lhmuykhl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2elbmkpdu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mgvpvfcu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2wpxtzkqc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tbwuwfpe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fkzajtau.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mhxkuuxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsrxlyvr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kbhvchjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncqhlxgr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztqrpfdp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kvnaufod.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ulerupkj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2iqjgihun.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgercjsk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2khvvzpmr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2udxsfwcj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vlddrion.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nrqigeie.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pjifnbmc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2umydgngc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gdcaicqd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bibildmn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iaarganv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2daeduuca.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dkgiupxr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jbswanzq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lrivmugm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vsfsftnj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uitqbynu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2dlhisbiu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2szpunxcr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uwkdkgga.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2labjofpy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2haahsytu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2cxukyfba.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2crbuancg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hjjioopi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jnfyqbxi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qrcobjxm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tlrfbgsn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xsnpnqbb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2avmraxpq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qlhscrbj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rtsmzjjv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2mjpqtuuu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fukjsxaf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lisfkadk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2feblpitb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gecmdpbq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjoxwbfi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2otzqptun.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kflxwyfx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cokqjeji.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kqpbubvi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yrgsyfoo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrxjzei.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2aiofejun.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2phbiemdf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zfuoogro.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hwxewrwf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2natxkpoa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xzyecbqu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eyuzxvdh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qhapwhou.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2awuxbxjo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2muorpqsn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2whcwcvhd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2evgugbkq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zzikwbnl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2kxqucbak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2pbyilgwf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2tkpgcmkm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xeqcldco.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ibjxmydy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dqfnppps.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2txnsohok.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2necznxel.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qxmwnkpp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cornpzjj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jindiboo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gbdartew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnscvosi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rinzpzaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upaelasv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vnajtxfh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2funsrsjo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mftcfxns.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qqjqehhx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ynltyfuf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xbdvtwkj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tgdbrdoe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tvueaezz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2abeesffg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2npuwbldm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tczgqvjv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zwoiqgky.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jilnwjvb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zbjhanpd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yewnnokl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rtdzhvex.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bfqgdqsy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cjtyrnqx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vcyvotgf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mzunpwvz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2vpwycvtw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dgmzenbm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2moeoisfy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kwjlfzrx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qdjyrmuk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ibdnwqvk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2eccnllhb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xwxyrgta.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2uzgnsske.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2emnahrja.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pcdbpcsj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kbofgwif.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuaoknoi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2omxxxyfy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jkvksucv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fmsshemx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ttkmuvgz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlaqzire.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2oxpqrsum.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bllpwume.html


<!-- 参考信息 -->