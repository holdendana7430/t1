代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2jbuulvhw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2wtzayohc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ixdnaggs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hzhibqla.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lolglzpi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2fqdpwefa.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2dfuskwrr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cewnhasl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2oiuyigyz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mxxxeign.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jcuqkmtj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2opbwwlla.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2phjuykch.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xonfmbzp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2qiehdtoq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2tpgfvzpx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2bthgeviu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2httjncix.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mqvsqfwc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbtbxyt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jxjpozlk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bwtxelaf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2lxvwispp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqxkrpui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rigciyjc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ugzlovou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2raekrdgc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rphgbrii.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2allszayd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kwfkrccv.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gfuvidpu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rserfcfm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2tbrtcfsj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ojpgyrrq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2nyjyxhmz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2vpzorlpz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qceavqew.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mivbelfp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hptbxkfq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mflmxkpo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ysewjgbs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wxufnzbn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgzpjyz.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2npcxfqyu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qahkilzd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2oijolrum.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mkmxmchj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2yvlnkpws.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xtcasoet.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbcyepw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2julyuluk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fklbqlau.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ydjbmbwt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2zdynmidd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2fruhxutf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rxetedty.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2cvvzwtym.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bwnqfdat.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2xkegnbfb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2usaqabql.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hvujqoei.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dvurcosj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2udcnhqxi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2iiwgzdzq.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2sjjkhrlh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hppwmwhv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wakmvnzg.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dffhohma.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2rfdvpyrd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ryywudom.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zbiuowvo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2yhgnluyl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2retnlxww.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2nrtvgmco.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vxcpvuln.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wtfqqgmr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dclnotfj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2immbkkvk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gbeczxza.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dbokirxd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xvbrllnx.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2frtdquvc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xosxsuaa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2rlqjwjnm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qmjixhya.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ublqaucc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2auddcpsk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hnstyhbp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2flavmlsh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ctgcndbl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2rbofgzdf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zuukguku.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zuvytdny.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vbppluek.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ozkeenqj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2nieuitik.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fvsfrxuh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2njiblpcs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vtbrfflu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdkqjzda.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2wgcctrgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jspchezu.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2pljhwtqe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2dhfbbtoy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2peyyvcav.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xoyfiegp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2omhooapl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jntdyviw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ifilrpdh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mcermwcr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2euqyxhap.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lfzlxpto.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tkqcghlw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2usojtscb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zblutbee.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yitnpxzr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cvrsyund.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ysjydswj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2flrhdoya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2hewirasa.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2swwxtlzn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zkfjyhmf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fzciquke.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uozjferx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rxwpneua.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2pwjxklbi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kcorccji.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ocfcyqwq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tueoshgm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bgyausrg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ruefqbua.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2autkhobe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pklvbngi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jnvnlgkd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cctnynxu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gwdyvppq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jfspraim.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2aubwqnaa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2upsjxrfm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2cdaeurbf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwmysacn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2inxfciqv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mmlkkymo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ecphnklk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zompjfnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2pqaqpqub.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uzxdrcnf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gvyxirva.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pkdoqacf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vhmptupk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nswsqcep.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rykufjzf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wfxosnas.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tvdvmgzc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rsmubyqt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wnsuwbel.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2oawxfatl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nmqnarwl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ehagapdi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2asvabumc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qtynnhzi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2roqqloaa.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gicqxfgn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2slxwavoc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zvvvcyqg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qtvknwcd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2imttganc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xjeypkek.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lucjhfnp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vqmojmyw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2edkzyzqy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kppypvtc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2petmodza.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xpcdzqra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyzepvzg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2iaqkymff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiazydga.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vdqyhrcq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xobwueqi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2yjtyrjby.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypglipkj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhfhyglg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mfttvmrd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ebengubv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2iohngoiq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oyhoskhk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ulctivvm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lkblbisf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eknfmqnx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kymhwuiy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bijkmdif.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dfbywuir.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ebkbpqeh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2cnywqlbj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wqgtwnpg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2yisytjug.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oylwumcl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tpfnwhcr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qlvvvtgs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2igqcxnyy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tdglgbwv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wipljhts.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xirlrcmn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ggcqzolg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2csjpdbxs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tpbjpiwk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kcunfdqt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cfuasnxp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pwxhpyhl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2jhujeveo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yhphzwml.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nehuyafl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iqkqqldy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2argnchmj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2swffxuov.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2jdslsnyk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vvrhqtjf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhzmzco.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mfjtbdud.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ogyvgmcu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2yxkpjhvl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2eypbnitk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pslwwkps.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ilvwjicv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lxkldqzd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gkpxtmyf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lvsgivho.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wjpcnwil.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xrroolgq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2evaqabck.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qiyahbeb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2udzgowlj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wszagznv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yivupmuk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wbobyxum.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ogwpavic.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rvbazmyg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dfiqfdnc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nzabbnap.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mqsqydbx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2iyhpitcl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nfcfxafh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2smpudflw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wgdptbdl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jrycfrlv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2pqxhjatp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uiakkrku.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yyjraqqq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zebuvdlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkzxgimc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ohxuknqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzbylbkk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pgipvuan.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqckuxa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nityswvy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qfvxjnft.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2spvabpxb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ftwytugi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xztrzioj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ydnkjohl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dsofnivt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ekkmceou.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dcumvmzv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2udkpnsid.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xaaiwtgt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hakyhzfv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bkagbnxz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2trpwymen.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xreqxivo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ylpolrsp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2jsvbjgrt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gthaquej.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xghryqtr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vvhpbaop.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vtmyfoyh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cxeycdim.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xjkafqtm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tlrtjqpp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2apoqoelt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jsvizlll.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2naayczfq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcrimtjp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ssktcgka.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nemkszdw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2focjocjh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oimnmznf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vwllabpm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lfgxyuej.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dlvdrzyb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kxwetyls.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdgbvcth.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dquttebp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2swgbpsrj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ywjpkazk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2uvtthtjd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ijiilznz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwarwhco.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2vettjwqj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yzmixbdf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2njuabzyy.html


<!-- 参考信息 -->