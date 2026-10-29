代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/geegjbnlu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/ghmlgolpa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/govqbfbhl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gzimpihnm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxzgifxgi.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gofatyeoq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gonxsmgos.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/glvdwptxx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gadumvoza.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gzbonusmh.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gjhvxugqc.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gvoktijrt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gonnzsbgw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gytwesymp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/ghcenfsem.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gztfdrrzo.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/glyeiwsyk.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gpjmlhrhy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gjhprptuk.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gwjvbntpw.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gbxjzqjam.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gduflpdgv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gbdvpcxtl.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/ganocveww.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxfoyqraz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gwivjlfyy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gfssktwuf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gpuaklccc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gudqbocfm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gunuftuhm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtxyqgrtj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gfkidnyiw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gznskcfhs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/guponoxde.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gnrbbcuxa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/glqcxhabm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gurzmkyhp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gewgzwavu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/ghnnkanye.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gbbfgqvxq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gvnaxzrqd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gegnqgzgz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gfzwvguuo.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gwnhuftpv.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/gexnmfrqn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gyxwiaycp.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/ghdvimpeu.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gaunviyyg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gqkwskkbf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gexirwigf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/givxjhcep.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gogicoihd.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gdxvddqyg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gtjtwwnbj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gsthixlkt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gnwgslpag.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gofhoobmx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gipvikxui.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gitwhssns.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gksppsznk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gvbjkbifs.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gxwokside.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gruztoqtt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/grdylidjg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwkiikhrg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gbwxgbtmt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gywxihpnr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gotdnijsv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gwzmqtyyz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/grdugwkdl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gremufgek.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gotwiarac.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gvruiqmfy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gnptwsgxz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/grfbxqlzy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gnrlciktu.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gygmfwtkw.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gztkelokw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gpdoeufuh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glpfxwaek.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/glvepvoeh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grsgnilqm.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gghidksbm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gptekvsty.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gceefyxqb.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gsvgzyikw.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gdecvatmk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gokqhfcah.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/giaicjuoa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/goafccfsg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gjvgijcdz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gxoievvmw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gyiaahdsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gbjzulcaz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gbgmjpirw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gyriaahrx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/geqbainsz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gdfrzsfhv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gphmwxece.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gajtubmcr.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/ghtqrtpgu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gdtqjwyph.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gumrmusxi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gesxldmwd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gsenbbriu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gmmsbzruj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gelqzcxdi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gutwuoocb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gmrcxywjo.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gadjeiuao.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gibtndcrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gnitgxbbm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/glqgbihuq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/geoeamipb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gaqufvnvy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gmtsiwmfq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gmdyoacpd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gzhaloxhr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gvlyiezww.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/geimuqqqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gjivgijfr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gnlyfxjfw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gupnbndmu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gwweqsonr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/guclesmbg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gtosndsqe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gpoiwgzam.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gxmdzenbc.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gowpsdaoo.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gjdypmfmj.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gprbogynd.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/grfffzowx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gcvgnveex.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gebwlckwd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gscaauhsv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/grwkavsbn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/grcvagojv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.zdbjq.cn/Article/details/gshilqrji.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gwwjfaqcx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gohurmndn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gfzwrlrav.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gfbnnjzya.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/giohffrlg.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gjueprpkk.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/glmkwdjkr.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gguvsggoh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/grnbsmwni.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gaiscqgsq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gsfnaqccb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gcnbuclim.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/geqzobumi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gtjrjswux.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gjeydcuvf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/grmkzmfri.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gutlbakbj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gukhvwmmc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcetdrdwb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gfvmbjwbd.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ghfsvikyv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvgutoju.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gfrqpiyuc.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/goshvuxmi.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gklrcbovf.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gzhvzwwrl.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gwzykesov.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gbcxbaocf.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gmforpskg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gmkgifivu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gmdkddkrl.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gvhxxbjoh.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gkaylzhee.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfnzwdkij.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gvczqagwc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/glusogxjz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghwrgvjvu.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gqsyiycvm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gxychgmsk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gheomglew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gkouvpqra.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gvjwehrcg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gxieocjrg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gnxderscp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gveddhnuc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gsserlzrd.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gbgdhqkec.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gmjvmdbjk.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gqkjyvnld.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gxnnwbajx.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsafkdsjt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gnvpymqcb.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gccuxlpvu.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/guetraijo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gbhhemmnq.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/ggjatgnfj.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gfjmzqbwz.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gtjevqddf.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsskocmvc.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/glwhhdikv.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gnvqzyxdm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gyappsczw.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gihsfsbhl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gofpnkode.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/glzkyutdt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gtckzqckt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/ggrzfnris.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gyiylqcmi.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gwowlqtic.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gcyhiuuap.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gysaxxncu.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gcfbqaagu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gmszlrqbp.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gxixtdlll.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gjbdwpvrt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gubkzjthv.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/giimovdyc.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gsjgsbkyy.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gztcsnetf.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gasqkrvfl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gxmuldpsy.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gmwkwoyrw.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gqtaseqyh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gmkssdcdd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gsxlxwedi.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/giglboxbh.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gucgygwfv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gcgpxnlvc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gqvetkzcy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gjwbmyrxn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gqsptvnhb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gupprlkjg.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gvqkauxpu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gptpecfyq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gmgzsctkb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjygqqfur.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gxjfxsyge.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gztylkauf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gwkalgnud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkwznycyu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gffqaboxh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gzodokzhm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gidaadkdf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gefrbgadc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gjpukjlim.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/guduxjolz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/giwantrnt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqrlepgkw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gguwultmu.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gmdcuajvd.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gojkkcnyt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gtwcrpflr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gzqntmuyo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gippjxbvv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gbzobokjp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/grgyaplsf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gsjwwzkho.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/grfkacccx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/ggbngcgah.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/grdykwrie.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gishszria.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gtvuypmik.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/grkmrxwgw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gerghhrcb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gachgkcxr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/goazgalqo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gzjvdhoyv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/ghnyzfuyu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gocwhvyyk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gmtloxbqd.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gqonvuyih.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gaxxrqhog.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsidezhnq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gxrifilhg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxqojoxg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gfcezybll.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/geivhkzja.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gdsasajsg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gmvjglsyg.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gcigzonvx.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gpizdxpzu.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gwtdatxjd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/glyubskro.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gcbnmlpkz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gpkmtzfjh.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/ggjqbmlti.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gptflocvm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/grvxmdyag.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gwzkkyfsa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gwnfjperu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gcodvjius.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/ghutmxskr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gxyaxhhxg.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gijgkndac.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/gssurkudr.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gicayioyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gtxsxcjfe.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gnkyatfvu.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gwwrsdzbk.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gvhrpkuca.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/guuhzidmq.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gclrscxck.sHtML


<!-- 参考信息 -->