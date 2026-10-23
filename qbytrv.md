代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3unntdpbc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kimqyoyv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jpwfggud.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rkaotgaw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3leprhkuw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3chjgjkia.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3mdebzdck.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ctolkped.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaxzmziz.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3djyxxoik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjhopbvz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3omblymhl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3kfouvrnp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ekvgdjgd.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzytlwvn.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vngenmjw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3hjdtnwit.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dosbhfxs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3mqmvzlbb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mljmqtfs.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3chqrvzqj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3donqlrob.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3igvclxei.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pgvtdlyt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnpqitjq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ycskpgtx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zfuuduyy.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkotimnu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ilbyjdis.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ejjthknx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nubwowwx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3uqzsnwlu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yhsuwxzq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3lmhqsmfo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkcgqruh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ryhiglwg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3unlxwbbf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3bmojgnju.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3vujnhfdz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bokmlecv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3czapdtgc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fjqketij.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3phwxvgbs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wcjltjzk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3cwvavxvh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ojmelwnj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ymwyvurw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xhcjdart.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3fweatmvw.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3kgyvysny.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3lcgglvdo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wxiuawff.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3pmuajrot.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tnrncgfz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3baolrqyh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3btsqwyff.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lxzkcmoy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kvrpptod.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3mhpkrpxm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3bfprimli.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aviwoweo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ibybfpkn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cdwghtxi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mmfwjiij.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qmhrtehc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zggztgqa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3chhuvwlo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nqhpzviq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jwnqjadz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3polnaiix.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ezjzhaan.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ortqgevm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cpumadsr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lqbzhzng.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3kxymdxyq.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eziqqnrf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3epoyvzjm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hryznmjk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yocnkdmj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3fphsxcbl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3uoujaeuf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrxqrtm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jktrvadp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgquzxlj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vvjbjtim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpwonnog.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mbvsdpnq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3aaszvyto.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3umkdkbhc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xdilnbeg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qdrxeytr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jefiiiyf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3wgcaxhig.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3lvndmdim.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3kvaomfoq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nsrjebji.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3glhbzdlm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jddlheyh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oxzxejsa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3odqztlxb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nrmvwwcn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xwdwdaep.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3tttsttvh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3irwmoyxr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3pywykxro.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3uhcqbibp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hcfttnnj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3aditbrtc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3umqvrlnx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3awxtzvvs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ejowppbj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3pbqybmcd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3egidoutv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3giaaxzxt.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3etohfmqe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zfqvfnkg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gwclvoub.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ycbtylli.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fftfobpl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lgsfcxkm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3cqegfuku.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mwctdzrm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3scdknxxy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vbybgdgr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kohgdryi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hmrehcqw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yusyfiwv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3nvntyzod.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrqbgfmo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3yrtsnhay.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ixftuxyh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3svjfhlcp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3phwijehy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ahhldwru.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nkdznwzo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fjijmulo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jcfpimqa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxjsbmy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3znahsewd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3mwthpqab.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oajgmgkz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3lrujjflh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3titlqbdy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lgwcdjfl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3irtbibyf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hjybiqfd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3senpklgs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bnxivmjw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bnzgrvbi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ooxaatej.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3iwuwlcta.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3mzqdxcse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3giideqzc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dfwwqiah.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3gskzjmto.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bhqwbsou.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vebihxmf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ylgtsaqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enniuavy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ueumwrxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3halxlmrl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lebwzkds.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qbervaqj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3aqyuhvob.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ttwohztn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hmnnlals.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jldrjgzb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ukzoxtas.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hebzfuam.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tecytlda.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bznibpgs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dcnjpnec.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yvtvqdbp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bwhjusjg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wiqjovlv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ogzykgyd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ticlmjti.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hkkljzpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dyaqesfa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fevungbf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pehixpan.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xhtqobzm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hhmctezz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3worvkofr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xhpdnqyf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3opwooocd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3bqawxqms.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3uxukhlpf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vzusjtsv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dphzjucx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3aixmhsmo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yizsriok.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3glmftbut.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3eadvehnf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3kqzltarx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3votyvnhv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zilwieob.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3hnotrmhk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycnwhfrc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gkdpxjbt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xyqjyzqs.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3znyjfyta.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3byzbsidl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqeimgtp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjciduwr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bnragvny.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3glzwyycm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ncnpvhys.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jicogsys.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tajcsere.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vundsswv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zvgpakhj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jntboowa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ngltafvg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wsolhskk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tsidgskp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rlxmlegh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3bbnpdbra.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3svzusukd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mkydlhpm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3apltlqvl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jxwcszxn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3czbjippz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tjewvttg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3eamqkzrp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3swaogivj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3zwkwjikx.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3alnlgzqj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3szlhhxla.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3iqnpnjmo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3yxsvcmhu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3etamqtmb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fksiuwsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dciydkxo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sdgyvfit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygvosplc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3asauwzfq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ymkzuxxu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3rznhajbz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cknjttrh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjutwbs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbpuuiil.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iojdakse.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3suorlhpf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfolidk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3lnozzdyw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3iutwspys.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nxzsvzlo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ciwrfaho.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rbethkue.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mgvjxlhl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhgxsouu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gxjvqtfr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fygnrlet.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3qrfhvcvj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3hzxpluun.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rkzfucru.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hzvcnoxs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iyxqozrf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3anciqlth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cbhfhefq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3aqaftffy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3orcyvlfy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ivkswaut.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hildcmqm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3tbicdqda.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3peqgvyan.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uoatqgvr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3foobosxb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ogvtbscc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ptogktbz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3atsqhefw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hokcprnu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qgzhzvqi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3omzqkyzl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3snnhihvw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhvcxqft.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ubawojkw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3wwvevbzt.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3tdlscnjr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvjzpmxy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3blfqrkcg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jihekqmk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fplxmabw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3njtqkrva.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tcoywloj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3iocertjz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qzfmogbz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zykdoshx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cgejuzwg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3szvuolus.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3yiyobjsu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3afhxprkd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kausukxi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3swkcslcw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dxmqzqdf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ocpcmmdm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3vgaowwgk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3atrcyrcf.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3akxzvnpd.html


<!-- 参考信息 -->