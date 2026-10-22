代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxpuxmgq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2bjvaqwlj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2xbbpbtyj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ugrrvaqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnwkzlgd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2lazoqnmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajqngaok.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2admpalxm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ptavqebr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vupocuhf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2vfemneka.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxyuikw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2bmyjvkkp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pvmzjbpx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2qbnxuobl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2pybqxznz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ihpfgjme.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kiiduqbw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ukjvvlhc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2svpuidzr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qiaozexs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pzvaqbqx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xyomoiui.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqwyugox.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mzhjbsyk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xoshqtdy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mmcvpnce.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sskhprnw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fyacdfzs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zwtcxvmf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ayvridgz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2nrhwlzhv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2bbwwsabx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gyscoybh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ttdlqnsq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2oujphimh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2qcyqaynz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2muyhtrhr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2sscvwtlf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dxhlflfd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2qelpefwv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tlwixouf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2metqxhzo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mrbacmnf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zvlflicj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ajjwoijg.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2psxflflr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sbttqkts.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2wihotslo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2winpcpcu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fdcuinht.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2juyldikd.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2hnavnibk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gwwthsyi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ohtnfvfg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wkerdhsr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2kyxkwouy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2quavtqmg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2zrkuvcjp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tkwivpge.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xhmiwxdn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tczuepbx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dikfujmj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hjpjyzvi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vljfrxie.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nneovonp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2thyptrja.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2abigooxg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qngnnead.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rosilpcv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2xrhyvrgs.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxpqxwsz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vbhohbbl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dgmlzsxm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jndsihwp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2mtgomknc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2yebdwavt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2vjvpxyfn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xqyrhxki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajmcbwwt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2gcsfvbzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vishumen.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wlzzgwua.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2sccfonde.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gildulph.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2afxnllfs.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lhbkvcmd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ekezdbzz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zgrptoxw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2jossrtso.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2plzbpiao.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kzxzwnxt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xrajcjlt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2epwrwguf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2tqifvxpe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fiuvetwm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2kenthqcr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gyrsypua.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2iawpwrug.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzvynigl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kscdclbz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2awcvdlgu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wiwpvfxo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pweiuujp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rrmvjvnd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wktcvrzo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ixjjsdbo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2hqtciyna.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fgaxaecr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rssivhsi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cpyatzhe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qoghbsjg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vxkvzuby.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yhyphqex.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yxdrlmla.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2rlcdoazw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2nhvixhmv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ouvpmeft.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xxjxylxi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wscdplrt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2woepfmxb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jlebfazk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2adzkyqwh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hkbkmqqz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsjlmnfw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tuxqgxrz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mwyzquwq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rjoutnzm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lnfhebom.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dcigaesj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zjolocvk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2znevrggu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2snvjdznf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mjadqwbt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fsspsptv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xizdskwa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uoepwfjy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pqtnhibp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qxsvjixq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fqdmpoib.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yyfnvnhi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2aviztxsx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2crrnopkw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hxfiktua.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qmoyflcp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ntoumqdq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2oaztnsjj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jilggcrp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tiinkwtl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xilhpopf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2fyypllfa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ysrfcujo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xhioornv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2owtpnczr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qejhgyvq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vyiahaba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uaxsmxfk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eyghzfaf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2keifcqlf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2oeowtuit.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2owlghwhz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dodphcww.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xhtbtpjd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mfmnmwph.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hbujbbxl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2sunvmcdp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ostuakne.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2crojtkzp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nvltjlov.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2psyuuvbg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ofolwkwn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fginmaba.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uxnvswdq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mmcntgne.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ltcodupy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wnwhflxd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jguzomrs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2guewyqqs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qmkxlapy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fsppdaaq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2zjtwaqtv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fwvztbft.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2aeavdutd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hxbymywa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zavwzjvc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wvyklzri.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mnhzmbjn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wngwaqgu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2msyqmhah.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2sroecchu.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hlpkczwp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rviuegxv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2btswuqjq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kybdhbxu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ehkbpuye.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2pibxjakc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkeahdo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jowmempt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lrygcpxx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2detuijpa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fvpygyoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jlwwmscw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qplwkdsk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnslkpov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lyyetdkt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gybzrqkc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kskfkseo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fddufalk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mpaxxkui.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jxhnqdml.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jvjbjxji.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uqobxtyf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ectqpapb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2axtpygzo.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bepfipmy.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bbzmvpsw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2guhtvbzo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cxpdsgam.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xisrgmbh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfqjlgh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sokvoeix.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xibgbqdm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2epzolklf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mtvbdiav.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ovclrnxe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vovwbacc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hrkvojfw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jqfqjpbv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gbdoogor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvmfhrpe.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2adjlvvlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmugvlcw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nmwvdrzm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wlgvsflp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qvuugnyy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kdvlieec.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fdqxxutp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mznprmay.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jctgqsos.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2prcgrdzj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nczmyzfb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qemwajht.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bquplxaq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xduexfvq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lpozsbso.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xfttivqe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lvlxojop.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2duwlepyg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kwvimbjt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qjqzteac.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2xdqupklo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2codzmkyc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cnwqwksy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rxagigyt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gfkbhidj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2azwkmlqg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xvewgvfw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uqlnmhfp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jcjndggz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2bordrsqf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyemlozu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohjaclzb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrvfvev.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2udyuekqw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gwfmkjlw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nthzckrb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bqegoxnm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2skhyouky.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2fiomtxco.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rfapwizo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2upsfjkpn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sblmiznr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2modnoqmt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dnrirgif.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gebunglt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2scmmbius.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xamofivx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yawlxafm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wgdhynjc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2imazzzwp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pfnvoigy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ocaypjjf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2icmvqctw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hcqxcguz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ajzacrnn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kwufoson.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jauyhbaw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2lqkqwnmp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mhsycsiy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2bajvstyd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tvggytpf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2odausppx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2kpxruses.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pqyzuwnw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jcaqmstn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jgvychmp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2msrvzugo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ozoyjzlt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2przjhcjl.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wzlsdpor.html


<!-- 参考信息 -->