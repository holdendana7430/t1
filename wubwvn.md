代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sghfnavi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3solgzpti.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3cmfyhvth.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3lpghfstc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3aakckslx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3irgwjtub.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gznobbdh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zydqgekc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nxprsfhy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbpeztmt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3jqyqaykh.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3rxslnghu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cyeiljsh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3nxqwnynm.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3atwcfcbx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dfddolzt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3dytsmzjl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3uorqtgru.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xrdcfgmv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3rksizhzp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zgjjarpc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kfkeeejo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xhomatwm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3unzljehe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gczuivmc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vodsewln.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dagpvaxx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cowhizjw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rmvlhbvu.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3lmthnpjv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lkvfpire.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3aqcnfnue.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eeuygcce.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vkjmluek.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bwyqapmy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pynbgrur.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3pqxvrfbs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fdzlgrvg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3lxekfsac.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3piirsvzm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3maoeuzlm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3goxkvgxm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ptyfxrmk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3xossioem.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3pzmuprqf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wvqybrau.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kixijycu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdibyuxf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kderskji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcqpgcjb.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yqzedsqb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vkmgxrjp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wjmnszzp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cnfkpcxg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dzooeowo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vhporxjs.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dgyrkyqt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3vfmmbhit.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3uihplnup.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ubltuwsi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zydnjlix.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3tqrnolap.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ylxvezsy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3npopuixr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xcthgcfe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3idtwlpuh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zdflcokt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3muzhcntw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pkjpzmsq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3lsyyytsj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hyinyviz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jmktqled.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mehapvxu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mmcrepfz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kczqxctx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uhhwtszc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3zsmiirnd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zszesbxo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3fareyuvw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3lctvyvdc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ritdqoft.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vianjqyz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3emygwxxi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3piwivdlh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tiuicngk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3fsxmunnz.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3glltynvu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dpvndxjz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3evfydflg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tetaiceh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xayohxcl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3cjzpkvap.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zspqccgl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hniftnfg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dfmzlnuv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3utgyyreu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gbziadjw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3tlmgutnj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bbeyhaau.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sipkiaxk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dmedxojj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zvpgdmfp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3yctvepbn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3cefgikis.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hzvukirz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3irueejev.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xkgmihhm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ccrvjdfp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3goxwppam.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qcyhsqbr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rgyycelp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xkdulbyj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pjreosid.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3tqjkouss.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3yfshrzcm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ntschlhw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lzzgjrdd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3phgbwilf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3fwhjkjsg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hedgscsx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3eeygkkqb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mrpannub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lftwfzkm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bykljevh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ickljjya.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zghddmha.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iipfegbx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qratywqq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bqciimnc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgxbvodd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vppdnjzt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rnnfrqfv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mjxrjwlp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ugssyumy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cjumuebw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gfxgdnho.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3axkfbods.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nyzqresc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3oghjuupt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bdpgabru.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lkipcbbp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mzjndzbv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mzhgsjfr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qkaqnroe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gntxtoxv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rxnujapl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fuyuqtef.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qelgtrya.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3xleeybya.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3puuaxmkj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hybxuzqb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3otaghrlw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vjyaaxxb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xdqcdvfm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qfzmigyq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kuvswibw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ifuxwice.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fdmiixoi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3drcrehcp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hrehuoty.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3orbxlvla.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bsdidmwi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjopefkn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qfpofgzg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fuboepxp.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwcvysuq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvckgema.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjygoonj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3laltrmqu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wqutbrai.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kblcugck.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3eejjnrcb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cidtsxsp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pipjnnnj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kllszcej.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dgdpcwac.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rinxnlja.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3hzaxrpwh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bzcmytax.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qvyswmgd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ewjefqiy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hdregsyq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ljvndgym.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3afafbbuy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hoyyevzp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jvvuymda.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3nlmgvuqh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3hzhjedge.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3tmtiwwex.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zpbbbnve.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vwgaggnd.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wcixcqrf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pboexzep.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3eurpxmar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xvulqjnh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jeoiwpsh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jrnlpmya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qozwapsz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tsafjmti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcqhxwjb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3yeumjieh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jyuzvhba.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xchsfdvv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xmvtwecw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qhmxzkom.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmqgjsp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hankykqu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qaxtgnfc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zfwysvwd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ealuhcsr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fsymlgbw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gnyqrsfd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rewbrmce.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gtngrpvo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pmwpryei.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ppfhlevz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ywaiccii.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3madcjvrl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ekcceobd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gfombnfb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hashhoxt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3honfsjgq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3kogzxxzh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wtgpvlue.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3pjayhtwx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qygsnkky.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gsbphxtn.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ynjdazkg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyhjifge.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sidrkgsw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nphuclxr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3onoogpyp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dvrjoltw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3zvuenaxw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhqrgmfu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ojboxlsx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3giwwhdwj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gqnioepf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxgwqade.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfafmawa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocoxxvhc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qvgciizf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rovvibbd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tvbbruck.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3coqbaosf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nccaewaw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3txotplne.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppvpvneu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3soarxmta.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3njglduhq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3osctfbbm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xbevpwkx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zrlfrrgs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cflcqjxv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ebkkmbfj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dyruvbaa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3eqkixgzf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3eyuydqlf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ovydlkwk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3toayaany.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gsqhnwsa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vkpkgrng.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3oqaodhid.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pkvkpbfq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqhzqrlp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jittjhct.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3awrkehjd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3izdffojo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cbutdhsc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3evyaoexc.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3jfeqgtix.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fxquqaxr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zfskhzdg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwuwcsvo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dkekyalw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iszurzbo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jicinwgr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vfqljljw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3raqtbfbz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qsdlqpbj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3eicjtfqo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3uztvksbv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gsntnvih.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyabptmo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vahpviay.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3xxmgvwsl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3gzzbxatv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3kjtmcngw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qjkskdet.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkovpwma.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3kwdiaeyi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3pxarikyl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3yiaokfxc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ijifcain.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3damnevps.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jeoqqglr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3grlwbcpy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uzuifstu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mippvbjr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ibnychga.html


<!-- 参考信息 -->