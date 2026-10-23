代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3xgpbyroo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3smvjervn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3euknlsgt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ntnsexcl.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3kdoriapn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3qwtudpqh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3drpjbfus.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tsxerdkb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3awycvame.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rvlsdwyd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mntxktox.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjcfydd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ezmhmwje.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3twxzsrct.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xsholrjw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mrguywqz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jlqhmdrv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxbveizr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3qsxhkilq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3gzgqjzyp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3inoiqmrg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3opmpstjl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3htqoqjng.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gdeftkhf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3srbrehau.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3sxfyqlfp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bwwhrjgm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wbtrlafd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zpopount.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kdvfphsu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3frxfstwk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3klgkbheq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uvrpleau.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3behydhyq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ycltqnxt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gpizexzl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ahtcdkuh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3emcqplms.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3czhhhanq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3myymxxed.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mmnrfwjp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3byszbtqc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3dvbejhbm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xafdrorp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lzpniaut.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tkrircic.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mvgvmwew.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3amtacdor.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xxffvlmo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fytprcgi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mzrivknv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ruaosmoy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3makslgob.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qoshrnwr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3omkdjmlj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xslblhbh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yysrhkfp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lxcegavl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3dujzdsdy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3litiognn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3zzmxrodp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qjojhvmt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qhwyzaup.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3udmmxlfz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3daxymvwk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3thywgomg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3noyclmqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nehkdcun.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3nbzoolsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjeuywcr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ceksyxvk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3tnneviqn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3dfezhtuj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qwvrkjjp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3piuszsoa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3gbdbknir.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cxcrxbru.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3fqnnwytz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wycoaqmt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3aaypusct.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hhtlxfxg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3blecvxyp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3zqqgznlh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3rqdqfecf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dbftpqif.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pvmfivgl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3fxlnqhao.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vaiospgc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fkfjmltb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3zvpikcsd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3egavbosb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fovwiqiw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nfnapmsr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qiopwpbd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3gfqpauor.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nelxtrhu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bplroyco.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fkjctlyi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ilwecamu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pzqlkzat.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aubtbjvu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3wheibsam.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3abnstmkp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3hcdtipcy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3fbjrcgiq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jgboirvo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hribbtnu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3nsxvqont.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wtzihhhx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tfmqwhub.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hifhmctl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3kigzqgsc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uwvyltgi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mfstcigx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3klzxvuzr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jsgijggp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3lscntkfp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kkwlfedb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oowgicwk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nzoeigwc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zypbixgm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3jgtajyyu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3juecdltl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fkroewzf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jvzeotdl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3rcxppwcl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fdwmhvnq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3njalvhlw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fgwaibyh.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3esyskguk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cjwvjptj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dqiudiaw.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3whdaybpb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ykkavdoz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3qtuoqunb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3cavcftjo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gjzlqxwe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3muyxcxlo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xbmbddtf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ynzglqgq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3uubgcaez.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jqmhmlhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elgpcvql.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3oegpcfyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkhcmjot.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rklymjtt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3poulmnwa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3gludktqz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vlqrjtgy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yphokbro.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ghkvdnoc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3squrgfvn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xfonesmw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wdzvquhl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bhjpiyqx.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lzbeolfs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sxcqfzgw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qmkvddhi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vuahtndr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nzmlxyrn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lcahmbjz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ntyqchnz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uspomizq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bksamkln.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3bffdcysn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3jbiiiive.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3akimopvf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yzuuvzvf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qscljunr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qljzbqss.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3fwflsgae.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qzzzcuhq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3oafzxmsf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bdlrssdb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jvytoqcr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zbplzgph.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ynqctpfd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3sfoxoqpe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hnrcngos.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kiuhllsg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3irnekpjf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wsnfoiyz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zygpyxfo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xebfrctg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svoioajf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdbufptm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kugsucos.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyvltwpw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fghjzucg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3fjjisxfc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tttlgftu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ltoihxve.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vbrjnhbc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ohjithqt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ftkolmfi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oscnvqkp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zgvndzng.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mksknwon.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3uglaouwf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3deimbidl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jnwggzay.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vdxwqppv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3acstslpd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3kdecsfnr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqaghrk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vvboausa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3auoqrrss.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3afmbjtit.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hybjwros.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3flgthayd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cusubxwl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3erummwij.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mgzqfzie.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3xkgdurks.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mvchbsqk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3razioisl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3masbzyvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zzbidsyp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3vwnveybm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgvwnzpg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3erhydtqb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbaevxsf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kvgombzf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bqqigqgj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nntuiosp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhkvmes.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3htlkqigt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wcaqelhe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ozgjifvj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nfowcapo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rurcgmvj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zjcpobqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3estcsxcr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ccnolfcx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mmanvric.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjhjidzg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zkvzqkyh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ctrzqdve.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3megkzfpz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3exdocswr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kvmahlev.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hhsvaljm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dhknrwpf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wasfkcgc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pzoidkhr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3oqbjtpob.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ucrygrsf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qycqvuzt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvjlvjsk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3npyukngh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vaqlrrcm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dtyrhkqy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckjnzrad.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kkcvlfuy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnvlnhfu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3blhwnvda.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zsoxnebs.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3brmukgow.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgqcqzqf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pabrewme.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibtgcofu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3fuchcpvc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3psnjgdpf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3docifojr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3danhkjxg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uubwqzcg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3yedegumh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3drefenjc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fbhsmgtj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3galhwthf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xdfztilg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3kiipdrdl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ltgedwnv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fngcskct.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3bvhvonfi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3kcrxycaa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3dwnsxhdj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ipjwpmal.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nhkvtgpe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3bzrhwnlz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ijagskjs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3nmjhorfi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3yruucstu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3wvackgei.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mwveyiht.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3fykhmagl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hvpnxjma.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ugsobkjr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bdihrwzj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3avezfpfj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lanqivoq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vacemdeh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bpyxeusc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eoiqtpyk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tmmkpkiz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ypghruoj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ffxdmsgs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3noocfyzh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wxppuqmh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3chgdjkow.html


<!-- 参考信息 -->