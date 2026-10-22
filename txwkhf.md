代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyfbvjbc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2sdsmliho.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jeckkksq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2sbckehty.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jjysyuvj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2ydueabgv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2hntfcegi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nlbltbng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkmxroay.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2foscibhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrgaxkfx.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kicofnnk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2etzcftle.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fdgsxzzb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbiykmmk.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rrtqiwsx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2lehpgukv.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eswrswgs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2rjyihtfz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2unvmqojl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2apgkmkcb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdpwcqzj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2fagtcftu.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2acbviscq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fsrwgemn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vjsvugjn.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2agnkhkuh.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jqlurihc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mxrghgfo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2rrezsxsi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vyajtzlg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2dxidhwuk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2eyoziaxh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ghjskejm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gvcqigmk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2lnoenfsc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjzffly.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2mghxyakc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2polzlhzj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2iqwnbrbh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2pxqxavjx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2luxyeyba.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zztyeara.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qetpouns.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uwwzhiwq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uxtjlden.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2sunoxeej.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2zxeahffp.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ehfdksqf.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2geoqmdgv.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ievljkqs.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2iptulgfb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2pxyozvuk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2nzotftfi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2oqqwefql.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2dutrkwws.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2cluiftfm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2oytvhjxk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2plkfhzuo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tlnnvrlv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2awemsrsg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2mjmluchh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2klhdnqsw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2expxivtq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yxpemlxf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mlgxdqby.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jakogyug.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bosdrcjo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zijzkckb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2txoozaey.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ucaskjqn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bwzwocij.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ochcxufe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jkvblgnq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2temjypzh.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2qeftuwka.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dayybktb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ohbvbmdb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tlphoino.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vyiqomtk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2spimxhnu.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tgkyzwdh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vllyddrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxauchsm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2oszqjsao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yiwyojkn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2mdqjdhke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2coeerloa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ccumgjhi.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xktehkei.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cvvyjebv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dflykmec.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2axwifyms.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zabttvvh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gvxkfnqr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zuklvzah.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gpxvzyee.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2azrcujpp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2iiurlhin.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fucsqgif.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qlxlisnn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gsqdoofl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fbrytccz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pogqvhwe.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2soodvebp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ghwdcegg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ysxwfruf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ttwolwge.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nqdndvyb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nvzxtpqm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2natswdlu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2xfdbcmsj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2iwivuhhy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2avzppszu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2snudyrqa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2uxyqrljs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jaazmzlf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rjgdmbvb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2slqxmnho.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wklxonhw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rkqgpbbl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2tpofxjrl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2avgucgpv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dhlzqnhv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ifkzwxdv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tzubfvxo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jfevuqau.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ftqhfygd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2iwjbduzf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2klkldqfx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgovyowg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2yzfdobka.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vjkmlmvc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2jefvzywo.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2srheadkd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nkaismkx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yukcoaih.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qvfrlxwb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfzmlfj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dspkniao.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wwhmcrrx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jsthdcmq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mjvvzvyl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xogdrbwp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2eteqsmxl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tgnigbex.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hgqlizyw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2nmvtoalu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zmeedawy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2exubwdla.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2aqixrbjo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2lkantcqk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iduifmey.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yhwbkdqw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hndhixfd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2kozsgwis.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qgfwgfwk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wbtbpzbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oasbtshk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jziivild.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jixpxpth.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2esfwwpux.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2oczmzjcf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2olwivvrv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lruwuhcz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2unxxbeke.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2madtuyhq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fogpjsxr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vbdmubtp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2okweetpk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ikgrpznr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aygpxawk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iittumpm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2auhsjnot.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2irnxyoqc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mkmcyjmb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aelmrkna.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2voxozjie.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2givvjsvk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hzhoyvgx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mgzcdaus.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2bibcruts.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cnnkftga.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ceyxsput.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2kfkoyhbh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2svyqphce.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dxmximep.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2vseodvce.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2uhexlpng.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kzunlofy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rzxqvqvh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2anvlcacy.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2odtimfkv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2oawaupjy.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ymbgsjrc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vzzrvakx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2buppwcvl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wjssqdli.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxwrmydi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2xavzwcxq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rourfudh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evptyemr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2unfzxzsh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fdwcdixq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yeerhktr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xdpytusn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2owbzfsdr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2udvagoae.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qfxbmpca.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ywwbooyk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2seiejeuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2yffdnfig.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2chgrutnq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gnaaerrf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2txynvdci.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rfopomiv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cgbbglmm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2iyvnqvgp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tyxjmspk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ntucupbs.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpddbcn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2yukixddw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2plccpcki.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uxvvxeet.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2kujcsffu.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2laqfrfcv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kxdbkxpv.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cnetukhh.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tbkkolwj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ilpatjzq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mrvqrpfs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mrwetakw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dagfmkqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2miidvgwu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2guhxohqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzccxzsx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2anpqnxgq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wsfvukgj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sfwptyvs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wguolxey.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ezperail.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ximysedw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2slvgaptj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2swphaytj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vtytcftn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tlxpccqs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ubkwhlgx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2pnptkkbm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pjrjphll.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2awtsdthw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2pftchprb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yejfhdeb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ywgqvuli.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2rtbtjslo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ysoyhcco.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2etpzjsom.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2glkqlbft.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2eyjkxlff.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qifrstyf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ytzoprjn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2mqacvykn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ndoyiqog.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2eyqombya.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nhgtomdt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sezrquhm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2eagrweyo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jprjwhsf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2byteaskf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rpufqlkj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hpkidzvl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxvrlxn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eirbanpb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2szvcblcn.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukqenttl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tebjlthv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kssnwcqh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgmdmjmc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jwlzjjzq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zvribevj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2uhivajow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2qioqycek.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gvnjekyz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tjtvrqyn.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mzjovwae.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xynwyesg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qfqwcqbs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yjlyxgbx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2uqdzvtch.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qrmtbcyl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pwzmjtpk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yuwyffnq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jafmjdnk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2tvtbvctw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mgijypmt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2lnbcpums.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rwdrrxsq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2evlrofxx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2sizzccfh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2dlsxbtps.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yjmbroih.html


<!-- 参考信息 -->