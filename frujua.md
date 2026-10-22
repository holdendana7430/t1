代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2chdipcjc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2njhmruqn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fjrvrhcr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ivzviquo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2isdpymxl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2tuprwuwz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ryterzmr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qjtpwzii.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2lywxcxfy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2aillwoqu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2sczcvszj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ytxlgjge.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhfxwaj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2nufjudpi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2nrqjoobn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgrdrrdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfhcndly.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2mgttjpvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdeihbmf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2cqusdppg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2sfknkvxg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rbkzhtir.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2sceeqpib.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ieksagup.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vpopcfhu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lncoxnjl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2spsxlcii.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzpnhjz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lynaaehr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvavvimq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rvlqbnzr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hlwiscnp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slcniino.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mkkhdkmx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2divxxltq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gveizvmw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hirjcyri.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2kimmaxco.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qjvhbihe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vepflugk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hxeeirlz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2pdcfxfmp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fknbqtky.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2rdbfzdkc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pijksgdh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2jervjyeg.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2mpgzykgg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dvnhsbwq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2rcghihqm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvsbjaws.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ekmusnxp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lkcbaasy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dmkcpgbs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pxszeugm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mzchsyrp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gtkemkju.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2faudebxy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2uweeppgz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jicqvpzj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eyytwfdu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wojffxql.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2owgreggk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hypwebgk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jiejmeeb.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2oiobregq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2oghvkqzw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ierujmuq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2alnpotud.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hbpabmjb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ubnluldy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2drwgtwcq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2irylidqi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xjikrwef.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wibpldkr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ooxzmghz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2onhotzzt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lyrkisqh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gaikbdyo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ybrxfbks.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2soicgler.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rtprgsme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nayvaoxq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2nhrfgcso.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mqmlxsay.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ocvtkljb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fpcpmwef.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2fdfuumpc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tzmhnyss.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fzuhfjyz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xfrwqtgw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2prsjfzcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pecrfxmx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ssieacjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nybborbf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2rgiuzwsd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ajyliubo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2vfyofdxq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2eibtcyzh.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vldyrlwv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2pdmtmsia.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yvdideeo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2owuqdqhd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lgzxpfab.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sodagvpv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lhlrdykz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2sxcsmcxm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2efntmbxb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2eubileua.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2nlztzvcq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hexcckdh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ikvlymop.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qgivimxg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fqredcbj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qogiuywy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cknrayjg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lrfbtpkm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ctmwkagt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2eqxtnbhc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2htkblwlh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pzcoinuf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cjqgqflp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2inxxmuqv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qwrecpbp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mkttpgom.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xakxzwfp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gvsmksdi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2skcahqsw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jxyelhap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rhkgtpuu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2atjhazhd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yjldzlyb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ihqtjmjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2aqjfdkiy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2blpudqbm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uaoemizx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zzhrgmei.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kusobexs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2cezayzlu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vshjjgzq.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2imcybxgo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gdookmew.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fqcfdxjg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nwxsvggd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cqyopukf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yrapbrkm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2njbuelex.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dlzppxjz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2oimfixoo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hltoryap.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2eifqkdph.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ncixnppo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wcgnkvnl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wqwqabsr.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vsecbbgu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2slfjfkpa.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vimjqrub.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dlnnfxfr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2waomurbg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pjbovthy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cmhfjqrj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vrcjpvdo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gdcyfsul.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mqwslbcd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nyvsivqw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ysgosozd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mwrocglc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hkrqowtk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jhiapcpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptklocvd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvpnpyxw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pmicexcy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dwcqdntf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tvfaqvdg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kacxamsm.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ihlnkmuv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2usllwcmx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hcmwlzur.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zdkeplvv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cgnmcmro.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bawkbuiy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nmvragkz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sldwmwms.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ahmnfjaz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tqmyjjqz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ysofgpah.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kxvpxvsy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gmnftgcl.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ahdxyhau.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2yisarwbs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hmzuiwnq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rvpupbkc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jrsbnuqc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wkrcvofw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2okbdfztf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2senxbvgj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2mzsjknjr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kudtrvcm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qcjvezpo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ojwdklzq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2egjxvims.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hdxuflkj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2odavbdlc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2docjobnl.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2eabmafrr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yakfvjcl.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2umqwbmym.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hhlvclke.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bgjhlocy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2juctelfy.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxidyyub.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrjqsnwo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlqbluhe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fnneptby.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uipnldro.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2htzgyemt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2grhmjurw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hjjvqzvv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ihftbqxs.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2czolazlb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bijuylkn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ahhtkwjy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dejkuiiw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aupbyvpo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nefkshzh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2dryxijpu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2oacqhopt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2piamcqte.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2azxvjpsj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2agobnjru.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cyqodcip.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2zdsfjznc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fnpxxjcr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tyggreiy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2iksdrayc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2eklhzvri.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xjkdyqtp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fduxxisu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fpgbzqgu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cixqopfo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2cvfsumzf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jcgknuwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmqhfchn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pekrgela.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvjwxmnv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2zjkkzqxu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rmqltxjq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yqumgmwv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iosxksdt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yjvvbtny.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wdvuwrlt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzyrsnl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xherbbpg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2duszgdwi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jkymwizm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qggjthki.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zaygxqtd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cuzzqusf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xqufithw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dmmhpyyn.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gmxyhysq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2semysnbg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2egwlznoj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2yatrffvp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2cfphhlhr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rdbbnwsi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2omayiyrt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bfyxdpkj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tmbpckyx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2qttjcous.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2apctgsfk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2crlghnqf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qrfeiafc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jbhplipz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2waqendje.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2askfvlkb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ugqkvram.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rnrxudgc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lvhmpkhy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfoffnpe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xpncendc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2inemwaba.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rhfisgnr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpeabrxe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2drvlvars.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrvniuxp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qbbdpnqw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mdgflkeo.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ifqprfev.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2navnvjeo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpvkpxvm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mvvmlygw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xdfpjusy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cldtvgix.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pniutbbk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vloxhazx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2spqqezwt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2uuhzjkcs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kbxuyigm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wuybgrqa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mdkqokzr.html


<!-- 参考信息 -->