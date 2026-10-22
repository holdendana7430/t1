代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrmzuhj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hzppcqyf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2panygopz.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2onkmhzgi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2lhbxejlu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ibypwlqx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ttmfomlc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2syncrwaa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yspneiup.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2vdiqkdkp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2yvzeyvfc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2clxaqwdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xulwzsbl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2gnccuqul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzdvbpsw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2txgltdqp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2aowybgul.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mebfwvzc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxidrxl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qkuzyfiy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2dqqophws.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eegignrx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2feofslau.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwcdcqys.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2pxfcpeet.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ybpqjbrp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2tvmafzyl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnwomzpp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nixhrmtb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ewtflgdg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvdhqtv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fodarvof.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mwjdmfaf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2evifzszd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2tvgzibwf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vamgjfcx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2thweqjzc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2obgxakhd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fovobsli.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2tazjsrpe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sgaribmo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2wcxyxrss.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2thjsycby.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bsvlyvno.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2uxwqgabk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qdakipel.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tfbmxgsi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lspnrwpw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bbkqvmvz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ktaazdlo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2uipjznkk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ydwmtyst.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2sefwdbma.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2pmikaspt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2csbbffkm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ajhnckgo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2lcgpxhiw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lrujdgio.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2vakhbmym.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2bhutrojz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qlwrgord.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pykipfcx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2yyrlbdcj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2wmbfmkmf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uexjofjc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2qtaevhxb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aprhygwp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tpitgfgz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vhreohtt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2tvueachv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lgouhzsi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2rtktnzee.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jxzhzyac.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bqfxrgny.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vjrbllie.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2nmvbdtrf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sbndiimu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eyxmdyns.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2swwtvoaw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iecexobu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gsymhglx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2flyaqkkk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2woazgspo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2qakrseaf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gylwqzib.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ilwylwpp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zvpepqip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojdyhilm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zzztrzmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yszyuuls.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2choniamf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2fkwuqvef.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2jpyejkrw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qtawofmq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2efzknyic.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2howqdkeh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2poulwdyp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pnsgmieh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gzmieyoe.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yfrxamul.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mrwtyito.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2kmeqfekj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kbhmcszu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ounplnzd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cdvapqrv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2iyrlfgbz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2lmadofox.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zwrrggyc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2husdqkax.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hkqpoklm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2evnawzua.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fysrnekz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zjotzxgr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vcildopa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uzooluvw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mipabpvv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2axouukhu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2jzophdmg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wcsjvmqi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yfcueqvk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ivhxikwj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fklpytya.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wxwsbtya.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2haxkuzew.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2heuvhenc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mhubqvgo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2eygkzgkh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lyydhqmc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rpduebrm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ipbzgqde.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2teeosjgh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vzcdrmkn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzkwfznq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2empktaob.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wivlfptg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zinsxzdd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cuilrcov.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gvagmnzv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2biaxglbo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2epfwgaqk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrrwtkh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2gfcgtgtj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2quvleino.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2moioodja.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2keqmtyck.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ldevreao.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2raxrcilq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mukdnvtk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vvrrwrfs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wvylkbqw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zvzainxf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xdksxntt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ijyjhwar.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2rptvuuya.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dkrgjqbk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rggfimsa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qeujloes.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vxnwlzos.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hlwqotqd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zyiyecqs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2htxjewyk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2lfiuamky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uljnwgxj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jmjadjfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rowsiobm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2edprkxtk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2voqjdxqj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pxyxlefe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2topmfqfe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlmsxdn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lhssmmxh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cqmeftbl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2shztoyzy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xfhlikzh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qriunktp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jelvyswa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gfsuleut.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tstfiubs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hwywfkui.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lvzgbirl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2krnzfsyv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2oxcdqxjs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tulldltw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2fnnhopbo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zzodlmoq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bofrgbel.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ybbijbga.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hwjbarsa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wejdwtrw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vrgernfv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mgpzynnm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kcaarxln.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rhkovtwc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2scpkprdd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sboixequ.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ozzvwbju.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wxredrlc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qyftvqze.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2krewzwcl.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vcyjdhkb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gueswhcs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sdcdmiet.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2berqsvzi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zxjhxxnv.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zibzaqcw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qfdovvcz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rrqmxnxw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uguhwvjs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2amppemvm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2bbulktqj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2efgmcaqp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2odpidisq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2akwfhwri.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jpxfsloi.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ajedwypg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dsgrtkzh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2aaqncezf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2pbuxcaux.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2olmojztv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2kyzytyae.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2fxpvjmyz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2reumvkot.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xslyumii.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zjbruilr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2lzrbvtyr.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kdnmbpti.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bjhztcit.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2smajifnb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qpiodkdy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fqamvhxq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2uzvqwjye.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vdhaokyf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bnpmqenv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tgeuwlhs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2clepgile.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rfgkfqpz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ugjtrvzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xevqeepu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xfsyzuui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtynysaz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mpwkklom.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kppowumj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zpazndgt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2imuvdxcv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wigemovt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ujqnmrhu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iwpkpgta.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rehjlhqz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cxakloio.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fxxdyeta.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2inidlite.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vrvgygvh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lcqvmwxc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhksqlwb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmmvjoh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rotnxrig.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dmglvczz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lhumzojg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gnjfqjxy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rqkmrhjo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2juqfjgee.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bdiseaox.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2eaqawtxr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ganaqdjt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zkwypuef.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2awbydope.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tejlhnrm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2fhffibpv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sefbqtjx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyqezgrc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ytivsaud.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2miftwnaj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pucdeiai.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2iyswnwcg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zfgffqaw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mndsdhvt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kgbimwlj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cxhruuga.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxcmipax.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbnsiopd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rpliocwx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bjglhqki.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qvbgtmnw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2idzuppai.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xigthmer.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2lhohgvxj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uukupfsx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dtmopjvy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zteglrhk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rwmceuyu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tjufqkuw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2emalflwv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wdkuqugg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jtoqpygl.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2buciezzb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wakjnvxx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2omnftzrf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2chxdtcow.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2iwtshizw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ixyoyvsw.html


<!-- 参考信息 -->