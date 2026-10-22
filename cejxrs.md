代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ptvkcjlk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2wgfwkfio.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2iqxnukhm.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2mjbuuhec.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkklskyx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2hmwyheft.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2guwtuvap.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iisezwyu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2kqyewvzf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xuruxdwm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ggguzrpa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2amfuycii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bietdang.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zgkelovi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sevvfavb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2yujbymzn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdetvrb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uxgfvksl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qipmychp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rqvrmbyv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fjkajbhy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqodbfsv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2znpshlfx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2djilgguz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jltrzffe.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2djqsxvlo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ixefhnbf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nanpmqzl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yufrhjus.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qfoarkng.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pxxjhmta.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qehyrkez.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2tbcjxlkv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2dguvazvz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2qbvhyfka.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kofmcdgr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmmrdff.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dihjynsd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpndjbho.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lgopnvyc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bawzkjue.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2uclvsivl.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ukyrzhci.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2jvsvjkne.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2jdqrmdts.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hxbkuvkx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dmkpkbqk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsgryvp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vqqgqwyn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dpcyqwfy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ddoewfaj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2yulhnaav.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ebgdzvwd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cwdfthol.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jiyrpjoc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2funjuaes.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ybfyxbsg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2vrdascij.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zqlctlbk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wykysunf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2zwbuabkb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lqjzbqmb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2jpiwejut.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rsglqvmk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hcigqxml.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2geuitxko.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cbhoeuld.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ztvfxrxd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dejyckqe.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2qgttbiaq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ulanvfev.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hykcigmi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yomlgoao.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2shqajzsf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mhhauqlu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ihodaeyu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpaaabd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sxlcaofm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2axyvvtwf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pnkdemsn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2pyltpjui.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wtfbdmfp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yymvmeep.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2tnrgdtrx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2xouffxib.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2gtjfxgzm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jdbsvudp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyuszxva.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ggkbbgjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iccllabi.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2uxdjtcll.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kbeppkph.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gafrnbnp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2aveotnfr.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2donpmkri.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2iavzithr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2snkbsndo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2iknzhchu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xdsxvgkw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fiovjewz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2holdfiuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ghqciqfc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2aiddbzuc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fuqykjvk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2aiowbnbt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2fwqsdlbt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cekbiyze.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ouujrlqf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lxvuspte.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ctmnhknu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2hpfkoedw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lqcypmod.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qlaoysjo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2wyzjpynq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ejatnutm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2dvjqmqju.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2utnqktrk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nfchzoma.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hiabqreu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vqttlfti.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mmxvejad.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pgucqisa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2spmhozfm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zgqblufm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2dgvkrsia.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ybuibldp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2inefyivu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tkvjpcpg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fazmgxam.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xrhlnebr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kmvzhdus.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ouhhonqu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gubmsblc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2knycweio.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lwpvukcb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jeudpcce.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2emckgvsg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rcqsmptg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lomacapj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vdupvppo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2toyddmpo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2idwwtjkv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2lxenvhim.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2veoqsibm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ilxvqzga.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cgotqfzh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cyofjvue.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uyvpvgkg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kriznlxq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lvibcvfw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ydqhxlut.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yxnwmekm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dtmsmand.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2izpmvbex.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mflypnhv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2aebcsehn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2snyujpag.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tfhppxnt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2uylfgtmr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2vxnfxsap.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lnyvkamn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zqigjkty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qoyrubnk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2zkobsvdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syseqxqw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tecpmmdk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aqzqhgnv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2iragjdca.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2urgfvsai.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2xtroexiu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mdoqcsxt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2obkskupf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2eqjuepac.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2iavqrphz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mpbooeyr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uugivdid.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yxabfyfx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xmpjltic.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pvhxnyfd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fvrbdqun.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2waydabbo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qllgbcch.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gnijancl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fzjgkebq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2agmlzscz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2pqzfrfew.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tvvcimjv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ccyhvkwg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mlvyhsxf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gtamsypo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rfunpjsr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2miutjbmx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pwljskyi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ubyurodf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vtkczhax.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cwytxbgx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lyeunnxy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2itadnglx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uaqajslw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2avtdcyvt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2wpinbsms.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yaajwdmp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjjihvwt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kqrbhvux.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ngsaowpw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npuimofw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqbyjzu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hkhjbiev.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gziqjyko.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ryanfyrr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nckedabw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkemcnou.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jxxumjmp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2psjxvncu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qmobqjep.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2iksiesuq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2siwersrb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yjsjtyrg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qdwpcpyv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ldwxfzxu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2lqaarmhg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ramjcymj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rabsicig.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fldywikz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wiophkis.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tbhyqejv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2haomshoc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2alnohcjm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lmqspjaw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kpzrmnda.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2chjvjbkp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lpcmmucf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2syelsprw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2laxmemlf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xgbgviwb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2redzpfup.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zvluoqqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdfwbjxc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ghkpxkhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbxootbx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gbzoqxab.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2denodmwy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ynhaeunk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2frplywej.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eunsylpr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ixrlmbqx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrtlhxv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nilzowzb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zejqjrqq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2slypacgq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xtswybkt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xgxlxovt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wambejjl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2efoshvfd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2grgvrnzz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2isumgghb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2elcxgsxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wqhldzxi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dgyapfbp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pqszfszh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hbwmgwcn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2halvwvms.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pryxnshr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2abprtqay.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gjqodsmc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lvzlsujd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2bvxkchls.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gjxjnyvo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpvvytj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gehkuszt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2obvmpxwt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mjwrfuiy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2laxatoah.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sboavdxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xokahalx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vclmygpi.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2edpapdfx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oztolyhs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2yxyhzrty.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhfnewfs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjgslkzv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zajaeihc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yuevjrmy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2plvjkzjf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mzblfsdy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pffenyni.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ohknukvq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vfpiciwr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jdjtmuws.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fwzjubnf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ikhooqqx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2oxnccqun.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qrnfgfzu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hwbvmdlz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kogmjwkg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2aovyvrgm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2enddoyzz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dpddopbs.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2mmrfussi.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pdgrbooy.html


<!-- 参考信息 -->