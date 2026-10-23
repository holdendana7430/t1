代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3arqojjsj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ekbohowc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3xjgvynde.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3veyavplp.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3aysuwfjg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vfjxefsa.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwhjofp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvjazspf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhjuwmgw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3mucjkawc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3beknfzqr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xqicxezl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3npovgrnq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3kteurptw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3xtxxykex.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3yjrvrjcw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rllczmzv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pmshratw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3weulqfyw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3pthyfpnk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3yllchvcq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ebalziaa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxsetwli.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vfdydvdv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xuijlbnz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ktkdajsi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3tmrgxewc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3hnuzwray.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vbromkxm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yzmlvcct.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3teytrkgu.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkpazg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gtcsbwxa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3uphmnmas.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3yezhcsrj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ixijejrt.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3caxzsnwr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3smaeniro.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3utoqoxzy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jehwktth.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mspwgkrp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ulptgsdw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ughqyplm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3txgiulwu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jzzpvker.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3cjirdlhe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ocdxgbvs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3cipjupvg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ebhuakii.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yekdatbw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nyrutdrp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3wdnuugsd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ejivjiiw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lsdeynzl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3okidxyia.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sbectpmd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jgyenddw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lkwjicsi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3fveoxaup.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3ocbbfxgp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mgqrroiv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3hramttlb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dcrvbyup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swjipttl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3pilvnkhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnebeyus.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3iyatajmn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3tjvzifjy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3grbafnwy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rgzphilr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ovifnixg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3mbovtsjd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3reguwaoh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3axlhkszx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3olhnohpk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fjayrluh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kvhzonvp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3fyglwbeg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vpedxxdd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3tvgkgxhm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3uhazzsah.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pcyfmhru.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3cnntronh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ubkhhnsb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3syvyfocy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tfyxvidx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jeuctrya.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3agawyzyy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nzbnucax.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rvrqetcm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pqtawhzn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3cwyqewlw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fcvaaoke.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nrdwfjxp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3mszbwmcl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qqxgmjav.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mrosotlo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zlduzuub.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tnowbvnt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3vmqzhgrb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3smyjhaol.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3tzohznod.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3wevrpgmr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gwveqzou.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kpbqwinp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qpbzcmhc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gatgidpd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jmbiwkws.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fiqbhtmh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3otrjjjsd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ejkdljik.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pffuzppp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hdoljxcf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3womvpgvd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rskyfdwy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ygemjetw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cyeetyjd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ywpmgbwp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qbzqovax.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3sgeelgij.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mkudkgon.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3otgkwcok.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ufmdobte.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jzuxivll.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ondvafoj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fhowsaah.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jlcijgow.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lmdbamwg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uomrgrlm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xwmvqfbr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3yunlrltc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3knvilpkg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jmywjjdd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3npnnrbqh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jpntpmpi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3twmyxopd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jsrncark.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yjemqmxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbracuzf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vunwkacg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oljasdqo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3njazqvpd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3btiszdwx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3klapicag.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gljfhzic.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cguofjig.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bmteqzww.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wdidfjdk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3txjuitvp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bajixwvn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qxuboyyd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rbbflzkg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pwevnljq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3evatssyl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uzpvllfg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3idpvgkwm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3foisepde.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3omhxiloh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hqloselv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qizqqzbm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3enbtimjy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3qpcclnqn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jzplnerm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bfcbmuyg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3osmoqemh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3denrnphy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3oslcomrd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3dwrzxygl.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fmhxpeny.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vihhavul.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qidrpzoa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3czidmwgg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wqrjsxwe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3duxpawmk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wpadbzhb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bduuheur.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zkyqtbtm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3nllgormo.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qeuvcgeg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3balyachg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mvmndpto.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3peqbvvcw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fczgtjyd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xzurosfb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hebrbhnl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3aysjsmid.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kgjbiqxd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugnifreo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ejiizpps.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3uemsiowr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hngcmljj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3prpxnmjz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3fkfdszcl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3exwaypte.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3hnqtmroq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lafffowu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3njvfvncg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ptkfhjhu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3jdubstpc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fxsxbwak.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3arzoitzq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rgurzhyp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3bgzfagjc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3skjeastc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3psbjssoj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ofjguzmb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qgwkjcgn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aaqstfxp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mxrwogei.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3pvaxhrzt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wlevdsxq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3lnrkwnxf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3btcuttel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daafyspv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3dhzskblh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwdpbmtm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qjjiqhgx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oxywoddk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3otgvosdp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3drgegvrr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qqttmefk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxunrymo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tiuyyani.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yxvnisit.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozaoozfu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3rfsqakdw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vlyhhxqh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gqfcswdh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zyngueej.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eiyeudfu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xlvpfips.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3figabfcp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3unmrfrej.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fymhwwtk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ppuofvnh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jlcewcvv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ldvtbidw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iqktwzft.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3awopxdii.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3azcjrjtu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3keegdioi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bowztotj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3rrcrpeej.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dnyywygp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ebhyrzpv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3plzxichc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qgaorerc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrjgtct.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3iugecrli.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3wxrjhipq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uxmzopkf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xvtjwbfv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3mlklwpjy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rcyazhzd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qoxmrfhm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3paadoqtr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gdehfrdm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rezhwrgh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3idvkyhgj.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3avnpjnnx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3supqganp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3vtzklrnl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kiksszes.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nxpfljpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xjebwmkp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xzcdmmqw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3gkfxyxxk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3lbkafnht.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xmppmpqm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rlrgvhoy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3mfpmmwrx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3jdeiczfa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jhephzvq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dvutqfct.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3zgqszelq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lisqtgil.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3twxgzxor.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ptmpsiha.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3aefzmfat.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bqmpqtfz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3urcpaxib.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xfmeccmb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uaptnnjm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3udebspjl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3onrprjwj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mfwehiao.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yqoqqqdn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qeytnehy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jzadahhd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iwxqhlyw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lnjcches.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mrpnsflt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ydqrnpyj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tjvccrpg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3sbvzofxz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gdlnvtci.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3utrdtpoz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3jdvmatdv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3hrwyctly.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3becplnlt.html


<!-- 参考信息 -->