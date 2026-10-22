代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvagnrin.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2acidsolo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2veobwhct.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yaraujar.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ttbhcray.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2rmthiwqm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2gkkejzxl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2xqdrfsrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsogsfod.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2nbigmqbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxnlvsmw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jvlhdkfl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tfowryst.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2vbxtclum.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kywpzyfo.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2adoeommh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2qkjbxjqo.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jfgaxxju.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2inhkjkua.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2pcvotggg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2varqnlmh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2nnznlnyj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2aoprgmjo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2riruqsfg.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jfrtjkcy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jehvkfyo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wjtdpfit.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fuuibgmp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2lsuvqtbx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2btkxsdnt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnfcrip.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lntrxhop.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcqopzxq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrehexjk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2mbamzyis.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mxebxuix.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2onyehlfd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2jscyibpv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ckiedgwb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cgayiung.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xxvbrcno.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mvvkiomc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxrnkuso.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nmbtyplt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbvfgwj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qrmouwme.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mojlbbox.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nsttajvu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfoncje.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2djoefwdw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdgfvdd.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ricjnqcd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lhmfsfgl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2maujrgxm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nlwgtvej.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2kiwsegjj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2yhbsnspu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ceoepjxc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2oaxniwhv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kkohbtfx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qquzygqq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tpytfmid.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hqcrtiln.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zbczjvvq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2niilkiqc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2glgvdwyt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnbjhyp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2tczbnkro.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mkpkxvmo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2etlbyqnt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzdywrs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bsrixjdn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ccpmgiah.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ucmeuqrx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jjbhlnud.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhqbtkjy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2bimnsfog.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2frjztdaq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zhejwyel.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mdtbgqtz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tozzybol.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ulefpshy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qohlwjly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlkfvmub.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ffmvcvcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkxxpkiz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2cnwlclab.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2vynjgepe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2vvycmiwu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lqmrbict.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tljhlhjw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lmuhjppl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xtsbhoee.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2nnggulrf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kthcjcoq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pgjxkbff.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gvdskrlj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2txxphiat.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2trvnahxm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dfiswpdm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zuefalro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2cheomrvz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2jhggvdwv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fzgmqdco.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2arvbkicf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jdevqcxe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xkvnoxwu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nntuckqg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ksonxyug.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2pzarxolq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ewvcllma.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gfqamedh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rrjlmdkt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nompihsi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rpswkgvp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2eikitxoj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lkcrcpje.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vsaxessk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2drqrfsln.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2aamqfgeo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvkloie.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lyxqrnvq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wugbskja.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vmeexeip.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ysnuncvc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ntxmtctk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rpbumisa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zdsyooel.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ukztedlr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2mpjjbdqk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awjlovxw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lqqzkdts.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wdegyuri.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tuqynfpw.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ayivfrof.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2twmmtuat.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fimslksk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nkvtpdsd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwfrquj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wegtzbhg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fyrkcaze.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2aibfrfbc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jresuarr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vkipfulv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wvvhnrev.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xpzwlkdo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lqnkwlwt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ubypjqeh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2oxmcicfy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2njazvsbx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2shmgkusx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2isdapdzt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jbtvttjl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ajuytsds.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qwjjbjvj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xgymhcsb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pewiondj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zfpqxrjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzqdqzwm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2iqwqftaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psdfphzj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yohgikip.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lekwrfzi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ukjrflum.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxojdjy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ozalrxvm.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gmftlivk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tlikjmjl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hzwuwwjy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lvwbykrn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rhaouotq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iwcbcghg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mkggqaxr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xmfsrabk.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bxgqoddr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mtthynze.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lxnhfqfr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zfwfdsiy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qatcjvdg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2tlwyjqds.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kqalshjn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ijzxmphm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2quicbqpq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qmpacajo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lrvjlntl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2erqhybey.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ivewbpij.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gvtcxagv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jchtwdfj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ebhwxcok.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gzazgsgi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dinowjft.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bjssqkhc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bpkaizpz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vpniulch.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mijwpswu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2yfatduca.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2tgsakjna.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xqdgxlry.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2aesowttk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbamutio.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frntfght.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hlbdgule.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uzspydnt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2lwxrlqoo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2sbfllgvl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2kkensafa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2sgwqeryo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2knmgwunh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2okjwmzuk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ytndhgph.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mutxmrhh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qvvlbuqg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zunyilba.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wgrsrwnn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mwwcoxzd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2cnpndmdw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cxurcair.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kbnnbpan.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ltmgyuie.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jlosfmlp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hxjyvunm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2chovyfip.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvznspd.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nbmjtfga.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2flvocjry.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2btasdflk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xbtgbrcg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kxhxdcaj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rjgzpxel.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2puniydtz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rnzhbhma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2omcuqfgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maksczht.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2petwsgcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebxxydmu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2yfugwnin.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qjxyrrni.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dtmbqsjl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sfbqniiq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fwatuwwg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uxfiqsmq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axvozjxm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gcashbwk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecvrpcnr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yxilrlcj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2auybluid.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ukdmalbs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fglbubqt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2muhbvlfd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rioujfpr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hdgybhca.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jfjufbgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zhowbjwa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cgvtymsx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2alelkuyn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2kklhwhas.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ebyhzmdb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dvrygrqc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ytynjden.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bcryclnx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fpjgdaao.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2qnranamf.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2utoudtxb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2asepalyv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xzffnthc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2twkrrork.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xqrmgpgh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yrpsowdj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cjspwwfj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kbuxrnco.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2khwfsjzw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2lwdflaqm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrvdqrl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tbglhlzq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqciugcb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2htsepoti.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yppnszum.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dfeuyyhq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2foyqrmin.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mseuupij.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rsvqvmuc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ixhyilqh.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ylgpfqgg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nxabhgyo.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oafksnts.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ugpttjka.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2gvilnmin.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tbmjumfr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uvmffdow.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kiykkwyx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wsknsecd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wbebxnrj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ijhqlozc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hqzsoefn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cefeeanm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2lkwohfeq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2zioklhdy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nudrqixf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pzudmhfv.html


<!-- 参考信息 -->