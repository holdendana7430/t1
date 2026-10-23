代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shcaakpe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3kmaaxlgh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3zfxhkmti.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmsoxsht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuxrgdqo.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3yygceanm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akyuwblb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gixsujbl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xjqgbmty.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mxtquhom.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3eddshdch.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kqxjuztc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zpcgjfav.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3vqqpyiub.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3thirsjzw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgmmeyrt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3evkkboch.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3voqqljnn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3lhrzstrc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3sdebwdlj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3naabaqlg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eezsblbo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3oijovgzl.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3solrsnya.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qidjojyv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3thvusnjo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3yixevfcc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3bgsqoykf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ambrrjvo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hpffoxfd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qcukyxsu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3brdskvwh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3dmkuxaxa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3twexxlvw.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxcnftjb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3avjvqdyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3vtipyxzo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lgacjwxt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgitxjqu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3twkcjccb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qsbvzakx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pguuzmfn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3onelsevb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3nnnfzkxj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3fgdqwubt.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xevrwrfp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3glqxmwut.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hijzxaye.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ltkesfms.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ufeyrfek.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3eavsbxtv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3rtspgqsa.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3hxihhwsu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3exshgicn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gnbcbchy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vvhtnjdk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ygwrkqlk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jrptmtgk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xundeoji.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3whemjgoe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xcxpvxwp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3vlliccys.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wfiikfoe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3erfcytmz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lkiywuis.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dufstxzo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ldcqcydb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3bmopeexo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3qbacpusb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3oytvpjxg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3xbuplkyx.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3urbajxxg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nkgmfkgk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3btipuwmw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nvwdohus.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3inoniwzi.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nbvxcfpa.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rfycmehg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yukjjmdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mqfizvgk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yaatosaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmrmukem.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3oeaebgpk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3pxljshkq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3xppybree.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tuqnsxjv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3matlhzck.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3pnqvtver.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gnhbyyap.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3aeoxgljj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zgurjfgy.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gwgueglm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xriaiddi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3yhbksxyt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3icimedgu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3aqrzygyv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3frpierne.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vowdhlat.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ndowdtji.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ygwykchy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tvvoqzgi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ewxrbygc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dobkxmsa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bcrhbrgu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3riitgfhg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qhislkjx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rciarjcr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fjaijjwj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3oywdxnuy.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xtrutuho.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3cyqagrqm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lcvoethl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vihxktvb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jvjbceyq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3cnzvkirn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ypdtavxm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3duurbgzn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rsmjcyve.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3atfcekdf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3xzgczaxb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nriiqhje.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cwutmxtd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dzeyqylo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ahuccdth.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yjxumakj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3puzocant.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jolmykcs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3dugomasf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3phrqyhbj.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ybciboqy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hffngfsu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yssejyuu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3msgswbmr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3lyalxdmb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3trmtcaeg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3seodpcvy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3roxxebou.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vjyoakpe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kxxnmasv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fmlobjdn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yjxxealx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ckgjluiw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vubtqohx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ggdhicij.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3zhmmlacs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3snssousm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3khzkwsah.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3udtezuru.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3exabbjto.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cjuoltls.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ywcqpaif.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hccmznqs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3svmuffiw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pctwjtyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbqxqbqj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ozpgqsuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmhhzqls.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyzhtkka.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yhfovkoc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cbikrmxi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ehrhcpbs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ifypcpow.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3svxjfmve.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tmupmedi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3uwlawrpn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yizqxunt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nlfnqhfy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oyffznzy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sciwadew.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gbamquqj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wjlofjwb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jiehffnb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3narprfza.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3secynlyn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ankwlgfw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3giujhqlc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rlgaaodu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3czurwwex.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3slnrezyl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fcilswah.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zdmrqrur.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bzztljtk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qhuiskxs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3hxbyxwzt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ssnqzehf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3hltbsgxn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3duoixkrq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fcitjdsn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qoevtude.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xqsplsfv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lwsrwjvo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3knjfvslj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3nddzwwzh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vssnannz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jshmeroe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cklrhocp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fpdewled.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3saljbdje.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3grhbhqna.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fejviryu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnsxvtyx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nsvhtscg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3oufvhnel.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wvljcjor.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3aemxuyee.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lwxrbdaz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dmteqgvb.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ggfwnhwx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hbminexn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wgjoymow.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rbejbcdu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3voavrcva.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xlgfeoiv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3krknftff.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3buwkcouv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cjdvhiau.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gpuyszur.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ssyysujr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3klaiyuve.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ubsuodrg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3bwlcpimn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ffsxvsyz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zcgilord.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jgppvayk.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dpyoresc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hqdiujci.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3swtytsmd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3xylcmsvj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vpspevpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkuiwusd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lxpgdrpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qglzzsnf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3psahokel.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rtdwesws.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sqszeehg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sodpizqy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nnsncdns.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3flphikjg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ucwwikvp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3xdedzqvl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jgvgfxww.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3depcsgym.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vnabtdle.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ijrrviwe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ohdcdsbz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ftpirhnf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3fnxrevaz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gwlsmvow.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3evifpufz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vdptbwrx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3algfiude.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vwzktwtr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3khzcxwvh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wxoftbwl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ytlupzqy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ntoyxkni.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3aspfklxu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3aycdivbj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lkinlkxk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3oahmkkhc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nexgrxky.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lahijjqf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aqtksngp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xkvqwaxz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3yewstcnd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrtrwsi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3aicjmlqw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aczsuznp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jajdwyhz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kdhzqnvm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yedjnzqj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3trtlrsok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpsmcikm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jzvhitze.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zxvrwfrp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxgfjvxx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioherrfn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gejrvoek.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3maafiqnn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ptstuugr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rzemtvim.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kvrrzkkd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3nretimjk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lsnjagmu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3euvanwea.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uacxksyo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3exyyhmhd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yisvphif.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xiynfpxu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gujrksor.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pgqbvvtj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3yfkvjbqa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3idbepegq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dgzvtanh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3eoegbgps.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3nvtynass.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ztsguiri.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3lseatqwz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lcbvmcee.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsfjulhr.html


<!-- 参考信息 -->