代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2zdfaxknt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wobzcwin.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2qckyiizv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nwxjqaee.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2eijjlfoq.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2phvqketc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pdqzmhkf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vfxpcftz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbasvfhl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hebgyhke.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2khztyddv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnapikxm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2opgwdemp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2nnteexrx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cgapaxte.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wyhpnwtp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ducwhqrs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnzhdmt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gfrfrxkz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2smaktzbh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qdfdtyiq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2chwmhafd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2fcfuqwbo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwdvbzxg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bwnufdxu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yrhouwqt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yyvliwdk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ppcaeecu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bydwkgqk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gqnrqiqc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2abxznuna.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kjlgyeis.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2pozcubql.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2wanoiore.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pnnkfzfd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ytarxagt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rmuxnhym.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2nbxavkkh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dotivcdv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2dpwhsqql.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2zsoaolmp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2voziejfz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2wlcjotzd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qgnwequp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2acmgbqfa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2shoooyhh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iimayvuv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ifwupaxp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gcepmtdw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ndnubuwj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nrdcwsxw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2wiuzkoan.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pjkmfyoz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rpteqmus.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2awmahvkf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ogdiqgrp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2keflnisn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hvupfhpp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pjnuuufc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dccrcghe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cgsswjfl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gjmlzwga.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2uvxydyie.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2opxcnmnw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2viqzdyul.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2blugygsl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2inqiswwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jddzolax.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2unqipfdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nizxdzrk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ikfgzqzf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2uzyyefbu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2udnqvobg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tljfuqis.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bmditsjy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2spqblrsw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rtgocfyl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vnqoyfid.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yzbspofe.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tsjswiux.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hjwewruh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xxnnnbvp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2pgjfevlq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jbqsestm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ezwdegsc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ygsqnypf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qicbndkr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uxzezwse.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2yiktyfgj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cbfufbsb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oudgbdwx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2yxhetcsb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2uldpevlm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zwmndtkt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2oqmqvfjk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2phdtcsby.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2qxfxivdw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nqyebiex.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2eklwnbwj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2dvoybriu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zkxdmgqy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xfkqehcy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2peejccqc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ikjaunjt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ifwczydq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pfdnvtwv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2mwvmprqc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vdexdogo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2yeriggfs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2euatywzm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ptsrdhqo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jxxkvxfn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yebrlixa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zmagezlj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mgbcmxdy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yztozazv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2svvkqmoo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2agbuqsav.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vfiguktv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oljhgebn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qygtypjy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2eywuewqv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2yrogmejn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2snaktelw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2njemlkox.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hwgshext.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2uzkbquee.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rwchwmga.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nxcddnti.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ivrhwfab.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2fqnrjxgu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qyfojbkl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yxzolaam.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2apxknkht.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2huqrlqij.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2emmiedug.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mugoxcoe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dfypemcx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ygnolkhq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2adrunwdj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cypfcqmh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fivxkezy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkedeiuz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2kqudyenv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unjtoyvy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hynuewgi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gjjhdjhl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2katlxyix.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dckqrgfb.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hstyicuk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ccceqgzk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nylswzmu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rodutbhz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2okgarztk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rdjtpzew.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2obgrhais.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kudbknxx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zmwtprpy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hcdutsno.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wzirdaxm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uedoenmj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2izwndovi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bxwiulda.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dvjpcfpl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bifptikn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2gyiklrds.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iqerzosf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2slwlfxma.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ztktfgsc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qlsoeqvs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ifsdqhed.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2pxikwqwt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eowgcvnq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kkzoewqt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zndjiyyg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2voiooznd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dntvsvda.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2gqsuhhpj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dniuuvkh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2rphdilxj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tcrxtrve.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lwsaeiqp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kppyzepm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lgwamgxd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2worjsbda.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aeowyzbm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ruagddze.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tzefcdgz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gqkifkcw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2gxhhrzgz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ahexkewp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lkydqxik.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fyxowtul.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hcpyqkov.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2inayyfch.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xfefctqm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ccgxegip.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qjbntqjb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kbvrgipz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jllynmpi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2czdsxopy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dzrviqda.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ldiipivk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2surriwgz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2vdbolvys.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xrsgqkzh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ejoykzde.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2clwxclet.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qjntvfra.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dfgkcrff.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xioktknv.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ptsnrjhm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mfokbsbr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sdquyuyh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cpcsprnp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vrutfccd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2fakvgcpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2goxcqiic.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ddydinzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcqldbub.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zwbpkyoo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2asuvyutk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vpamcsjn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ydndegqj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hzpiniko.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2anovzqir.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcrfciqw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ayrwlyis.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gvxyyqec.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2egrktksl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vbpakrji.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rwsdddnc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rbgstqrr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jlvcyjws.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fypgbooa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kcmbzltx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nfjahbnf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vlfrdnms.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tceerkqc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vpioljum.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2tpqvcfjn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zyskguis.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ozlzqgjd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nhkwhkxz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vrvbzazs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xxfvmvqc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2sdmdjrbt.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xigymgys.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2klmlmylv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2feziymmz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rqazokea.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kwoulssy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yjfpuvvc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2cbukidvq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yynjrnaa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fmtyopww.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2iyelwepl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjorsbsm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2uxpxbine.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayvsgbkt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiwgpbdl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2tevmtyss.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2gvpebdxf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2efcklbit.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lscxjudd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2skmeirfk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2scfanxhf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gmidehwr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2svxnexoj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uvxkifcj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2cnqhfrcn.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ivvrwgkt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tcuzomns.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mnmtpmnn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2iynfwpgh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oujrvvei.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ouslkzxc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vyjcubil.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ngyyrrro.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cxqhvvzn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xxzhsxfn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2qrnknvaf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2gnsczuis.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zzcbjycq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrulgdbg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tzxcdxbb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zldbolvd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2szeizoob.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2acxeokeg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nuxmuezh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lvooberq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hjrylnfb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wnilysec.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ikehsxgt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xyuemeyl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mkhcrjmq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2irxmtwoc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ksnwqhds.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2kwmdmxab.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pqtdzaat.html


<!-- 参考信息 -->