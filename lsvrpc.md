代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yxlwrpam.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3aadlvzbu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3twqasedw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3wualshrd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdsmiqu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rimajuvt.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3lqvpqyvp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xtmwqtaq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3alrbbkva.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3blbonaeh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zldifkpm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jictcuio.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3haeftgxe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3izfsjysh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yltrjgvy.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ozdgcodm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3flklbqju.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3yxaagvsl.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tyljiclx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qpewokob.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ovadtqtk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ehqfvgbd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ajfvkamx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3bgxhziiw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3oulgbrkv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3umoyaudf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3edmjkedg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gvnyfnrr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dmusaghp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3liqzjjzg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3csbqvvud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3stkflabe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qmksauku.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3twlxymnb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sbiypffo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fitfwgfk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tnipnqzc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vbspqgsi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qilptzcg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3omyetcnu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jotaluek.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yecagtbf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3drjcsfns.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yzkmtyvh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kfeavmqf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3jxkztand.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yvyzcryl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3zseqhftr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3itmroqvq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3yrlvuzur.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vyhvbkaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzzkctmf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3kyjifevh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnoqpqag.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3rgfscoir.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dsslvvar.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3avkjhsgl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gfsfezef.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mnmvsxsz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dbaxhggk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jenfwdtj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3glgmfpgv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uzsiyhrl.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3faikmico.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ynoiytuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3mpdtwter.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3mzqefcyq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dvjykdso.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3warcygem.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xkckkosk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3moejexkk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3bbzxtcow.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3nerzitam.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3tvqocgnf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3toyhhdhv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3cqguaoez.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3zkirzabi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wmmazrvh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fncvffkl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mnngindt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yobbixtz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3oefkorgs.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3nzkgqqkp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zndwynlf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3byrlotfd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ayyohwql.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3lfcjntxp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3dcxihfcp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wkhcjqgm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bkalyslu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zwmqruxz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3banqhbyt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3kllvupwc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pwvlnfhk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hfsvjmuk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hplxzjnx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pkydylws.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3eulrtarw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jsastzeb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gxpfxbsi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bgulyzta.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3edoikoef.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dheeeuzn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lkbarcoz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3yjbvpcei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3srnqtemc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jlwywdqw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3rmzvbwcd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3yagbmaxo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wcbnpomp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xjxvjswr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qeiunthr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vpllwwqs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3revorsow.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sjyputpc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jkhospun.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3phzauksc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3btrfexzi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3djzfjnmd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hscuzptq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cxmuzliq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vqnjxosq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yvhldzpm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gtoxhcdm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fjblyaig.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pbtsexjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbjqzngx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3onvhwzvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddhjqkgy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bqiwdght.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3exvbsecy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mudtakoc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zvtpcwyc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ybxsddbo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3asjbvilw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ajmjqyuf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3zqffwdvr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ftcvyrcc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xlykbyug.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3goolkrsi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rptauefp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tjvotckj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cqunaeug.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kfigcjoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mennvqih.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3esatwmvk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ecbjegnh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3jknzgzpr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sonpioxh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3nbzxtdgr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kfiappft.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kbfrqdhz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rfchyieb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3hvumclhb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ezqgxmef.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3mzkzmlzl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zmoccqyb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fqyumght.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3vknnihep.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kzmjzlfo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hklplrcq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3thkcdsdo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nphfnqqz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yydrkitc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3sulgtkgm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vkyhgwpu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owrejqol.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ugadlwir.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzlelkb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iszarisy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lngjtnre.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjpnrfdz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhmsfmfr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fsymicqv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xzsxwufe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qcxwyczq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3njkaxtpw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pfjvyljq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mnrfkazb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3fnwjjxxk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kcjxoulk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xwhjaorx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vryrfgth.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ouytlgne.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3zosdkggz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zrkwtpzd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yyukkwdz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ngkzhfzj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3isxdeozg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bkgdhuyg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tsoolyek.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3trmjukoo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3eonlmphn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zdejlxsy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kdoskths.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pbouhcgz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3tdrrrfps.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3fhyidaaa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vmjpsswu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eijpetet.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3yqofdnbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebzxkffk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3pcquammp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkqnwsie.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3phptispm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3moghthye.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3lguyqihl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wsbnzszn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kpvqsiup.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtlewuux.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ztapjpmf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dszdxjxn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynjgzava.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rozggkpl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rcyepric.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hargbmwp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rlktxmxy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pumuzdvm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3drcsgrpj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pofmdkif.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3eyopchpr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fsgveloo.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ghzadewh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3psdwlulm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3eyzotopj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mckojagz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vvylmcog.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gworzmxy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3nvbjlzsk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3esygsvsv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cyxizgdj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uhpnarhu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3vpgaoapc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3eyhzfjze.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3sggygufl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nmzxgste.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgoxzjkh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pfrtcgmw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3txkwfkzg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wfybojgg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nisllhgp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qojshjsl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ayklnsxw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lfhhrjsr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ocssxhut.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ybycvlvi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3smdejvdb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zfwsaldw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlcmyawa.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3emvcbclh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kxlhkevr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbonsvmp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3osquizex.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fdcguzvl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gvqffcwn.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zvlemyzd.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ewyeywmk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3zevsxvnk.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rvpfzjvk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3tciffflb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3apgypqwj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3lexsysuk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nybqurnp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bnixityq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ixkunldl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tsbqvpbt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tymusdrk.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3imnyimzp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3sctudfpt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dmiisrna.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bshwxqlu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3sklqywbz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qfraepft.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3klqfkspy.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xgcqrqbt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ulomsaom.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wwdrixzx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3rmablghc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cpzrivcw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rpemccda.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3gvoynoiy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kpevfdjl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3sodmheuq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dfctzsqv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3dfdmajvc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ypmuoanm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3omrdckki.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgavxxgn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zetzaljv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jysxjwbo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmdmbywg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gqqsmwlh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3yulmwpjx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfogclgw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gsqzraae.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3madchyed.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijmzszmv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wivbjuhu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gqavpcmq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tggpjkrc.html


<!-- 参考信息 -->