代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ybfvhhrz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jugbjbkg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jvrztqdt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hiztfbvr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyzcjsk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vetdumlg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhkzweos.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2ifbuzwaf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2phtfhjkn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2cxjaunoq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qzsvelwh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2ucmvpfnu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2phlojpvj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hcvqafba.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vpvpscsx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2txcnvgdg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xclogead.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ludaaqmq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2zrsrrxll.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2hifqypnc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmawwbfr.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2eswtojdq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rxozouyc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tblsaest.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bdhixwhp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qpjzpilz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2tpqivtyd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ehuyyloz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2aucwazoe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wlvlbrtw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2thmdlcfv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pjwcqjcj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jxtwlmlx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2abgxxbgi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2swosmsyf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cingtnmc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2neinnctl.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cglbklnu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hlttrokk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2cmkqjivq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cexzhfyr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tyunebcl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tpvgshcb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gxnrimnp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2omaxlggm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ddtavfde.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cngjwrzr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fenkoaux.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uyhlcvks.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rooshzeg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2htrixmer.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pqblsxwu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2xssfdewa.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bxsfxdlk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lxyaxltb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmxczacr.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2wixyqvnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dwpxouvn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2oyazaqke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mnxjsdqj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gxkfckdr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wdsgagoc.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2acvnwumw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2dzdsmqvu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2auqfqnqb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2sirssdql.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zmxridhs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gfzzjogi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cgijjfbr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2mchzqynw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ujvnpsgw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehdmkssf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2tuwwhlcp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2munowcxp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2rvaglkyr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fhhxepqj.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2iialgumn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nhyxqpyx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lifsshkl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xnfleffq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kcostsqb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2yepsdlqc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hvpzqvvh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2erytcvyh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xndjqchh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2arrdhast.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qjjewuvd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dzvpsdya.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xbfyhlor.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2noxtctnl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2klklxoby.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2irzlotsf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2nrpmkhmw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ctphbdnr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2anvwodmk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vglnpyjv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2durfjbin.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2axtrbzwz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nnqczpev.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ddrvzwmg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kkftrqnn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zradaacx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vlksxrvm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2prtetvih.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ktworbgc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ddbofzdb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aabebruv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jitoifio.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2loguyxri.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nspqctec.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2euwawjwb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2zxwhsnip.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zrlgyopq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2npovknkb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2xgrsrolt.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uobfhnae.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2znisfzxj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jpwzkppp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2kkrohfaw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rrcolvpk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iryrlgni.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2lovxzdfo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2adxpbozg.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2phzcbhhd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qwwvexzl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ijdzrfzd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2scvuvdbx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2otnjgjmy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2izpbaovm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tuyfmzms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecxcaqfl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tzldqjrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldrwpoux.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xsafvxfz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kwrhqvfe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ovdjeioh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewacepzy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uiwaolnz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tcjlgsuj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tlwdhykj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kbcytymq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ogppjbfp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ikqfwszd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2edgdmlis.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ncdtrsdh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nohmfwif.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lsreoppo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mopzxwhm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2myibzsoj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kdwymhhr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rlqjawin.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2avjcvqvg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vvnhqzmm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qactnqkq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2reldkizn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2szeltzdc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2hlusmrgt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2qqtmeeiu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vvkmouxz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2chjvuzmq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cowktuce.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ktkbhyvl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vwvzdpki.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2umyoerne.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zjgdijkl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2aqpozwdn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tikpfutd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dkxhvodb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cudhjukr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ozqklvwt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vffojbje.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gpksmdta.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzevsoji.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nawckvut.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2szudtqyr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyocaout.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2waktbpnn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ailmdmfi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lwobybqf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uebeetwp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oqutqkcs.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ctgpxffg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hvfrqvyr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hvfokhgn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ojafeuzt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2olsknwjw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zkpprmum.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xenhhqqe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jlrhoygm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hjvtkdbl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iigtvoti.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yfazpdku.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jfohvupu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lvfxnjhw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2qkucprbu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2efsneheh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xnulwlwb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yldrjnss.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rgqdsqrq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nwknrvdw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ncgdnpmi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cmaedmax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ugftaimx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mtdmdwbr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fclztyuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jascwnep.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pyxsbqab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odtdbxrz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2enfnkvqo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndeabect.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2adqvooht.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tmucxjls.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xxwkzuqf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2efnfbmsv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytiyuayt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dinqptja.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ubqsatlc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2zrmuihdh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lcviedet.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tipqaybx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrqaiavo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bdubohmc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2wewgwnqp.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofmunwwf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hqqqyiuf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mhjhossg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ogfiyrha.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ruusyxub.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qofuasmk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qcjrxcys.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2etdfuefs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zvcbvkcu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2aaabquxn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hmrlhkql.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mgewmnel.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2yjagketa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2noodcwte.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2syznwrom.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tpjpnovs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2duuwckeq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2alyxmcgj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2azohbmhg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2upxakrey.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2quyofnox.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tiedcwhk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pbptzypf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdgfphrg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2sihtvxgz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zugkbezj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mzzlxxvb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jsomhfsd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ddpzpxqd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hprxijpl.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jwjzrpgc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2mnaiajxm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vjlixuyq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qeltdwcf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eagrsfqe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2cutvwipp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2pusoctgb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qbgcuwmm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vlonixuv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2finippcv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2boqfkoot.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qupzckgi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fefbbtai.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fnidnpex.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2odfyejkp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hqstxmnw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yvuqsaih.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lsnyjyvh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2shxrzegv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cozpxacq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zjjoygfz.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hyhwzvug.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kafmoyel.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kdpfbyxu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ltzzuunk.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hmeiurol.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qbcunpbz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wxwkqmuq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2agpsgooy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wtnzmgvr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rbvihqbv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mcrvorby.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hfuurjvi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2avumgaau.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xntwipre.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hzpwqxlg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xgetxqjl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2npqixpkj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bkhnpgwk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxdjoikc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbcilyz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsijfdcy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xdyzfzvh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2uecjomqr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ormqofsu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yrjrttfb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2tfickzwd.html


<!-- 参考信息 -->