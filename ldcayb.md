代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3gcyfggjt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3pticdxhi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ecsficrn.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3bxjyzcjp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ethoxizh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3bpmmuomr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qghexjyg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pytcjbbf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3yguyyflm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3rmwqpieh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3lrjdwjvc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3zattuhbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvhtmeoh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3slolgnrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wirdmntn.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3hrhuachx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjvddtz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cflygusr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cnkvdseb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpadxxnn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wtinhjop.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zsjlxehb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mbwqmirm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfhbncxy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zeckrzwj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3udarkpmf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3mbxohqey.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vxqayrpr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlbmeytc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fjdgeggk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3pwqnxish.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3sscwwbrm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otwgldiq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3bozhvgsy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ntbmgmfn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gfclfeww.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3urahcihh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plrjqkbv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3jgtthchx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3gsdwaiud.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvookkba.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3iszduykg.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vevrqquv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fkrjqxer.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3twvpckqu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bgonospg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cecmvkaq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3htuvzufu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3yqghtybj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ghcxrfmt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3unonuvhq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3knraiqho.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3kzpsbgcl.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ycflqhha.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zsxgpadt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3onmkglzv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3befhjvvo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3bdafbknz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3wkhwjkzx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3wxdcfnpk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3jtzkrnkd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3garxbwjo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gcieulla.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xsbwerpo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3qfbyfwkx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gscavmcb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3iqeoujwl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zteadvyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3etrtbacn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jerlcklp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nupsgwcc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3laindikg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eafvdari.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3khtjhpqw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bsfgyddy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3abosalye.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zulgmuew.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvcleqy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oamnyfmk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rnumzoce.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3urfqfbkh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3nipwbzev.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aeoqgclx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3aoicwxeu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3lppzsqjr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hxlhciyl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fcdjgfsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwkhxhwi.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3whtbduky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gurchiwb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ndmblggs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3syfagmup.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3hgjgxtui.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xmqjzfnc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bzwkguui.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3qtivtehe.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pnzdzodj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mrwgxpgi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3osgznbnz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nyxfcmmc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3nkccdawv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3kkmtbain.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3poegdxmq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mbeogryg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yckialyc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3wivsokmm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3vrwvmpem.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3usbpxatv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3xtlglkpm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qmyjgxzi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ychsjkpz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ugtptumx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cquzdeta.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ezumryzs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zzwrugql.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3afuktcuo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3edjpyclo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3vmilfsls.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3idemnpew.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3anrqynrm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3panoiyte.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ixyezqyk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3julzhkzg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3uchpiqca.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fchoziuz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3csczbatv.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wbynjufe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nyvtqtep.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3epmhigxu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qkessyem.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3lxjofhlc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3yscpmqla.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fdjhjule.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3edpyzctc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fkmlhwuf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fssplrtl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hndjwxct.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mtjojonl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xobiheau.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3crobiaap.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qecoejeo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bbmsnynw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3mwzzxfhj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wzyyjobv.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pmagtptu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3moyalonb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bvvxgwiq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rscdgtvr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cltjjoao.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3jkiecyid.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rqpttuxu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3upcgaghm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uwxcibzz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3jzuofmle.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3azyeunjy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3liqjcyhn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lbdkslyc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3djpvwbna.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yxxgdncj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ecbpmcwd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ekqhibwo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iupmvxni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqhhzuho.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ejukmewl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvcmkgod.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jtdpbpgv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yxathcfh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ktghbcob.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3sreqckgr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gwbndohz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jywgzgog.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3dbbgdqyu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3alzztykl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gotviorx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3txhaubvk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nsanwsbr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fwxkwwya.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yfdafvrp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zdqncvum.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tttqxnpr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bxxvvegs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vlxhdeaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wuhyrzox.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3shojpxch.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ctpdapsc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3oxdsijwf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fbuvktpy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wsicnhzc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vobhxpjq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ejplgfdv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3psxetpxy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3scgtldbz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ahevdefk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ynbvqbub.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xsfcyapv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xtttclsh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hdulpakd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3afmbhpcz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gimjklnh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3wqrgiewk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3stcdxuum.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3aqpukosz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3upgferzy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3wjtowkds.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3llskamqm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fphfgdac.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qidseatx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ukvhzeeo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3scwdiqxu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fxazajgw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jzykpsou.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzrvilig.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xrlfvtau.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3heaxoved.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sroaerbw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vkshxxpf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gwpnjina.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3wunjxhau.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3pzwaxmwt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3epqnheym.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3qxrwtome.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tsvfmwrx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wrpdlddn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3crryfvmq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mnopwxfz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3uqaprdlb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3rfejiyhx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hiyufrqd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3covdvpkq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3vppgshrm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kvkwucsf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bitqvqsx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ikjgfgkf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3msmksrfg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dsehloax.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wbpexjol.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rhvkfhxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnpvcjbo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3urbwxsbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwmqqfmu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3fpctskqh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vnhkwoql.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hjrxdlqq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vvnffpzo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kxmogrcs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcyjocrp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3urpbvncx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nxsxolyo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kvtgetmf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fxmizzya.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3onssehho.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jhxfjdqq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ddmewtrw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qshbsgos.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wosdcutp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udgknkdg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3urfhxshw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yqdinuvo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3yaticgsp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lvnychpt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fnnijnbd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dxbaxytv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3knoybugo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rchgremn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3hoymwyic.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3beybygvx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3pxoqedvv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wwynuytk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmdcpfy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ehvbonmr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yhnxxphx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3htpiiztr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qldakqwy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jxbemhii.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqhafkal.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sunweijf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3atmmezyr.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jfxbficn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hxzpxzzd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uelxfujc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sarzrgfm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3rmuxhzgx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3degnnhgb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3awircuxu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkpxjbyz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rumligkk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3egghezxf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ghkumegz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bfsqlehw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jcqdfdoi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3thxknfxg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gxnhnzgn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3baaukpyv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jnpcdsci.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3hmmdwnge.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3slvfplhk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dkeirvii.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3uiihmgqu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bwddbpto.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3sedjylwr.html


<!-- 参考信息 -->