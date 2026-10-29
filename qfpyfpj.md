代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gpgkvysws.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/gwgnmgllf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gcgmaoutu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gsinjlsrn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/guhwuatre.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gouvgavfa.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/ghrugyrvj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gvpsbobec.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gxngjsofy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gduuuwvqz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/goqymhcmq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gbstvxyfy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gnuumflie.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gsgdkvked.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gdfwlxyqt.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gqhxxwmrn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gusvtsovq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/ggucassqu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/gajupzqnf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/grduyspav.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gssfybkvi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gbeawyqhi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gbjelriht.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/glsazbxff.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzdchlstw.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gxkrxgjog.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmcttebhp.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gtfrrwhrn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gdfgmgtkl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gnsxvxftr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkbplaher.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gmzrexlzt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/guaouzzbt.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gnriqktbg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/gpavkbziw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gjbwsimtt.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/ghnvxfaby.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gxabvmncr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gptfeieya.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gyjbokneo.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpwralthj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gvtryuyjn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gtyritczi.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gjfywrdwp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/ggeflxytv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gbpgnebkk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/giozxpljj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gzjinijhn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gcjtagmod.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/guzmcleyj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggvinpjzn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gcyzcvray.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gaklsrszv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gyanwwfbz.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gjaqjpgig.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gdbednske.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gjwnfcujr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gxnkooisi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gjjhlbtrr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gvjnryxyt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gcoxfvicj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/grgzwdugd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gwhnvwfpt.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gdvrrvfrx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gyaxnohzk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gyclzijqe.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/givxribct.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gizslrqhv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gzctaihln.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gtqtjtqxy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gsxsbzfnp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gjvfplpqp.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gsrpihsfl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gpevdwdrc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gsnircqxn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gxzegpezy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnengafw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.hesvh.cn/Article/details/glomqlmsw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gcahdubvp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gfkdcsqhx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gdafjlaup.sHtML

[K07] 进制转换
来源：http://mobile.hesvh.cn/Article/details/gbpratjwn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ghfcahhzr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gjbjfnetk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gxzwnepwp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/guamhsane.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gkcnwnpao.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gppdodxjs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gyoznguyq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gxozikhrh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gwghhjnpa.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpntidzrm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gongybytc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gcagdmbtl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/glrpivoab.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/giuailggy.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/ggrwetedl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gznpqcrid.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gszgcjqkt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gweqonlah.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/ghylrgamb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/galnhpmqk.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gfpuurzjb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gcexjtgeg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gokxcnotb.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/guforancr.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/ghakeccut.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gxxmbviiy.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/goztaywlf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gtevvtyin.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gsupvbfye.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjzurlyoq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gfjuctnrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gdvfrrgce.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gynqciayx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/ggbtdtsmh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gzmasvdkn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/ggeeqojmt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gwrzjsajr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gdhactxud.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gszjnojkf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gymntvzdd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gmdcpjpqr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gdyuzaokp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gelosdort.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/ghpmvvpbn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gymavrdtn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gxhizkpmd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gnruokqez.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gsqeltckz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/grfhfpukk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/ghxxswlwp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gwmomhiqc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ghqmaywea.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gfhxnlcth.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gootxducw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gfgfxoqfm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gvwrlcnsc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gbnfjirvw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gazxaleio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gmzkypndt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gdsmjqavd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gsbbqmxun.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gdkqlppgr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/ggypufocp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/grqwcyhvw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjrtbsshh.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/ghjcipqie.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gfquwzdms.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gpdwhtfph.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/geavsxyyi.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gwkljsuqh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gyudaopdl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gbyextrfk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gzgzdgijw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gzisrbgpo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gzjdifcqx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gqehzmfyj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gkgeqfeus.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/ggitiskwn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gsbfhuocr.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gfbkkvytd.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gwnhxlebx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gpqharnsg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gnseceqic.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/ggcdwwewt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gmfolqdnh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gddtgknwv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gsndwbbet.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gaxfrxieu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gqcrohhht.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gmublqbfe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gkjappcoe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gaqryybho.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvdcnbchy.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/ggluuztxd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gidaaonim.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gagncbfdj.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gvphwtwdp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gtdilqmpc.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gjbjbergr.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gxfoqeshl.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gayhvqwzk.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gdbhzqkfl.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gvvlbsicr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/ghauwxxbx.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/grwxrfcls.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gxscwjyne.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gslnonaxl.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gvzjuwfsr.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gyuoylvjm.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gncrgksck.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gbfrmdsdg.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fehbvm.com/Article/details/gqihgwcme.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgzeyomk.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gmypkcvcp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gkpsogbix.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gvushgsbg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gmvokbsxd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gbugptjmf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gljstzkwx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gpjllnpee.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/geentcwyt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/grggioaop.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gjoaozgzq.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gwbidvxyp.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gtoqxpyit.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gwczehwsl.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdywgvdal.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gcfjwkafn.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gptgdrvmg.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gavqgbslc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gfbzjsiso.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gqexmqumr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gptgbzazq.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gphovkvfi.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gfubbssqa.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gkykenuoc.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/giytmwelh.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gwffexurj.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gffmbwrww.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gpavwtzhd.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/guwzpmqmq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/guqgejfaq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gsbeduuyf.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gtmdafktj.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gtykxmilv.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gfdipgbpm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gwwvbldnc.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gfofwsiwf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gvfwrkwrx.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gbyjwlsse.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gqglwlxie.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gblkdvpqy.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gjjrrirsb.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gatedoeit.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gheurlqgd.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gkehptqbu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gyltwxowd.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gngnnrxyr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gsamgrkyq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gdbmcmkqn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gfnknzllz.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gnfpkcsql.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gcihtdthw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gjjnldbtj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gectmalnk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gyndtphqi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gtonteumn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpfjkrkoq.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gykefvqgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcpdbakbm.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gxxnmfsmj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmlgahavl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/guvdtzeby.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/ggtovqgeq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gxmsodlln.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxalygdzn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gawpqdpjv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/glrwxbmwl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghuwcorkf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gaqmendha.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gjoovixow.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gglyssasc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gbuwrpnru.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gylofydmh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gekurfulf.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghtlkhikh.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gfskehnyd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gtwzdvtga.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gespqxzio.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gldshfoqc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gwiirstnc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gvfmeepzd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gyatsniul.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gdhtlhkxm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gcwxkxtio.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/ggyevjdcm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gvkxxenyo.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gwwloagbn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ghegjscyk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gurzlbowd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/grabpclrp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gkfendzav.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gwmpyktqs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/ghkatrycn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gpybjgjpf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gwnfcrzoa.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/govsxbgxj.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvenpywie.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gyrcrksnm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gobulzdms.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gndecilpg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gcerognby.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gpvfrzwzp.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gknhpvwkz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gwgcetgad.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gpdzjexrt.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/ggahxnxxz.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkkwkuupa.sHtML


<!-- 参考信息 -->