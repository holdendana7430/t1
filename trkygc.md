代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3adflysxc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lzdfzyzn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3cmagxhzy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jsjuxrre.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cjarwosy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwgoprx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3hiracvlr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3bbdlkiml.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cltwelnz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3bfzlcgew.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3dolenjbl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3oyfsubbd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3hdemfdkx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3gwhpxvlt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3mqbkmdts.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3cynyhsgl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3bmyggmgu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3oqxzgoqg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3rfzmbtva.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3qxqzjaws.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3kinzeuow.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3stpxtfkk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zyckivyf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3excynuxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3thynvakq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3wdoqltsv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3vwkuoday.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3nrovdyov.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijznuftu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zzetfnru.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwlmyqjz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3storpjsn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgpgzaqs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ntjgidqr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rmnhnkwi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjmyelpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pldqmatx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3dteowhmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eabwyghw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ujwdosdh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fmyifffz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3edkcgxux.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zzvixlci.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mpjnplpb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wsissxtw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ughecmcr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3lqmmziak.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xosakxgr.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3aqzngzwu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3quoclqnu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zbamlvbm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ffvyzmnn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3eoustjzf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ontqirhu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cgjfskpa.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwfbdepk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3vayihbqb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3uubfgesx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tsctadre.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gqnvynxy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3maxxliai.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urgakrqs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivtkrcsh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3rzplikcv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ydcdznyy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3rsjfdgmv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nlehnlpq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3shpljkph.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3cmpydgnp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zybfrise.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fsqspbvp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kkmmmdnz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jyachekz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qcwkelcy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cxlhrqpk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3oamnaodu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3johaytoi.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3jkubmvlq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3nythidly.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ozihzqtv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ifgpiuee.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rdarwgjs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yaihfnvj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3hzvmzhxf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xukpdhge.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qbgqhvon.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3vxgxjghd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3pxdeopex.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dmcwlcsw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fiewiqxx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gvgvcxsk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ljeonule.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ihwksbii.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3bvnphbfw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bnndiltm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vwoqipwr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dlhnkkdj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tzhgkloi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3obeqmegv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlqbzhm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ewsjqvjn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rljjkaik.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3fditmpii.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3hkmgftbm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hujfqyar.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jxtexbyz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dmhybtuo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3duwawvxr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mmloibat.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmyiruf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3temqhkaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tncjlstj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bkpulfvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnenhdkv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3cmjamknu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3usgosjgq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fhbokdcd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwxcpcs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bwumbhhr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3yqoimdov.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tnpullqh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lnkiebcm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3eixxhsnm.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fjturdtp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3oxesudcg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3tueuajmc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3axrcxceo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wjykmtxs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3augdorrd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lyuxkccc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3glsjmmoa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ctbsppfx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ahafmkuv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3cslvxyhy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uihauddm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qckdwphe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wphchbyv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tgmcuzqv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3parlsxnk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3kfphapxv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kgnzdinr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bdrfrjmh.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pudqnwdq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3diaithmv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hqybleth.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hrsyhowd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bezsciiv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3vyefdjnh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3smfbavhq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3xgaotrqo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rypundio.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3wbplizli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndpblrav.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kcgqlkhr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rlhalhlt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wyqzslzz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xoggxcan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3dgpqwhgc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ahjnzyls.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tyunltai.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kmvjopof.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3manfkeyz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eztganhc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vpasmcao.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cysekvrm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3owcdruvq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3knfwcnrt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zsgdohpg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3odszblmi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3dtvocqnq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wdwwwiaf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rnfmrmzs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3shqkbtds.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tsncfjzp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zrsdistk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dgwqdvhd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3glbhmfki.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3usvzmsbc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3kakluscs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xkwubkxk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xadaajtj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xmxjcfca.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ttopufvs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3iduovkge.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ccvpziid.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tidjwlqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddynthnx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3xpckypsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjelcgid.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vwcdqjxb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3whrusoux.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3djferboh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tlvlixqv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tbasyqic.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tocurobd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3zzdbkvxw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mqkcvqmz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3epmedhtk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hmommxyj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hyyksguh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vdbaqouw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3obozruuo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zepvnciz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sfilljlc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ckmooqed.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ekswylju.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hbsnbegy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3zxrlxjbz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3agfcvslq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3yusaupum.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3arlpnlje.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oaeygpzy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kzahhiwv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bpcphyxr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3zbosfjbd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vrcczkpq.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3qlnlfupm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3knlyjhdl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uuwrgfxg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ybldtuqf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jarwmtfx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3namqljft.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xcuexmdn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3pmdabqxl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dngzdujx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3npkbyrnr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rsgzvkpq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3klrqnotr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3amnsgtcw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kvurtuwd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ilduqqwe.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lueokhaz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kepwkazj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wrxundwb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3smqeqwdm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wmywxhdb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fnihfrbt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mdqszced.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tkaerogv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mikhgpyv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3grawzlcv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mbfocobt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3akhwsezd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zamzxwfu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hoqoazbi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3evnrsves.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xrkxlrsw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mcrjvykr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mjrxddez.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3wlvbdkrw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uwzvuhka.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gqakpqva.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3bxjjhqhw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jfttejco.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lbeapiod.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ktwnjufp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dtmkzvsz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3blieldat.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3avhgpikq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jcdrmwls.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3sanyfxnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsvwzwuk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kvoyksnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guhddxxv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pkjqzeyj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwciqdpi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yrmksqzf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hbtvaxrj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ugebivkm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mnsdylmy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yyvtlgfs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mptcurfi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3apefaqvw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vorkvzxh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jtirvcpy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3btcdqjnw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yxbdgarl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cauzgfvj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ghzuunkg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udzhudaa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3meinmngz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3kbwgfqyh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tkkfvbjd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fogaopan.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3korpmtav.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oqgkokzw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ydfuahds.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3djuhycvu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xhpenoag.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gvgubceo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lkvmdnzc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3zaubhuyc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mhykrhkq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tkkpeqcg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3erkupdhl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ryayxolb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wzhmefra.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3yjqvqssg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3imwhqssg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ranpfgux.html


<!-- 参考信息 -->