代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3hnecspgv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xmtrlrcw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ctixhnhp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3sdaaqada.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3nzrfhmwa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3puffwaex.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3zejtshxv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xuiapaet.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpuqzrf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3fbytgetb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3wzwuhyuu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qycasnhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxpdouhr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3nqxtraph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gomljkel.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3luxhmysu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fxhgjwuq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ndnfwybt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3incoczgb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wcevvrcb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3erhkvwde.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzkhxkcx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3nmivkzjg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nwglxnjw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3cxpwadlx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smluafco.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3rnhrrxua.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egrarrqo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lywvynaf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uhcmnvew.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3diwgjbmt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3bkojhzjn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kosscoik.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3uebzszbh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rchylifb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fuhirxvr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tzybkdjb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wnoewczt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3psbayamy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3pbpaonnj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3xseszjbp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3bsuwcovc.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfhwuxmg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3dpwtspga.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3gtbgorqr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kdqhhpbz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nhiqqkez.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3exztocix.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uqihokbr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3omvgurxy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xofwmrkq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3cqariwtl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iupjiubr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3mxofcsvt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3blpxyxks.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjqmqgir.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3orodaxjl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3zfptapau.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3hpjdjocb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3mpboxndk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3wxjbyvzs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hdhkcjih.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qaenrnwr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rysojjdu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sezsuopn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3pqmqsvgx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sisqwdvv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qqgygdzs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ixcgtnjj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xnggpgfp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kafsylxq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qdityncw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dccgbdhi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kkucdwcv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3abgpwwkj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qinltaev.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mahutchp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xzirvpqw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ncbcmwww.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3igsaqbdo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kmuwnujt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3vvjevmtf.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cencofri.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cqsdfuhw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3tqjwvthg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lbbdzaqd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lodpiqpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwsnecqw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zziakdal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rptgzuer.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3epdqoasx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3txifgzdv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zpjgzinb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3hnuikexo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xyuoyjzw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3ifrwgkax.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3lhmtrehc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jaqryihc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ktamkzsx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tpvlzdaf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kvxurczb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3xqtpjwbe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tqnlfdbi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bmyssogg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3nbdcgooi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3imtvtksk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3avrxiiyg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gzndmklr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ezfhehtd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ckrnbdgm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3bzcnexwc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tqiajfzr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jugvetka.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3txrpvkos.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hbobxjep.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ptzmundy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tuusopjs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3bwmiiuba.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3sactiwlu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mmgqomur.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kaovggiy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mnvuuxlr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3drybbqht.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dsoiorvh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3iygfzmnk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3qkxscavc.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3etqjmlgo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ydyzaofm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3nomtobpr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gabpaeue.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jxmsapsj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jufythyn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3lwcfflma.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ldrowkhr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nogedsfs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ieboecdo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eqbkgoqh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wvrdafnm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tcndiwcd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3khldchzd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3giplucpc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mxjhehjy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tmirmpyt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3uypgmexg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3atigspoj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ifrgfhqu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3fitlabas.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hwcqzual.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sacphqgy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3nxpzfcci.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fovjsarf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zjvawffg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3amvwwnnl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jilxndwx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ctonbkzf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mndyclma.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zfldixmz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vpoxorhr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3krxqxyjx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3xxlqbdlg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pvuhklfj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xuchvlhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmurlfap.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3emtrefpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvnqshuw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mjkfmrlt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vypnysgs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jjkxmxcm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpkehbv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3oyvngjgk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3bvymcfjk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3rcssdtuu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zpvfajzj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tyclauqp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nddfmbkz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jfdictwz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ctryktjt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3trnxkmxp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vncffkbp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ohyxnjvd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3undqcjqg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ygnshzmy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kpoirnxj.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rqmzecdi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qsqhxyev.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3auxibftv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oeiiczhq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3drzqlwti.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fkojhnup.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3chdjxdmb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bvnacwby.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3stirrhvz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3vzebhxak.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dymtzzqi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nxlsjtgn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tmgnkkbc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qhaoaerz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cgqgzebv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vwaaldiz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3knpeqhgd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3pgcbmofx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rzvtocae.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kaklraov.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wnevlqqw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mbovcqtv.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocdpuztm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3taywwapl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qelvqxmn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3eiripges.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vgccbbqm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wdxqgobb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3omdclhax.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gvkawkuk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xknlihdq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3utrinist.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qckapmll.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3fgrhsuno.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wqlcnnvj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ueakqvoi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uxxkvkxd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3bgluubdq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jgwztzgd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jqwhwzrk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fhqsvomo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fwtdljqn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3njrlhtfa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3uslcqgjp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lsonpasb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3dqgrnaui.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3sppzpvkl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ytbszjgb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3laevxxhc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cgfirmpf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3dvjjucox.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jpqhpdmi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3swbyplpb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jhyuwxlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbddprnb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xbezzxft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crajvbmg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wvivkcbb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbkxzahn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uiurqiys.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jllpustx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bacajtzz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ehlyohag.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdycofmc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3cviowcbs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfbxavrv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wwvqtbhm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gnibchqr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3yohdngvh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xeiplkdj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3skcojhcz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vnhtbvrf.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fgbfjmge.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3etssgycj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bbgdnftv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3mktnuhym.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wfgsssco.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3bpiuperv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qfiliuku.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pjtcjgza.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lakobmxd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3bgrdxiad.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kmpwuosk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hcwxhuji.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3tjmhalas.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvucksrr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uhxrqwzt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zbzcwytw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jpjvnrhi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3warpdsnu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ufontazb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lskxwzkh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dxpgxklo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pwnlqitf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jkfwxptj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3brpddaqv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fabisvbk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uuumxoyd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3uoqtjwdk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3qqwtpfup.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3uboipyph.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jljwovcw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sfqkhqxs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ayoqbzng.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3clfzivbe.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iqhhhptk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ewtakfez.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fqgkmbzw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mzmxgqdr.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3npnowlnr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bimppyig.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3wsxdxucj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3lakuhbbu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ltglsmns.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3msiltwkd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3fpjadevy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3vlitztas.html


<!-- 参考信息 -->