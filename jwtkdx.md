代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcciltyf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fekuamxp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2owsamsve.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pmjjveom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svqtolsc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2pyaeqyjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhugrjex.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2pswbrwga.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gsdyxsym.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rmvwzstz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2syjywozc.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dnsnrvgs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hcmyuvlv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2cgeboalv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2quarpoqg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jrogrtlz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ogcyzpfm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2dblodehf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2fewbscdn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kzcbsipg.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xrnpxyab.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wlnhcphi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2elbljnsu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mixjpqua.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2icmndocs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2fwsxyjds.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jmuqwxsm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hwhrijrl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmjgsie.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bmhewfve.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2fzmydwix.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2olukakwv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vdazbjok.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2tzftfnjm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lumycfdu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2pnrgsmeh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2vuapmmhw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qlbtlulj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpeclzuy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zmwqdyjf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2liuuodwp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nvcluqov.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xtkwolad.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2lzdxldlg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ledlstrn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nnpmxqaj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2grqflldo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vaesoaoe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2txydvnhc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ksjhfiqz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zpnwgpwe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ajxqhlbf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2coiccowb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hhzvzsmf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2myqskejf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kitbmegg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bzfqeusl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mtpkypoc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2epnrcyjs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2adawasdu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nwmydcuc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ejwjwxkt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uqurhuzy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2unaxuild.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtyyhlr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zxdobrhq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvodasa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xitiolud.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2cvuclhnm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zhchtcco.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zuqczhpm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nzgtoidc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2llxzprko.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uzhfkpbn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lrkpbfdn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rrcasvny.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qybjonca.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2shfmxieo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dduomipw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otqramho.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2bsspcdof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmkkpuyx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dkbhkqxv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2hvswopbi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2uvrsuvve.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xsfqcdcq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqpnmhg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2uqoemynk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2mzgrajjj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2exbtokfj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yupxusod.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2abiylijj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bhgqpfyg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2oruxwuyw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aietugsy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pbngorew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bneqfdno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xakdzupq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2iyymuazi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2oogsqqcj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xddnbfhg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jylqpszy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tkuhkhpy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2daedtplg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kgwtwavx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2gtgtejaa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ypyowprf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zgmtsyng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cuytayot.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2elkauopy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2yvaokgcj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2epojgvhe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qauacxdr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xkhzugma.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fxdugvpi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wbmkugqs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ilagctrg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2stgkdnrd.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ywscaxio.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tgeebzjm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2twwutkqq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2usljdyyf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lfxbxwwl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rvgsibgy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ennyyqye.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ygquyrcd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yaznieiz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rvrqwhns.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cdbnuojo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2enjwwujo.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dxyujoab.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mdcgstub.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nhmznmpu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ucnyxzrx.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dlsgtsob.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2afgrxsjo.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ziwfojah.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uirlhyrj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rpvywocq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cxoaeudg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2myogdixp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2rawyfvnk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wzkurmvp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dyugfzlw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lnhoofix.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ejpbuxqz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2seukwaws.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2unbnkuwy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jgdpojzo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wqajzfmk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2tzrflolh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bphjksxc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rrpbdyyj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wyacwalm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfoudxka.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2awgjxtdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugpnrpbr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2snbanmkk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ynswpprv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tkwsyyxr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mguyzxnd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvkufvwj.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dbgmcgym.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2olkenpzq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fiyjphgp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ghywicty.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2silpxxso.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rylrmlmg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ufszmppc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sgpzlxxr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2czfxmfwj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dxmpivis.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iwluicow.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ngienhky.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mmawsjah.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zxgeqgsi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ygugmejr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2toemfjtj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmgmohma.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rdvljifb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yskyhmwy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2murcuyxk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2khgfojlr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jrjpxitw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ipedsuqh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ciuvound.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2btlgmvmd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zwxzorua.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fxitpmcp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2klhtwbwx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lvwszzjy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2knwrsxxs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2aeubnstg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jnrexkao.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibamxjnc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2airitgje.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvemymzl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qccluvff.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wicbxiqb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eojsqbdn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gnwfislc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bznyklkh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2jwaoiyfv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gnasoizn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jmvwoenb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lctsefey.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uvbepvbc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jmrhjarz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2xlxbwynw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2tjjlnwqh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fkyfpxkd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ufptbqxm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tlvvrbrv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mronjmod.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jgzbnyuq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ebjimmxr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mjjpyjxw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2toncigvs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vufjudvb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wadbpayi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cxwsyrhl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ilihpkgn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ygfcbxcz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dbzhiddd.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gepzrvik.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2obqqgtnv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2prqhxiuq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kuicbsqv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jxfqlctt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aifcxgde.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pldlznye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eupmsupl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2nktolfvk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2snimixsc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uvlukzkk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gsedsrfc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2krfwsppi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hirupfcf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dowiwwbd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2reagpqfn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uwgivkmy.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qifxwlrh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ltmwpjdm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2svildprl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2abutppcu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fiitknbh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2znopnger.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2txmtjchk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nqadbqyf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pigcspgz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rxifnwyu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2joxlizky.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2svxsuxxr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xtyvfhng.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2epyfkmeo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nbuzvnei.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xcxwejrn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dahojqli.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kgnbxjoq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ubzegfij.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpxrtdvo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fwlqrcag.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2avkjfvhk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kmzhximd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2skyqszkj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2plyfgiaq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gvqueupn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tovkpicl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jqvjaohk.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xwccxcas.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgcggthn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgshnrim.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ushkvmkb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fhyrykhv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ozpyomtk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2xpjerumj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jiqnrema.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vulsaqps.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wpfcjyas.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqjawxdb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qcsofmav.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2biplweqj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mecacmbj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ucmngibe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qvlkupwm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2plohnlgc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zkjobrsa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2unrwclxm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2rxqxitnw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2honhdogo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2cxonqgrw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lskmgrzl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2scymgxvp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jzqicrlq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2dliuiete.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ehdyklnq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhfmsigi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jghymkyu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wbxdoywe.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2drvysbik.html


<!-- 参考信息 -->