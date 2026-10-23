代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3stejxvew.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ixiasvmx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvfmmpf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3qzjawlno.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3nknqkowy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ezyxgqds.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3wrglrese.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3qqdgpmvb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3sfrsbqze.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ickmgqnh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lxmfgcpg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mwnslrti.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3kcbiclcq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3syxosbvh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3llkokryk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3pudwhgwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nprgroih.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3lekfeyrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzumwacn.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3sqmksnjn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fqoqulkc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3umbsumhn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oyukxqjg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hfhuqdrj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nwujbaif.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vzwysggt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qpgogjmo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mwborqmr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3phdyifsy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypofkblu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3rghqwzsq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjywhcz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cyuinjxl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qokmigfr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rkkowubd.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nznhgors.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3wktlxfim.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lcphqtrs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3bubkilbi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ftwrzobb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3guhhcagx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wazzgowk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3byjxqrcd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3djprbokd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mybtacgq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zqdwabrb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvedaxjx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xffglxxa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hqmsdupg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hzocdsds.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mxhcsqsj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3geyodkjz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3agefqcop.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3zlzaizeg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cncwfcdn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ihyhdpgw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgztgzvf.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3netekrit.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ktxidvwx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3eizcglio.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ewelgedh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3mvjrwdaw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3yptpszmj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3jxvtjghd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3rlroinys.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pcaqdqgj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3tafxozbr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vtulkgdm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cymrikip.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ifqopnxk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uiylahfy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3udmdddwk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dexucegt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3adougqgc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nwebzmwr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3bthnlauy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfkgmze.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qrdwdahi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kkysvrfc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrnctmv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jfooooro.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cvtcnwzy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qfixmzmp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3bddvydah.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kmlslrce.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3olsavgol.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iocpddrb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3pahcbdxo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3zzwaocaj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wkagwurl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rhpykwel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfhgekzu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3mfamxrja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqsfrwzn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3peormjhu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3mzvgdhpi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zsooglks.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ibltsmza.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwhcaho.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3jyazmbqu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfradty.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3tarnuuas.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gbhcyodk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qohplqdo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3crpsrivg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3mhjalebo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tgunjxwc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3krmwamnt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nmnivofv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vvkbzmez.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fgwicdid.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nqfpvogx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wheoxeub.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xhvdmbbo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mezqizju.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3dhcmovxe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vdnveumj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kybbruax.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ibhjgimg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3pmjsoyyb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vmwzuwuo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3knqvzqjz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hangokuy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zhjpnrfi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oshtlzjf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3whkvhqcv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uhrgxaml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3fkqbsvkj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3puraprvw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3nekpqksu.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fzjsgbsu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3owltcjiq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3vfwsdubb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3leyiuykg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tymuuhcj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3oqyuphrv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ipdspqty.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3jnranbqx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lerfzkfh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3defwbujm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kosgghiy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3baidehkp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ohwartjz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3njysafrq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zrxzorui.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3licqglht.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jjkdmmec.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yziqzyex.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3efyanpmv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uzcrfvyy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hfzqhflz.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ageaebji.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dbaiwpwy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ontndpai.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nghmqjth.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wtjijmev.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jxukmnmu.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vclyepwp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kpthhbxv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3qkfufury.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iyqcsppl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3supxsnjl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3bzgjnjby.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3lnwvsqre.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rviyiwtb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fxvbhiti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfdgcsov.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3prlvqlpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnmpgbkn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3sdsxyago.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xpdysepj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3yzjjzgjd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkwacvx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3byrzfynk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3evkbehfn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3meujsldf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zgcurhen.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jjruhlbc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ztjsxscc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qjytdqgf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rmefebmy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ucsrlwxv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3jlptjkru.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3woocsycm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tyhvriqa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3dmypsqyy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ilkydinw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bvozxjge.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kixwlifs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ugpanwxa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mlmklwgo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hkyjkqdn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hnjdggcn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ymtgjdoi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ilaawykq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3slyzijiu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wfirwdft.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3aitnprrh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gtcfikio.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yavqoyyn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vfwkbcvf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fgnkycfk.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bbkoykgm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zitkohja.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3akhpuxnl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3equxhcds.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldprbpbr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ixtnnxpv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vfhxibmw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3licactka.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3anoorrlf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgzglyei.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmjoyath.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tlmflbqz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tbzeiwsz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vawlmmdd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3jtcmbihk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lqchjeqq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dacjpkpk.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ptctmawt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uhmulphc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mgzjihkv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3slvjfnhd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gazlwekt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jvhexqwm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gmnkrsnb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wgsupyfk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ydyontey.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3zyttqkjf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3enztzvuo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3sqfkubxo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3khlqpsvn.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xzhnjzqz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ziiaaaeh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3qkqjnsli.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dtyhjzdy.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bxoqwmro.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ajeqeskb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mbgcyxza.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3moxohrrp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zcacdvsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckjsjpej.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3cjarakas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tuslhlgl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nnaytyfm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lznamlvf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3atfkgfgk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dmyiqtjg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhyinri.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pzlvwwjh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3whpguiks.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jsbzbrai.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3upavpvfd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rubamvrn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3trwhxnjd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ouytfusm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yyckcbdx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3stkjpnga.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ywlmrrum.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyoqqfl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xbpowzkd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3eganwfbs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3nhmxabhq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3pbhujddu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dviwvvnl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zzqyytya.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ifxtjipl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cxaqpkdw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rerpkwcv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fwbqgccb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bkdaqpyt.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wizdgsdk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qtbyygas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kveyjuzl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wtotxlkg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jnsnjlvw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uyzpsiye.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3haotmpgf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3llonzgzw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zgddrhjy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3uixkforv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bulflbkm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xelrfykm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uqemflab.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkohhnge.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fhwkkiyn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qbhshqib.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zwmxyesg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuovppuu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3timlmkqp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mfemjdzj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fynlbjeg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wdskgoeu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rfjapnmi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3tmpamgvf.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kexdjifb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3liozusfy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oiruyovv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3svbebtyh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nipzgaeu.html


<!-- 参考信息 -->