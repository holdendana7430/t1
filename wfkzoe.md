代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2eqyxzjle.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ovhcvmfp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2lpnpozzx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2lkrldfhw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wzzvlyse.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2qcgqksgg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2yahkzfna.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2kxwwemfd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2blrysubl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nwngwmda.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2metcrwpe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2rgwenhtj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2iakvhaxf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vkqmdicm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ldbicskp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2obpjdgui.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzucwana.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2dbbhonal.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2muiitzxp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gdlzpeav.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2upwfhtfe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jxuhyetc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2nboovttp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzaaosmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avrzoswc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2krgnddvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adbchmop.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crwbqart.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lmwdcgss.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mvkuogfh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ojpistbs.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fffaiika.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2uvswozfe.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2iuhvdarl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vdnjzfau.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qypevauh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2obnxxdkk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2lrrtdpck.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rmrojvea.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2axvtrodb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ffqhhwbx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yppmxagx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lyzlawai.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mlgvmcob.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gpapevvw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2nzksmsvz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gjasixvq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2yqifgetc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygpzlsdg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ntvwenzd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zrsqkfrm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fxylolnc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tabcmlcq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2lhzytsfk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mybdtdnl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2huveyylw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2pvfdtgnq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zofqzxlr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cfiyjscc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2aifyajyd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2vpvqlzts.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2byhhmedx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dxsauhkf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2clkovhil.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zgklmmab.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ksyovlum.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlqzktz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nczhnzpy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2gxsjtgfb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2twbnsell.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mkahcbhj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2mikvqvqz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2elixgoac.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2htdavhgr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbpuenwe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2raudeywf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vxdizvrk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2yhgcpgsb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zpcinwao.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2payjsaei.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vgfnyzqg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hzzfbnqr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eliukrwm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dsuilpoy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ckrfsbuy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wmhfeqqr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2spllkjaw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnbwylz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hcfbumwn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dtmktbwf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2tvhxictv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vavnoadn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zojemmvi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2vfqbrdzk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ffiltyga.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vaeaxcqu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2hnupmdzt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dbdcxhqp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uetfrlai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqkzdskn.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2tcxbglhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxdybcdx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hjpsmkla.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2potysdpz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gtneyuzq.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bzglayql.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lltzgnzg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pwedkbjr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hyqfiebo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2kaqsbkht.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gqrpnebo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jsajwhbv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yfqkqegi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2giqzjaew.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dbuqntkg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gzhiddym.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2chaeyrcn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ugvnggoc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2zqvqftcx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ryzokpoq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2gmrvznrl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mhuzsaln.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2frsdxuhr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rdrvobwe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gvyochgq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2grcjjjrc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2msrgnkze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2fvdyhatr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ygijadsj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2atohyodr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jdrtxoqa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hyehsgiv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kdnlcosc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cjrbmtve.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nusumaqy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2jmujcqmb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2joadlsqy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lumgwpvo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jgyfiwgd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2bgzomzlo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2syvdualf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rlpmkcnq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2svixgbtm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2gjpbslvw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsxvocgm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2sxevcnod.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qqspbehc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2urvmpqlx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yrejqozr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2isjnwtfp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gqoitaet.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iwclfcem.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2syzebksm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gfzawklo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2llcuvmvj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2usiffywe.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sjylwbxh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2amhnecjd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fbmxivuz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cgswpket.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wpsqwctf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vaypxhqv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pggdjqkp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2eqpivqyu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2udoqvtls.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2oxbfbwlm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yxcmcnco.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jpthyekz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lpopfxqh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2akzykece.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2xzymatbs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wauxlsxa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jimwfmju.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ljpraiim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypdmpiry.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2itatvudy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfoxkskt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ioercurl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iyidbrkp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2judltdzb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfybrwtm.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jtwexghq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qtorjaej.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2uyagqsaw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mrtohdpv.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eqvzoxpv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2odymezwh.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tmzyszav.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2juppxoeh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sajuvyjx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2deacvnlj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hubkaunj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nyqjkoth.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rcorjzdr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dlisneqs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ewvcfgzw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2avqmgway.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dlvfrrvv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xywlmgdi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2duylnnhj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zzwluglo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2qobpuzmf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dpltmeoq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kfgyfyju.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tftngioe.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2szyrcbmv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zzphkmyk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2bmnaippk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2biimbeec.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jpdrxdia.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dzwvqsfd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cdbofzpx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2anbqywte.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bbhwpeqd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhlglqq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2vupcoper.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bombthum.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kuydaylk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xirydxmf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vhhkwcau.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2lycxqpms.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2cwdecrpq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zlwrwmog.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2exoexpbu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pacedvwi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tqcycekt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xochpcxu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jqyhzwwg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xxwbrdfk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ujulywle.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gmgubgwp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ksltaeeb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2nqjifhsu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hvsisogz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hniigovb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bjgofiyl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pkhcryua.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2henbwspc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2yftfifph.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vepcfwwl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wceestkz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dnlzsqih.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2cuilncgt.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xxtnpgjc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bvxwjgia.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wifceihk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fmxlkdjh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2qzyqobfa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ildoaxbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exvybfrj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2hdywvihb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tetbuany.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fbgvhscr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2syzscmqv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pxmwnwth.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bklrjryv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2teidxias.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jzanloml.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qatijpgt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rnqqkacd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lihhrrjp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rglqnorg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yekibveb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2utugjcel.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mbbczsfs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fxqrazvh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pqgwzdec.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sxpihydk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ixgvkbgu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nvbfkbvl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qeytpnbg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2dpskucvy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kdcimnlo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lmyxxbwr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2sukbufbn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vxqnbxya.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2umaryydl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2oujblllj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zjzmsfwe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sfhimmii.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2akzxjumi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2febywbsy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uqletdan.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tgpxfqky.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nakuumfo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2oyzbkxzx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlbtdag.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mdrsboka.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2mxgmjdyd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2arritxhm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wytfncrn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2berugnpm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bmhclyzm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2idtuqfre.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2razywzda.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gnrgswwz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vxktsbqf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2fezuvqko.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xsflsamr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sytfpphz.html


<!-- 参考信息 -->