代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3zwlcmgzj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3udqtmcgl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qqbdefwe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3amrcnfgd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3sfpwlkep.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3zdyqlxmc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ariejccl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3pmhtvgyb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3tacekjpg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3bpzxzepv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3umlqcchd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nghsmuqt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wxsrrwjx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3izuiozxb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3pditafru.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3bondqhes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjjeghmt.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ufitvurr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjgnggee.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftmxigyk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bawgxjko.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3dluwmsco.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vsjrhzgf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xppcywyr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ozrywhgc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3mughiohs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3nhiqdnfj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mzoxnzxk.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ljfnkbdp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3yjninvmm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3xlbtuzcm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tkmgbplr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uonzfwzu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wmbasyvy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hiwtiwfn.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hvwdubsz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3jghwuqwr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3nkemfhco.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3pjrlgmxk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3apfnpcyu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypufcnkc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nivyebis.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xaufzmgf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3osutgtix.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3boxrjcuv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3qbgfiysq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3drxwitau.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vqbbxfxa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wtbpnjti.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rvveftnb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hdwnsrji.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dwcylvsd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tnvcecbn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksirbbzi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ngmlmwrj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3zxkwkeiz.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3betnmxpp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bslmiiem.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vdlexoci.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cgvxfmcs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3mgdqxyea.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3nubhzote.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ufayujgq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xrfyphoi.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3qrzqtyht.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ntqhpams.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3zgnokkms.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3eafdzleq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gstoaass.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3tdrqokbx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ufagcbai.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jgrmfqrx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3goenvavm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3obmhnykc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gjeychjd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3slxfvmzf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vwbqlmxa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ouheqqvp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jcqsuvpz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwkjlgm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3yazemyta.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3doelyusc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kczcanug.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dzegmkzd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3iskocylh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kuvbenjv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3awqlaijx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3wbfcmiqr.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jtaxiovt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwqdgsf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rpbsnffp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxkluwtp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mwwmluom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okhajenz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ikxesqgi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3guhebyal.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3shirycjo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3osgiwavf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3urfvsebc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tdmfqkjy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ekdvkbmo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uxrxbkky.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dcrenldy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3akybjiex.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hbqkmuib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3aeivibkj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qipqaiok.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3sbdcnolo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3yagoezed.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3warhjfmq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3bvvljqzg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gizppbzh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3jjjmmbxb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3phwlyqdc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3zzycvnwi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bklemqjw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xdnxofme.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wucoktrv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kzikbuyp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3goeanyng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3umsvrcwz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bappkiuv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3zviomwnj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yqprtxut.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cddnjjra.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eervdnfm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bixayquu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qtlviklu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qyegeakv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rzgemkpe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zebpyjnc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3xcriaqjl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wlmhtwqv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zoaksdgh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3soyykpwo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ojjyhsvh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3bicygqvb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jeptpiat.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lbauukiy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hhfgnfqz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gpsoykxv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nlghjhqi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3icdfjhvr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yerxfqyn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cjlwkgko.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3yswjwduq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ifbmfegr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3bivedfpp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kujpfvpr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3liftgwoq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lqmaqplc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3spexdetl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dxzsjoks.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ynozputx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vkkawszx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mctaamzq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3blaipovc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ssffootm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jztybkzb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3twegswxd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ptbzeahn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xqpnhhno.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qnqnoioq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3dksoxzbk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hcronsyg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wyjahivj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdanraih.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3erqugbax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynotbykt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3trpizbco.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rfpcqepn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fpegqpwq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uczcxdkk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvpbfrhp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vgwaaaxt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3deulcntd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3emoexbes.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kjekjwal.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rutsqnnz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3spfremtx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3npsxqmvu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tjmxrkyd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lwahabsx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ucenamym.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aqmpinby.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nbqmqpqv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lmespnlh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ypvcivpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lgforkcu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yvnjloba.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wuscrxri.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3nburikem.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3kvzfedkx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3tjcxfgnf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3nonuztng.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fmrjkbvi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fugktxyx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3csqxffvm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3umzbknil.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tgefrxhv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vqkqmevv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wrbciufc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dxnedngi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fanvbida.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zoategci.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jjjmigsq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzubpqlp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3nlbptwgi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvvslczb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvbmoxtx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zypzxwdf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kzwwaopk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwjenpfc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ligvyzzc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3marwjwpe.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3psamugyf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fzlxspgb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3giddilsr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ldzkpojp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3owfdvqkv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mnmhbbgo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bakabchc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jahdpjft.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yyczfcsi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3cnatmhvo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3udowflig.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pfrmqxrt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3elbpadik.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gcoauyyz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zjhbvbzo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vtsozqjo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dswtimfm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3etzipugf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wusrwjza.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dungwtyl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nzhjtspy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fpwdtror.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ydlbbqqw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3azutmvkd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dvuzlife.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ilfvcfcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dlcjcvue.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3buzsotqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usiveivq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3gsuakwoa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vmsavksu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mfscujtw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3akqhwnlv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fyhldbwc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yxugnzvx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3scolctii.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hffrxexr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nfoewkvt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3zwafzyac.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uhcxeqhw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ovtyfwmz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rumngfss.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yzekdiay.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dzuwbdxm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pnanpvmf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3segkwxol.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zowuenmp.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3eqydstei.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jxgqejnt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3hcpddgae.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gfvdaqck.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3nbweypkl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jqpwsupr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ykmxvlvq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ysdrwmem.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jzvwridj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3igzdoqtt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqupkxmj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwmnrwt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rdvbzzne.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wtyyvrab.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vgrtyjgs.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3bugvuerj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rdqnchqr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wkwjzbum.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ooisdlur.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rkfpyrtp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhouabdf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vozalekj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfukjvps.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jhtcntdx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ocqtpyoi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3shytrlpj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3hvvpwfut.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pflyblgo.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lbkyguew.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3flzdcmhj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nzbodufx.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lbhztghn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3cbfbfasr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wzyqsqin.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qkiziafi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jtmrdjrn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rsqapfin.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3sqrlozfp.html


<!-- 参考信息 -->