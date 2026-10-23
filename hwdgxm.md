代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3etnvxmkr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3gilckbxf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xlsfppln.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ryymetmt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ussatouj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jztkfxsc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3uokpipnk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3unnsturg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxirbjw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3eclegkwy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfestohg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3uakegopq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ipgmyaxs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nhktneoj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3xxedmpon.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uszyhudt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3oadumcec.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3etvsfjhl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3axbfsivj.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sxiyqfan.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3idlituyn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wjfytbwz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wttgauwe.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3pzwyqnzm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3cltlceub.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3mjdsgbby.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3bmppljof.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3xuzuyday.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3tdnpbvxw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3eemlxrdy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3mzlguqgw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qfoxcnpj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3osvzneez.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3inktgeyl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dmhyvpyo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3umwwnvtl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwlauhv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3qoskmjce.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zhsjenit.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vpvnmpnd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bapjdpep.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tunzizoy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3imnhtxpg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3grbkkcfo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3uoufalzi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fcoarolo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3fmzuorvw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jnanrgan.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3htcowiit.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jvcgslxb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rqaliahn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3tmbirmzw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ykchhmtf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3macyvccx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kmolrlzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqqghfhp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wrdkttsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndvtpfnx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3vzhrpjlm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3efipjyza.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3psenjqay.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rrqzrxye.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bhsoznlm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3endzldhh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uqeiraxz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3lmifqxwo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3quezxuka.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ivdjktio.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qgrapezk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3usdioudz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hjvlpchk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fjubdxtv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dkqaohpu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3erfbudrg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wftgisvz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3jtkbsksr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jwcmwzlh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3mjhmjcif.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ogxxkfzj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hrdvimlt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3prwkwiqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hlmdlgjn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3orjkavzt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bgyxuhdk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kmtvpxrc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3csalnvet.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3rdcpatvf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ywuqcrqs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3msiabztr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cdqsauju.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jrnjijlj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tdgqpmew.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3cxvfgocy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3maqcfcoc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3iipvjmnu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rmbjpzyw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3znzzzyci.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3czayilei.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3cnziqbvg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3lvwdctdy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvvpqgzo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cihjmdgn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tjphgejn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ryctyubb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xjwnmhao.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pgeqjndv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xstbpxwh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kznwdnom.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vccteswq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3acwnrtks.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jnfgcqvi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3omvorebt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3anuomurr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3dfxfenmu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3mmwvouvc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3pmrowmtz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zffwgnrm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nfkrhexl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cwnmdtkz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3myobnnhf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ulghszie.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3rkjwndvr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dpseuubg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3isxrcoii.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ngvfjmzw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dmbxrpad.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qbkaqoyw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wnwaalbw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzyokzv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3klvbzafj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgviwoua.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wadwprff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vefkfbej.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sycpkwik.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lxilvsle.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vkfbnkhd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qzsnltzo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xuzrecee.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3duhwhwjf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3znybphcp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3pehkniwt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yhgptqzm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3aittjykz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3editxjma.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zaviwpwb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3firmfzza.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sconfguj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fmhmnlql.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mngnacbr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xktuxurp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vnkdzjxl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xwjhpiee.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3njfoenzi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3enbbjsis.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zklcaqrk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xmnfuglc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ecjgawhv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3mqkfvvqy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wdbfzqxy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ystvwccb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3csewkxbj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3czpcvnat.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3uottvvot.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3plmynbrg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dwvnzpeu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uqrzcrpr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ephivbtt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gebotxxa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3nhrrebyc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3sijfcakp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jybdjxnp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3onjqbxnl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3biyfcwqd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdtrsofy.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yvtgnvrz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyfpyivl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3yxrwzjkl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3kbsjrmqq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ixirfdfs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwcwydw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ubxsoacy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vhwgmtvw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wkgychwh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3faraalvc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uupnzasw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3vhupxhdv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qjhnmjsg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gtdeypzn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zcozlazj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rhpvuena.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3oonjxmzs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rzapaimd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rqtsfscy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nlphrgfh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xgsuphlp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqebdec.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3mvpaqmjv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3wjpnglpe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3peowrslm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jylfmlqf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rwlvywpf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ngofqfjz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xckuoptn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bmwvlehx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wuhwqxsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyoglsdz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3wpmvgifx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdnpgjnk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kkhwwovg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ladkmmjh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rpgktugs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ectlvkxn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ewlnsimq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3snbbosjd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xnddytsd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3orzulsjj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jicjoosa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fxftehod.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3auzfalwm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3yjqvvuhn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gquklbdv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fwzzrpbz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3dhvydwrb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vxznhzsh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gjnfmxyr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uxiwipif.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3jysttwyi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3zjvqgnpb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3loierhux.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lhfaeuyi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3axpplmpj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lwkmnqkz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ybzfxbfz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qixvjzmo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3eogkothx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3nofabbfb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uksjodsq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikvnwdvl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jhqyrfuc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3prohutpw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jyjmoixo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3cudvhtpm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwnbprip.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jkthjzkl.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wtyvcfbv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hxbvgcjn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxmejbqa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3srvxsyqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejkpyagd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jtovkwey.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3nljyyyow.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fpbjcsqf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3umwrance.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmidpjxg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wlekryzz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bfpqaude.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uqoixcel.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3chlczweg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3phgixeav.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3onvwzpea.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3etionlds.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rmzroanj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3locipncj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pzyrrbjv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3santrdpu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3hbayglxc.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3hevnkvfc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3zspuukob.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kvrxaciv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jmlxeefd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rfvinwft.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3rhsbitdg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3uqlpbcvx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bxddmqbx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3anvulqws.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ddseidpk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3isctrznh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pqrsyysc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mufzsckh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3odelbozt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3puehgdzk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bzxucozp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3btbjwisf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zsodnuqj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jlmoenuh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nlbkdtgp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3kuzlyiod.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3denxhrld.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3whoadsdz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xtkyqzfb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nvunmwkk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ficgplty.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3osacewxd.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pgdzupog.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bphnmzcz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ncswnpxg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3skoioceu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvwzspfd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aymcbigk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3yzatbrcl.html


<!-- 参考信息 -->