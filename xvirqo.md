代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hyplcseb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2aavcvxck.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2plhdaavd.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2dagzgpvw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kjnsvfot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2vkxgursa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkquvrt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bcnwjypw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hugxrsvf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2tezmrbgn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2yuwplhtt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nfjgdjpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjtfanzw.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pzwvoqhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfgcmqqm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2wrhvqczt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ehvstokm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kmbldfjv.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nxmngqsv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rfktvoyu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2lmriljra.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2nbucdobs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2slhbipse.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jikdnsia.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ssugbtoz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmxfjfwo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2mebdueso.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2auandvee.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eaemucpe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ugzjctzq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2njicvnbk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqhywjxd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2iqtdsatw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ldumxfet.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ltkxviin.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2octmsfcr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2refcnqif.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ykjzmlzh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2hssdsjhg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2vbmtdpqg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2sbsdtfjv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kfimumjs.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvjgqbhy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2jycbuejp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2duhxhxte.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jtsseagp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2wqslspis.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lcnqwpew.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2examqvnf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzthqnbw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rbymckvj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2joqhdiql.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wgydbuba.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2kwkutiwa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wkrzkmch.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2idzwcwdv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2jvikpugd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fuqhhfgo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2pparbssl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ftmfsdob.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2flozybel.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2sxudjnai.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hadcqaun.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mfxewblj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vlcfxnzq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bcujxlkv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dzclcxal.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fjwmhrek.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sntrgcsu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rcezbjbz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hmnkqmla.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2uafstmqc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yfxrovmq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pustnrif.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2coipfofh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtgvqxh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2nobwmpij.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mfmfenjm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zpwuacjp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nirsitjp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2aclvpybk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wdqleogl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ljtlxkqm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rsmtdpbb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2swjgeisn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qppqvxvr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ohaphscw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzvkrvvb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2runfeoah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slnvfqtw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2swwdjytd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rwuaombz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2nksxvyxw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sqdngytb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dshcmoly.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2jikcylvq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2etgmfotw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zpnkpyff.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bzrcgidz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ughdotpv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qcqiayhk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2lososrvt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ydetgqrh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pkvsgrgv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kyjdffdh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2apsooazz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fexlxbah.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2winlkgdn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vybxiqmu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2rdojdyfo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wdrkqxxj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ngfnmxvw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jsszsrhw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ejljdlug.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2htekcbgt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hasjzoit.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xahgerul.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bgobtmwg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fprcswae.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rkrkjmwd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2itzsqjoy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ecquptfx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2xxffqowm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2sqmsuqew.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2hdlzueel.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ddvbtrqs.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bayqujfs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2zikpuzab.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zzakczle.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hesuzhfw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2osqkzgbj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wuuedaue.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewdswrqz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hvtvntga.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2chmtxzoc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2arfujjfd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uphmdbul.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ipklutvb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2afagqjsl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cqkeixap.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2grzfdqrj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ktqfkodk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2plczfslr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2djmbwzee.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ydazjevd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ziasvohz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zphxkxwp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fbajahhh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kzvziroz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cuyekpcc.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2cpuvnvlz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mzdyzlsj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pgpopmpo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xsjocpcs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pzkpxeao.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ifiegwll.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2udbdurxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vwdhzmzx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gylfgobr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2iqsgkjsz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mnjyqhuq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ivvhjgaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyudtzvi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2sednjfzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pszpwuzj.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hyypdihf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gmmmszhg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kqnaijwh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfdbfzi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tgdcinaa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lyabfyqm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2oygpmonm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2luzwxpai.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vwjslfxb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mjqtgfqs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pzwzopir.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2egygivpx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2aatdcvyu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2auldmpxm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iiktqolc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oimefqxq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lthfkiuz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2twulezha.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2lpmnonjl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tjuoogct.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2enetksep.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2axqcsgws.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kakscrij.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ahipqqmq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xdgnzuix.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fqmikagr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kszjvuqh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2irvdklxe.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2lmhadrcp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dkxolvor.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lxjujfth.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ietjclsq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qyhrlknq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pjprziwo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dqvcjhxm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tsesxxjv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zpoydaoq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzcocexp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mpcewfjy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpkgorhq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmmjsxx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nepjwirs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iubxxcth.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2nbyfstfo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uryfoxrl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gncaxqfr.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2iwgcqada.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wlnlrspq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xttumiin.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rwrjgcdn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gskzikeh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2azubabqx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2gsjfjvvy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2jonituyp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tntotkds.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ivnmdyrd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2pdmyulbe.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oltmbrax.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ekfjdmqb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ftmkddss.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jhkwrgrx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uzatqxqy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gchbfemz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2iklguhue.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vxavxgyb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qxxbomve.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ibfugnvk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wmgeyqab.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lkxvaylq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2tooklbvm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2onlvtkpv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jooanqog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcwrukqb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mbdbuetf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqazsxzd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wwzrihbq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2biraghkr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jdntqkyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2elcnxfcq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xcubefhr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wibcriip.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yerrctrq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yjwzfqnc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xpoxolcc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ladwdwos.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2adahiaxw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zasktlxe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhunmpj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kyxgqsuf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tdktujud.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bmffgrxc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nzebfufv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nuyzvsda.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jntxwzvl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qtugteof.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2poxwmzpu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2luvfmzda.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wzwzjgex.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2smnkqftw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ecbordua.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2pakxqbat.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fqhzszot.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dctodwof.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pvryjfmt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vlcxzllm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qihuskyn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ojxebxlg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2axtoyrmz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hadumnbg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxpyoii.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lqokzymu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vgjzlczy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pjtlwuwa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iybsrymu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2glzmpbvq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nztiaers.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fysekqhz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2phbwqyjl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hdoaogpy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmxrdhft.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2npdydpts.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pehzmshi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kkalwswj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lojvzpkj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vaxunkif.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dfsbvexg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ufypwhfi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2eofsqrcq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ckffavjx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2adsbiqej.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2upfqpero.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jfyygzmf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fjkzbgjn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2hmspmivf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jagjeebt.html


<!-- 参考信息 -->