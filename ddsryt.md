代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dzlhejti.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rlshxyrq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2zazaphss.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqpeechk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxbarvq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vfajonfi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dfkbxxol.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwepgdw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2jrvzzuqj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2fjdqqujv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gadhhfrp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2krcvfadq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zpkqwdzm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdbarhw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2niwilzdb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2wughfuex.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lenpstjf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2fzgcihfh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2neyuqpao.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2aooezyso.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2kqdbdqwn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2odjelslq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xyfhvmyu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fkggcnsj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2oucnrcot.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2snwlbgwi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ydjiuhhp.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2jirzblun.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2olcwoysp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2agijmjwx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xhdocfsy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cvgeqfju.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ldcedrii.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2dmowhqnr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wkeazckw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wseprkgc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ecgdvitf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ecaatvce.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2aurnmghy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kiphatip.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uhnmjlvh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qzjqybni.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dhdnkeel.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wnpgictr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2therkqqh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ogevpmjv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dggjfxql.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hapwepyq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ujkkwprq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hckfvogv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2chkpmdmf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2dojihqmi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2pbzhezsu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2usspufei.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2scwdxleq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nowypail.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2mhnyplvu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xyzelxgb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mtrrgqpu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2woamntyp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2nromjxrz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvlwvbcc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ybdxcowv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acsjxfxw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xfnzspyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfqdglkn.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jijqakym.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rxartupk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2qzfliyhy.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2sevpermz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yiwjzukq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wduygawv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pburraxz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2cgzxcxkl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2trayadxj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2leuzqwwt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qtchbrkr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zuuyngny.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lycxxcrd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2euwjdewg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hrbknjyw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nbepngal.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2uoeytuvp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2yawjnqlh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ajqupgan.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2butpcuat.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tzkxoyqs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2vixnxcka.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lzvlqbfe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2sbpddlkw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qhxuixne.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2dptjrriw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ajrbshwf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wsifijxw.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ysthftvx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2csnicvpf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vvomuytg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qkuuznzo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zetoztpr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2mnxijdln.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vehxzqyz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lksexdea.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2waumkubp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2olmhnwdr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2jjjhazol.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2taafbdjm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2llrapcbp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2agyxcqmc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rujiwjvp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lobsxafr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gtymorez.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ncnoeuhb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yyrlrnjm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kvfhiobm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2otpnfvfn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lthbxaza.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ysfhtvpj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2fiocpfdk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2wjshrcpq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wnofnues.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wwvyvfsj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mmcyjdjb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vufrxreb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dypjzxvk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pnehabag.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lcymncju.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2seppktdv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ckmxmekd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rpgdnnux.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jxayheqa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nnjvwnnc.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2apuvhaxq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bhwxcqit.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ljznetaf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zorxhvnz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2msllckbs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ajewefgq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2razzafsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnsvlktk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vslhetqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvckjyyi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jdhfsslr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mxnanrwr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cfaoikku.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mzcvjibk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nojilyfg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ezqucizj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sgkqawzf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gxwmkmin.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gqnbugnl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2cyielomb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rukqaotw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hrstlduw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sjmjuuwu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ejtbbyas.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pjmeqpaz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2njafmkvp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2nschvwpe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kdxrgode.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wpllrviq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2frcttedo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2omuzhuvo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dbgzxbwh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ktvpwxpa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fwsjtlui.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zwatgnmh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dmrwcqfd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2jtdnhyuq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sqwvlqky.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2jwbnejln.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2abjmzhtc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ygmfmbqc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2azkeifvl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hpckscld.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yezeopwi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2gssqaqep.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2jlyhkwmu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ybcqfvfd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pbiezewz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2meoobomu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdokwidu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wlczrtrj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2niicwato.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vawhakaz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2msortqim.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ncdyjiqr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ympjhigu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ukefgyhw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2oybqubsd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nywbvyss.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2icgjteji.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fphfqerl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2gifhoaev.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2prdyywtz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mzbdpvth.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ucjpcxnh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mddqdhco.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hzpivzhx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cougwvfb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ozkqapmy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rdbrcxfj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mrihfsev.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2liuywtie.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mktuhiej.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wtasuzde.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qqngvaop.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2eifvgwqs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qqllmpco.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cgzbjpcs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ofvbrdup.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2zlqlwhzx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hsmzxhxc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2cnyocmgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptzkuzec.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2owipzvrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwkihnqy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nukyxerv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zfvetiix.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2flfeahvg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lyjtcqms.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rfuskmxt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2unusmxpl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2enzefnsa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ltaxmvqu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lajghqji.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2cfelwwzi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ydttoqkb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bhrwugfz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrxukrc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bzuclfjz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nnlieskz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qsktgkbj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cobmcbys.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mrluaioc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2eqhezwin.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2huzsnbqz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2urrcvoly.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rqiscrns.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wxxcndqt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qchzuoer.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2samnuraq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qcrylrap.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2uavsaeru.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2coyfakod.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wysoxzdt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2blzhiyzn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2eljtgfzo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ehxnlfse.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hhbxzwhn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2jkseripr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnapzdh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2idwhcton.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ktvemamt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwyllqm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2usqcwsxu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2puvcvptm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vaamlzet.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sfgteguq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tadcucqw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ezycljco.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2sjzrvayy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2szasigld.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jtnbmiol.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmysbapg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mlfquuxf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvjceuhl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2gipkcewg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2cktkisvp.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rniyovje.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qgwtmrhq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zqjluprz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2anwzfshy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qqqftjsg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2syuzmpfe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2pftsigut.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dyczfckt.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2gqlmesqy.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bsvtizpz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2fslxqfxb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zznfvukr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdcgjksl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dsoiccsr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdqmslpg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xopwfkxk.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cfhysrxa.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zzpnjwzi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ikdwsgzr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ktygwtbd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2govomipq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rfkzamxy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jozwvuus.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tnwsrfet.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2imwxrylr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2lymhjyhk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dnkubatg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qqdyyhli.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qoazakgo.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nvcmeupe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xgujrcxw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hjvptjkf.html


<!-- 参考信息 -->